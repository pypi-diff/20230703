# Comparing `tmp/tcod_ecs-3.1.0.tar.gz` & `tmp/tcod_ecs-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcod_ecs-3.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tcod_ecs-3.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tcod_ecs-3.1.0.tar` & `tcod_ecs-3.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1079 2023-06-10 15:18:27.842121 tcod_ecs-3.1.0/LICENSE
--rw-r--r--   0        0        0     8465 2023-06-10 15:18:27.842121 tcod_ecs-3.1.0/README.md
--rw-r--r--   0        0        0     3708 2023-06-10 15:18:27.842121 tcod_ecs-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    37039 2023-06-10 15:18:27.846121 tcod_ecs-3.1.0/tcod/ecs/__init__.py
--rw-r--r--   0        0        0      160 2023-06-10 15:18:39.870181 tcod_ecs-3.1.0/tcod/ecs/_version.py
--rw-r--r--   0        0        0        0 2023-06-10 15:18:27.846121 tcod_ecs-3.1.0/tcod/ecs/py.typed
--rw-r--r--   0        0        0     9660 1970-01-01 00:00:00.000000 tcod_ecs-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-03 03:27:18.545176 tcod_ecs-3.2.0/LICENSE
+-rw-r--r--   0        0        0     8461 2023-07-03 03:27:18.545176 tcod_ecs-3.2.0/README.md
+-rw-r--r--   0        0        0     3478 2023-07-03 03:27:18.549176 tcod_ecs-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0    38097 2023-07-03 03:27:18.549176 tcod_ecs-3.2.0/tcod/ecs/__init__.py
+-rw-r--r--   0        0        0      160 2023-07-03 03:27:26.565305 tcod_ecs-3.2.0/tcod/ecs/_version.py
+-rw-r--r--   0        0        0        0 2023-07-03 03:27:18.549176 tcod_ecs-3.2.0/tcod/ecs/py.typed
+-rw-r--r--   0        0        0     9656 1970-01-01 00:00:00.000000 tcod_ecs-3.2.0/PKG-INFO
```

### Comparing `tcod_ecs-3.1.0/LICENSE` & `tcod_ecs-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcod_ecs-3.1.0/README.md` & `tcod_ecs-3.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 True
 
 ```
 
 ## Relations
 
 Use `Entity.relation_components[component_key][target] = component` to associate a relation with data.
-Use `Entity.relation_tags[tag] = target` to associate a tag exclusively with a target entity.
+Use `Entity.relation_tag[tag] = target` to associate a tag exclusively with a target entity.
 Use `Entity.relation_tags_many[tag].add(target)` to associate a tag with multiple targets.
 Tags and relations share the same space then queried, so tags can not be in the format of a component key.
 Relations are unidirectional.
 
 ```py
 >>> @attrs.define
 ... class OrbitOf:  # OrbitOf component.
@@ -211,17 +211,17 @@
 >>> planet = world.new_entity()
 >>> moon = world.new_entity()
 >>> ship = world.new_entity()
 >>> player = world.new_entity()
 >>> moon_rock = world.new_entity()
 >>> planet.relation_components[OrbitOf][star] = OrbitOf(dist=1000)
 >>> moon.relation_components[OrbitOf][planet] = OrbitOf(dist=10)
->>> ship.relation_tags[LandedOn] = moon
->>> moon_rock.relation_tags[LandedOn] = moon
->>> player.relation_tags[LandedOn] = moon_rock
+>>> ship.relation_tag[LandedOn] = moon
+>>> moon_rock.relation_tag[LandedOn] = moon
+>>> player.relation_tag[LandedOn] = moon_rock
 >>> set(world.Q.all_of(relations=[(OrbitOf, planet)])) == {moon}
 True
 >>> set(world.Q.all_of(relations=[(OrbitOf, ...)])) == {planet, moon}  # Get objects in an orbit.
 True
 >>> set(world.Q.all_of(relations=[(..., OrbitOf, None)])) == {star, planet}  # Get objects being orbited.
 True
 >>> set(world.Q.all_of(relations=[(LandedOn, ...)])) == {ship, moon_rock, player}
```

### Comparing `tcod_ecs-3.1.0/pyproject.toml` & `tcod_ecs-3.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -110,16 +110,13 @@
     "D",   # pydocstyle
 ]
 ignore = [
     "E501",   # line-too-long
     "S101",   # assert
     "ANN101", # missing-type-self
     "ANN102", # missing-type-cls
-    "D203",   # one-blank-line-before-class
-    "D204",   # one-blank-line-after-class
-    "D213",   # multi-line-summary-second-line
-    "D407",   # dashed-underline-after-section
-    "D408",   # section-underline-after-name
-    "D409",   # section-underline-matches-section-length
 ]
 line-length = 120
-target-version = "py38"
+
+[tool.ruff.pydocstyle]
+# Use Google-style docstrings.
+convention = "google"
```

### Comparing `tcod_ecs-3.1.0/tcod/ecs/__init__.py` & `tcod_ecs-3.2.0/tcod/ecs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,26 +175,36 @@
             [<Entity(uid='other')>]
             >>> list(world.Q.all_of(relations=[(..., str, None)]))
             [<Entity(uid='other')>]
         """
         return EntityComponentRelations(self)
 
     @property
-    def relation_tags(self) -> EntityRelationsExclusive:
+    def relation_tag(self) -> EntityRelationsExclusive:
         """Access an entities exclusive relations.
 
         Example::
 
-            >>> entity.relation_tags["ChildOf"] = other_entity  # Assign relation.
+            >>> entity.relation_tag["ChildOf"] = other_entity  # Assign relation.
             >>> list(world.Q.all_of(relations=[("ChildOf", other_entity)]))  # Get children of other_entity.
             [<Entity(uid='entity')>]
             >>> list(world.Q.all_of(relations=[(entity, "ChildOf", None)]))  # Get parents of entity.
             [<Entity(uid='other')>]
-            >>> del entity.relation_tags["ChildOf"]
+            >>> del entity.relation_tag["ChildOf"]
+        """
+        return EntityRelationsExclusive(self)
+
+    @property
+    def relation_tags(self) -> EntityRelationsExclusive:
+        """Access an entities exclusive relations.
+
+        .. deprecated:: 3.2
+            This attribute was renamed to :any:`relation_tag`.
         """
+        warnings.warn("The '.relation_tags' attribute has been renamed to '.relation_tag'", FutureWarning, stacklevel=2)
         return EntityRelationsExclusive(self)
 
     @property
     def relation_tags_many(self) -> EntityRelations:
         """Access an entities many-to-many relations.
 
         Example::
@@ -524,15 +534,15 @@
         """Return the number of unique relation tags this entity has."""
         return len(self.entity.world._relation_tags_by_entity.get(self.entity, {}))
 
 
 class EntityRelationsExclusive(MutableMapping[object, Entity]):
     """A proxy attribute to access entity relations exclusively.
 
-    See :any:`Entity.relation_tags`.
+    See :any:`Entity.relation_tag`.
     """
 
     __slots__ = ("entity",)
 
     def __init__(self, entity: Entity) -> None:
         """Initialize this attribute for the given entity."""
         self.entity: Final = entity
@@ -893,35 +903,49 @@
         entities = set(requires[0])
         for require in requires[1:]:
             entities.intersection_update(require)
         for exclude in excludes:
             entities.difference_update(exclude)
         return entities
 
+    @staticmethod
+    def __check_suspicious_tags(tags: Iterable[object], stacklevel: int = 2) -> None:
+        if isinstance(tags, str):
+            warnings.warn(
+                "The tags parameter was given a str type."
+                " This will split the string and check its individual letters as tags."
+                "\nAdd square brackets 'tags=[tag]' to check for a single string tag. (Recommended)"
+                "\nOtherwise use 'tags=list(tags)' to suppress this warning.",
+                RuntimeWarning,
+                stacklevel=stacklevel + 1,
+            )
+
     def all_of(
         self,
         components: Iterable[_ComponentKey[object]] = (),
         *,
         tags: Iterable[object] = (),
         relations: Iterable[tuple[object, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None]] = (),
     ) -> Self:
         """Filter entities based on having all of the provided elements."""
+        self.__check_suspicious_tags(tags)
         self._all_of_components.update(components)
         self._all_of_tags.update(tags)
         self._all_of_relations.update(relations)
         return self
 
     def none_of(
         self,
         components: Iterable[_ComponentKey[object]] = (),
         *,
         tags: Iterable[object] = (),
         relations: Iterable[tuple[object, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None]] = (),
     ) -> Self:
         """Filter entities based on having none of the provided elements."""
+        self.__check_suspicious_tags(tags)
         self._none_of_components.update(components)
         self._none_of_tags.update(tags)
         self._none_of_relations.update(relations)
         return self
 
     def __iter__(self) -> Iterator[Entity]:
         """Iterate over the matching entities."""
```

### Comparing `tcod_ecs-3.1.0/PKG-INFO` & `tcod_ecs-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcod-ecs
-Version: 3.1.0
+Version: 3.2.0
 Summary: A type-hinted Entity Component System based on Python dictionaries and sets.
 Author-email: Kyle Benesch <4b796c65+github@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -219,15 +219,15 @@
 True
 
 ```
 
 ## Relations
 
 Use `Entity.relation_components[component_key][target] = component` to associate a relation with data.
-Use `Entity.relation_tags[tag] = target` to associate a tag exclusively with a target entity.
+Use `Entity.relation_tag[tag] = target` to associate a tag exclusively with a target entity.
 Use `Entity.relation_tags_many[tag].add(target)` to associate a tag with multiple targets.
 Tags and relations share the same space then queried, so tags can not be in the format of a component key.
 Relations are unidirectional.
 
 ```py
 >>> @attrs.define
 ... class OrbitOf:  # OrbitOf component.
@@ -237,17 +237,17 @@
 >>> planet = world.new_entity()
 >>> moon = world.new_entity()
 >>> ship = world.new_entity()
 >>> player = world.new_entity()
 >>> moon_rock = world.new_entity()
 >>> planet.relation_components[OrbitOf][star] = OrbitOf(dist=1000)
 >>> moon.relation_components[OrbitOf][planet] = OrbitOf(dist=10)
->>> ship.relation_tags[LandedOn] = moon
->>> moon_rock.relation_tags[LandedOn] = moon
->>> player.relation_tags[LandedOn] = moon_rock
+>>> ship.relation_tag[LandedOn] = moon
+>>> moon_rock.relation_tag[LandedOn] = moon
+>>> player.relation_tag[LandedOn] = moon_rock
 >>> set(world.Q.all_of(relations=[(OrbitOf, planet)])) == {moon}
 True
 >>> set(world.Q.all_of(relations=[(OrbitOf, ...)])) == {planet, moon}  # Get objects in an orbit.
 True
 >>> set(world.Q.all_of(relations=[(..., OrbitOf, None)])) == {star, planet}  # Get objects being orbited.
 True
 >>> set(world.Q.all_of(relations=[(LandedOn, ...)])) == {ship, moon_rock, player}
```

