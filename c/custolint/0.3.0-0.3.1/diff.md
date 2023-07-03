# Comparing `tmp/custolint-0.3.0-py3-none-any.whl.zip` & `tmp/custolint-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 22358 bytes, number of entries: 18
--rw-r--r--  2.0 unx      265 b- defN 23-Jun-19 10:55 custolint/__init__.py
--rw-r--r--  2.0 unx     3342 b- defN 23-Jun-19 10:55 custolint/cli.py
--rw-r--r--  2.0 unx     2485 b- defN 23-Jun-19 10:55 custolint/contributors.py
--rw-r--r--  2.0 unx     4710 b- defN 23-Jun-19 10:55 custolint/coverage.py
--rw-r--r--  2.0 unx     1969 b- defN 23-Jun-19 10:55 custolint/env.py
--rw-r--r--  2.0 unx     1623 b- defN 23-Jun-19 10:55 custolint/flake8.py
--rw-r--r--  2.0 unx     6908 b- defN 23-Jun-19 10:55 custolint/generics.py
--rw-r--r--  2.0 unx     7731 b- defN 23-Jun-19 10:55 custolint/git.py
--rw-r--r--  2.0 unx     1574 b- defN 23-Jun-19 10:55 custolint/log.py
--rw-r--r--  2.0 unx     7039 b- defN 23-Jun-19 10:55 custolint/mypy.py
--rw-r--r--  2.0 unx     4077 b- defN 23-Jun-19 10:55 custolint/pylint.py
--rw-r--r--  2.0 unx     2211 b- defN 23-Jun-19 10:55 custolint/typing.py
--rw-r--r--  2.0 unx     1188 b- defN 23-Jun-19 10:56 custolint-0.3.0.dist-info/LICENSE.rst
--rw-r--r--  2.0 unx     7330 b- defN 23-Jun-19 10:56 custolint-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 10:56 custolint-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Jun-19 10:56 custolint-0.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-19 10:56 custolint-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1406 b- defN 23-Jun-19 10:56 custolint-0.3.0.dist-info/RECORD
-18 files, 54008 bytes uncompressed, 20086 bytes compressed:  62.8%
+Zip file size: 23526 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      265 b- defN 23-Jul-03 09:51 custolint/__init__.py
+-rw-r--r--  2.0 unx     2211 b- defN 23-Jul-03 09:51 custolint/_typing.py
+-rw-r--r--  2.0 unx     5208 b- defN 23-Jul-03 09:51 custolint/cli.py
+-rw-r--r--  2.0 unx     2490 b- defN 23-Jul-03 09:51 custolint/contributors.py
+-rw-r--r--  2.0 unx     5144 b- defN 23-Jul-03 09:51 custolint/coverage.py
+-rw-r--r--  2.0 unx     1979 b- defN 23-Jul-03 09:51 custolint/env.py
+-rw-r--r--  2.0 unx     1899 b- defN 23-Jul-03 09:51 custolint/flake8.py
+-rw-r--r--  2.0 unx     7394 b- defN 23-Jul-03 09:51 custolint/generics.py
+-rw-r--r--  2.0 unx     7747 b- defN 23-Jul-03 09:51 custolint/git.py
+-rw-r--r--  2.0 unx     1574 b- defN 23-Jul-03 09:51 custolint/log.py
+-rw-r--r--  2.0 unx     7313 b- defN 23-Jul-03 09:51 custolint/mypy.py
+-rw-r--r--  2.0 unx     4841 b- defN 23-Jul-03 09:51 custolint/pylint.py
+-rw-r--r--  2.0 unx     1188 b- defN 23-Jul-03 09:52 custolint-0.3.1.dist-info/LICENSE.rst
+-rw-r--r--  2.0 unx     7292 b- defN 23-Jul-03 09:52 custolint-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 09:52 custolint-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Jul-03 09:52 custolint-0.3.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-03 09:52 custolint-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1407 b- defN 23-Jul-03 09:52 custolint-0.3.1.dist-info/RECORD
+18 files, 58102 bytes uncompressed, 21252 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: custolint/__init__.py
 Comment: 
 
+Filename: custolint/_typing.py
+Comment: 
+
 Filename: custolint/cli.py
 Comment: 
 
 Filename: custolint/contributors.py
 Comment: 
 
 Filename: custolint/coverage.py
@@ -27,29 +30,26 @@
 
 Filename: custolint/mypy.py
 Comment: 
 
 Filename: custolint/pylint.py
 Comment: 
 
-Filename: custolint/typing.py
-Comment: 
-
-Filename: custolint-0.3.0.dist-info/LICENSE.rst
+Filename: custolint-0.3.1.dist-info/LICENSE.rst
 Comment: 
 
-Filename: custolint-0.3.0.dist-info/METADATA
+Filename: custolint-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: custolint-0.3.0.dist-info/WHEEL
+Filename: custolint-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: custolint-0.3.0.dist-info/entry_points.txt
+Filename: custolint-0.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: custolint-0.3.0.dist-info/top_level.txt
+Filename: custolint-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: custolint-0.3.0.dist-info/RECORD
+Filename: custolint-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## custolint/cli.py

```diff
@@ -1,16 +1,19 @@
 # pragma: no cover this module will not be covered by the tests,
 # since it is using most of ``click`` external already tested API
 """
 Command line interface API based on python click library
 """
-from typing import Any, Callable
+from typing import Any, Callable, Dict, Tuple
 
 import functools
 import logging
+import sys
+from configparser import ConfigParser
+from pathlib import Path
 
 import click
 
 from . import __version__, coverage, env, flake8, generics, log, mypy, pylint
 from .contributors import Contributors
 
 FuncType = Callable[..., None]
@@ -58,32 +61,93 @@
         LOG.info('---- %s ------', func_name)
         return func(_contributors, halt_on_n_messages, **kwargs)
     return wrapper
 
 
 @common_params
 def _mypy(contributors: Contributors, halt_on_n_messages: int) -> None:
-    generics.filer_output(mypy.compare_with_main_branch(), contributors, halt_on_n_messages)
+    mypy.cli(contributors, halt_on_n_messages)
 
 
 @common_params
 def _pylint(contributors: Contributors, halt_on_n_messages: int) -> None:
-    generics.filer_output(pylint.compare_with_main_branch(), contributors, halt_on_n_messages)
+    pylint.cli(contributors, halt_on_n_messages)
 
 
 @common_params
 def _flake8(contributors: Contributors, halt_on_n_messages: int) -> None:
-    generics.filer_output(flake8.compare_with_main_branch(), contributors, halt_on_n_messages)
+    flake8.cli(contributors, halt_on_n_messages)
 
 
 @click.option('--data-file',
               type=click.Path(exists=True),
               help="Read coverage data for report generation from this file. "
                    "Defaults to '.coverage'. [env: COVERAGE_FILE]")
 @common_params
 def _coverage(contributors: Contributors, halt_on_n_messages: int, data_file: click.Path) -> None:
     file_path = click.format_filename(data_file)  # type: ignore[arg-type]
-    generics.group_by_email_and_file_name(
-        log=coverage.compare_with_main_branch(file_path),
-        contributors=contributors,
-        halt_on_n_messages=halt_on_n_messages
-    )
+    coverage.cli(contributors, halt_on_n_messages, file_path)
+
+
+def _parse_cmd_array(value: str) -> Tuple[str, ...]:
+    """
+    >>> _parse_cmd_array('blue, red,green')
+    ('blue', 'red', 'green')
+    >>> _parse_cmd_array(' ')
+    ()
+    """
+    return tuple(i.strip() for i in value.split(',') if i.strip())
+
+
+def _parse_cmd_kwargs(value: str) -> Dict[str, str]:
+    """
+    >>> _parse_cmd_kwargs('data_file:.coverage,a:b')
+    {'data_file': '.coverage', 'a': 'b'}
+    >>> _parse_cmd_kwargs(',')
+    {}
+    """
+    kwargs = {}
+    for _v in _parse_cmd_array(value):
+        key, value = _v.split(':')
+        kwargs[key.strip()] = value.strip()
+
+    return kwargs
+
+
+@click.argument('config', type=click.Path(exists=True))
+@common_params
+def _from_config(contributors: Contributors, halt_on_n_messages: int, config: click.Path) -> None:
+    config_path = Path(config)  # type: ignore[arg-type]
+    if config_path.name == 'setup.cfg':
+        setup_cfg = ConfigParser()
+        setup_cfg.read(config_path)
+        commands = _parse_cmd_array(setup_cfg['tool:custolint']['commands'])
+        halt = setup_cfg['tool:custolint'].getboolean('halt')
+        LOG.info('The following commands: %r will run with halt=%r', commands, halt)
+
+        _globals = globals()
+
+        halt_error_code = generics.SYSTEM_EXIT_CODE_DRY_AND_CLEAN
+        for cmd in commands:
+            try:
+                cmd_kwargs_raw = setup_cfg['tool:custolint'][cmd + '_kwargs']
+            except KeyError:
+                LOG.warning('no %r command configuration, skip ...', cmd + '_kwargs')
+                continue
+
+            cmd_kwargs = _parse_cmd_kwargs(cmd_kwargs_raw)
+
+            LOG.info('---- from_config:%s ------', cmd)
+
+            return_code = getattr(_globals[cmd], 'cli')(
+                contributors,
+                halt_on_n_messages,
+                halt=halt,
+                **cmd_kwargs,
+            )
+
+            if return_code != generics.SYSTEM_EXIT_CODE_DRY_AND_CLEAN:
+                halt_error_code = return_code
+
+        sys.exit(halt_error_code)
+
+    raise NotImplementedError(config_path.name)
```

## custolint/contributors.py

```diff
@@ -4,15 +4,15 @@
 """
 from typing import Iterable, Tuple
 
 import logging
 
 from pydantic import BaseModel
 
-from custolint import typing
+from custolint import _typing
 
 LOG = logging.getLogger(__name__)
 
 
 class Contributors(BaseModel):
     """
     Contributors API abstraction for CLI and GIT blame
@@ -50,27 +50,27 @@
                 LOG.debug('Skip %r because is in black list contributors %r',
                           clause, self.black)
                 return True
             return False
 
         return False
 
-    def filter_log_line(self, log_lines: Iterable[typing.LogLine]) -> Iterable[typing.LogLine]:
+    def filter_log_line(self, log_lines: Iterable[_typing.LogLine]) -> Iterable[_typing.LogLine]:
         """
         Include or exclude contributors from lint log line
         """
         for line in log_lines:
             if callable(line):
                 yield line
                 continue
 
             if not self._filter(line.email, line.author):
                 yield line
 
-    def filter_coverage(self, coverages: Iterable[typing.Coverage]) -> Iterable[typing.Coverage]:
+    def filter_coverage(self, coverages: Iterable[_typing.Coverage]) -> Iterable[_typing.Coverage]:
         """
         Include or exclude contributors from coverage report
         """
         for coverage in coverages:
             if not self._filter(
                 coverage.contributor['email'],
                 coverage.contributor['author']
```

## custolint/coverage.py

```diff
@@ -40,23 +40,24 @@
 
 import logging
 import sys
 from pathlib import Path
 
 import bash
 
-from . import env, git, typing
+from . import _typing, env, generics, git
+from .contributors import Contributors
 
 LOG = logging.getLogger(__name__)
 
 
 def _process_missing_lines(
         file_name: str,
         missing: str,
-        changes: typing.Changes) -> Iterator[typing.Coverage]:
+        changes: _typing.Changes) -> Iterator[_typing.Coverage]:
 
     if "-" in missing:
         # The condition was nether false or nether true, we will just point to the first line
         if missing.endswith("->exit"):  # alike '8->exit'
             start = end = missing.split("->exit")[0]
         elif ">" in missing:  # alike '58->56'
             start = end = missing.split("->")[0]
@@ -67,22 +68,22 @@
 
     start_end = list(range(int(start), int(end) + 1))
     del start, end
 
     for line_number in start_end:
         contributor = changes.get(file_name, {}).get(int(line_number))
         if contributor:
-            yield typing.Coverage(
+            yield _typing.Coverage(
                 contributor=contributor,
                 file_name=file_name,
                 line_number=line_number
             )
 
 
-def compare_with_main_branch(coverage_file_location: str) -> Iterator[typing.Coverage]:
+def compare_with_main_branch(coverage_file_location: str) -> Iterator[_typing.Coverage]:
     """
     Apply coverage check on the changes only
     """
     changes = git.changes()
     config = Path(env.CONFIG_D, '.coveragerc')
     config_argument = f"--rcfile={config}" if config.exists() else "--show-missing"
     execute_command = " ".join((
@@ -141,7 +142,20 @@
             for missing in missing_coverage_lines:
                 for line in _process_missing_lines(
                     file_name=fields[0],
                     missing=missing,
                     changes=changes
                 ):
                     yield line
+
+
+def cli(contributors: Contributors,
+        halt_on_n_messages: int,
+        data_file: str,
+        halt: bool = True) -> int:
+    """Provide interface for coverage CLI"""
+    return generics.group_by_email_and_file_name(
+        log=compare_with_main_branch(data_file),
+        contributors=contributors,
+        halt_on_n_messages=halt_on_n_messages,
+        halt=halt
+    )
```

## custolint/env.py

```diff
@@ -26,15 +26,15 @@
 
     $ MAIN_BRANCH=JIRA-14407-core2-merge custolint mypy
     INFO:custolint.git:Compare current branch with 'main' branch
     INFO:custolint.git:Execute git diff command 'git diff origin/JIRA-14407-core2-merge -U0 --diff-filter=ACMRTUXB'
     INFO:custolint.git:Git diff detected 28 filed affected
     INFO:custolint.generics:Execute lint commands 'flake8 --config=config.d/.flake8 {lint_file}' for 18 files ...
 
-    # The main branch is autodetected with ``git remote show origin`` command
+    # The main branch is automatically detected with ``git remote show origin`` command
     $ custolint flake8
     INFO:custolint.git:Compare current branch with 'main' branch
     INFO:custolint.git:Execute git diff command 'git diff origin/main -U0 --diff-filter=ACMRTUXB'
     INFO:custolint.git:Git diff detected 28 filed affected
 
 Config.d
 --------
```

## custolint/flake8.py

```diff
@@ -29,31 +29,37 @@
     file16.py: message
 
 """
 from typing import Dict, Iterator, Sequence, Union
 
 from pathlib import Path
 
-from . import env, generics, typing
+from . import _typing, env, generics
+from .contributors import Contributors
 
 
 # pylint: disable=unused-argument
 def _filter(path: Path, message: str, line_number: int, cache: Dict[Path, Sequence[str]]) -> bool:
     """
     Return True if we want to skip the check else False if we want this check
     """
     return False
 # pylint: enable=unused-argument
 
 
-def compare_with_main_branch() -> Iterator[Union[typing.Lint, typing.FiltersType]]:
+def compare_with_main_branch() -> Iterator[Union[_typing.Lint, _typing.FiltersType]]:
     """
     Compare all flake8 messages against code different to target branch.
     """
     config = Path(env.CONFIG_D, '.flake8')
     config_argument = f"--config={config}" if config.exists() else ""
     command = " ".join(("flake8", config_argument, "{lint_file}"))
 
     return generics.lint_compare_with_main_branch(
         execute_command=command,
         filters=(_filter,)
     )
+
+
+def cli(contributors: Contributors, halt_on_n_messages: int, halt: bool = True) -> int:
+    """Provide interface for flake8 CLI"""
+    return generics.filer_output(compare_with_main_branch(), contributors, halt_on_n_messages, halt)
```

## custolint/generics.py

```diff
@@ -8,18 +8,19 @@
 import logging
 import re
 import sys
 from pathlib import Path
 
 import bash
 
-from . import git, typing
+from . import _typing, git
 from .contributors import Contributors
 
 LOG = logging.getLogger(__name__)
+SYSTEM_EXIT_CODE_DRY_AND_CLEAN = 0
 SYSTEM_EXIT_CODE_WITH_ALL_MESSAGES_INCLUDED = 41
 SYSTEM_EXIT_CODE_WITH_HALT_ON_N_MESSAGES = 42
 
 
 TEST_FILES_REGEX = re.compile(r"(^|/)(test_.*|conftest)\.py")
 
 
@@ -57,40 +58,41 @@
         message = match.group(3)
         return file_name, line_number, message
 
     # unexpected not parsable lines
     raise RuntimeError(f"Can not parse lint line {stdout_line!r}")
 
 
-def _process_line(fields: Tuple[str, int, str], changes: typing.Changes) -> Optional[typing.Lint]:
+def _process_line(fields: Tuple[str, int, str], changes: _typing.Changes) -> Optional[_typing.Lint]:
     """
     Process a single line message from PyLint or Flake8 report
     """
     file_name = fields[0]
     line_number = fields[1]
     message = fields[2]
 
     contributor = changes.get(file_name, {}).get(line_number)
 
     if contributor:
-        return typing.Lint(
+        return _typing.Lint(
             file_name=file_name,
             line_number=line_number,
             message=message,
             email=contributor['email'],
             date=contributor['date'],
             author=contributor['author']
         )
 
     return None
 
 
 def lint_compare_with_main_branch(
         execute_command: str,
-        filters: Iterable[typing.FiltersType]) -> Iterator[Union[typing.Lint, typing.FiltersType]]:
+        filters: Iterable[_typing.FiltersType]
+) -> Iterator[Union[_typing.Lint, _typing.FiltersType]]:
     """
     A common API for pylint and flake8
     """
     # pylint: disable=too-many-locals
     changes = git.changes()
 
     includes = re.compile(r'.py$')
@@ -135,15 +137,15 @@
             similar_line = None
 
         results = _process_line(fields, changes)
         if results:
             yield results
 
 
-def _output_grouping_by_email_and_file_name(chunk: Iterable[typing.Coverage]) -> None:
+def _output_grouping_by_email_and_file_name(chunk: Iterable[_typing.Coverage]) -> None:
     """
     Output grouping items email and file name
     """
     iterator = iter(chunk)
     head = next(iterator)
     file_name = head[1]
     email = head[0]['email']
@@ -159,18 +161,19 @@
         start_line, end_line = head[2], last[2]
         line_number = f"{start_line}-{end_line}"
 
     output("%s:%s %05s %s", file_name, line_number, email, date)
 
 
 def group_by_email_and_file_name(
-    log: Iterable[typing.Coverage],
+    log: Iterable[_typing.Coverage],
     contributors: Contributors,
-    halt_on_n_messages: int
-) -> None:
+    halt_on_n_messages: int,
+    halt: bool = True
+) -> int:
     """
     Group by email and file name, used for coverage.
     """
     found_count = 0
     previous_email = None
     previous_file_name = None
     previous_line_number = None
@@ -195,38 +198,45 @@
         previous_line_number = line_number
         previous_file_name = file_name
 
         found_count += 1
 
         if halt_on_n_messages and found_count == halt_on_n_messages:
             _output_grouping_by_email_and_file_name(chunk)
-            sys.exit(SYSTEM_EXIT_CODE_WITH_HALT_ON_N_MESSAGES)
+            if halt:
+                sys.exit(SYSTEM_EXIT_CODE_WITH_HALT_ON_N_MESSAGES)
+            return SYSTEM_EXIT_CODE_WITH_HALT_ON_N_MESSAGES
 
     if chunk:
         _output_grouping_by_email_and_file_name(chunk)
 
     if not found_count:
         output("::Dry and Clean::")
-    else:
+        return SYSTEM_EXIT_CODE_DRY_AND_CLEAN
+
+    if halt:
         sys.exit(SYSTEM_EXIT_CODE_WITH_ALL_MESSAGES_INCLUDED)
 
+    return SYSTEM_EXIT_CODE_WITH_ALL_MESSAGES_INCLUDED
+
 
-def filer_output(log: Iterable[typing.LogLine],
+def filer_output(log: Iterable[_typing.LogLine],
                  contributors: Contributors,
-                 halt_on_n_messages: int) -> None:
+                 halt_on_n_messages: int,
+                 halt: bool = True) -> int:
     """
     Filter output by:
     - date range
     - include contributor
     - exclude contributor
     """
     cache: Dict[Path, Sequence[str]] = {}
 
     # get filters from env, configuration and cli
-    filters_chain: List[typing.FiltersType] = []
+    filters_chain: List[_typing.FiltersType] = []
 
     found_count = 0
 
     for line in contributors.filter_log_line(log):
 
         if callable(line):
             filters_chain.append(line)
@@ -242,13 +252,19 @@
 
         output('%s:%d %s ## %s:%s',
                line.file_name, line.line_number, line.message, line.email, line.date)
 
         found_count += 1
 
         if halt_on_n_messages and found_count == halt_on_n_messages:
-            sys.exit(SYSTEM_EXIT_CODE_WITH_HALT_ON_N_MESSAGES)
+            if halt:
+                sys.exit(SYSTEM_EXIT_CODE_WITH_HALT_ON_N_MESSAGES)
+            return SYSTEM_EXIT_CODE_WITH_HALT_ON_N_MESSAGES
 
     if not found_count:
         output("::Dry and Clean::")
-    else:
+        return SYSTEM_EXIT_CODE_DRY_AND_CLEAN
+
+    if halt:
         sys.exit(SYSTEM_EXIT_CODE_WITH_ALL_MESSAGES_INCLUDED)
+
+    return SYSTEM_EXIT_CODE_WITH_ALL_MESSAGES_INCLUDED
```

## custolint/git.py

```diff
@@ -7,15 +7,15 @@
 import logging
 import re
 import sys
 from collections import defaultdict
 
 import bash
 
-from . import env, typing
+from . import _typing, env
 
 LOG = logging.getLogger(__name__)
 MINIMUM_GIT_RECOMMEND_VERSION = (2, 39, 2)
 
 
 def _autodetect_main_branch() -> str:
     """
@@ -37,30 +37,30 @@
         logging.error('Could not find default/main branch: %r', command.stderr.decode())
         sys.exit(command.code)
 
     stdout: str = command.stdout.decode()
     return re.search(r"HEAD branch: (.+)", stdout).group(1)  # type: ignore[union-attr]
 
 
-def _split_as_blame_porcelain(output: str) -> Iterator[typing.Blame]:
+def _split_as_blame_porcelain(output: str) -> Iterator[_typing.Blame]:
     buffer: List[str] = []
 
     # 005661f440bcdfefb2fd41d4e781351471dfb3ef 26 33 1
     head_re = re.compile(r'^[0-9a-f]{40} \d+ \d+')
     for line in output.splitlines():
         if buffer and head_re.search(line):
-            yield typing.Blame.from_porcelain(tuple(buffer))
+            yield _typing.Blame.from_porcelain(tuple(buffer))
             buffer.clear()
 
         buffer.append(line)
 
-    yield typing.Blame.from_porcelain(tuple(buffer))
+    yield _typing.Blame.from_porcelain(tuple(buffer))
 
 
-def _blame(the_line_number: str, file_name: str) -> Iterator[typing.Blame]:
+def _blame(the_line_number: str, file_name: str) -> Iterator[_typing.Blame]:
     """
     Parse blame log to extract: author email, author name, date and  file_name
 
     > git blame --line-porcelain -L 33,+1 --show-email --show-name -- setup.cfg
     005661f440bcdfefb2fd41d4e781351471dfb3ef 26 33 1
     author John Snow
     author-mail <John.Snow@John.Snow.tld>
@@ -94,15 +94,15 @@
         sys.exit(command.code)
 
     stdout = command.stdout.decode().strip()
 
     return _split_as_blame_porcelain(stdout)
 
 
-def _process_diff_line(diff_line: str, file_name: str) -> Union[str, None, Iterator[typing.Blame]]:
+def _process_diff_line(diff_line: str, file_name: str) -> Union[str, None, Iterator[_typing.Blame]]:
     # line like +++ b/care/share/calc/_methods2.py
     if diff_line.startswith("+++ "):
         _, file_name = diff_line.split("+++ ", maxsplit=1)
         return file_name[2:]
 
     # line like @@ -0,0 +1,146 @@
     if not diff_line.startswith("@@"):
@@ -143,15 +143,15 @@
     if command.code:
         logging.error('Could not find git version name: %s', command.stderr.decode())
         sys.exit(command.code)
 
     stdout = command.stdout.decode()
     versions = tuple(int(version) for version in stdout.split()[2].split('.'))
     if versions < MINIMUM_GIT_RECOMMEND_VERSION:
-        LOG.warning('Be aware that current git version %r is less than recomended %r',
+        LOG.warning('Be aware that current git version %r is less than recommended %r',
                     versions, MINIMUM_GIT_RECOMMEND_VERSION)
 
     return versions
 
 
 def _pull_rebase(main_branch: str, current_branch_name: str) -> None:
     """
@@ -181,28 +181,28 @@
         _check_git_version()
         current_branch_name = _current_branch_name()
         _pull_rebase(main_branch, current_branch_name)
 
     return current_branch_name
 
 
-def changes(do_pull_rebase: bool = True) -> typing.Changes:
+def changes(do_pull_rebase: bool = True) -> _typing.Changes:
     """
     Get diff changes of current branch against master branch and
     return a mapping of affected filename and line numbers
     """
     main_branch = _autodetect_main_branch()
     LOG.info("Compare current branch with %r branch", main_branch)
 
-    files: typing.Changes = defaultdict(dict)
+    files: _typing.Changes = defaultdict(dict)
 
     _git_sync(do_pull_rebase, main_branch)
 
     the_file = ""
-    execute_command = f"git diff origin/{main_branch} -U0 --diff-filter=ACMRTUXB"  # noqa: spelling
+    execute_command = f"git diff origin/{main_branch} -U0 --diff-filter=ACMRTUXB"
     LOG.info("Execute git diff command %r", execute_command)
     command = bash.bash(execute_command)
 
     if command.code:
         logging.error('Diff command failed: %s', command.stderr.decode())
         sys.exit(command.code)
 
@@ -216,16 +216,16 @@
         if not result:
             continue
 
         if isinstance(result, str):
             the_file = result
             continue
 
-        if isinstance(result, Iterable):  # pragma: no cover
-            typed_result = cast(Iterable[typing.Blame], result)
+        if isinstance(result, Iterable):  # pragma: no cover why is not cover : TODO
+            typed_result = cast(Iterable[_typing.Blame], result)
             for blame in typed_result:
                 change = files[blame.file_name]
 
                 change[blame.line_number] = {
                     'author': blame.author,
                     'email': blame.email,
                     'date': blame.date
```

## custolint/mypy.py

```diff
@@ -46,33 +46,34 @@
 import sys
 import tempfile
 from pathlib import Path
 
 import bash
 from mypy import errorcodes
 
-from . import env, generics, git, typing
+from . import _typing, env, generics, git
+from .contributors import Contributors
 
 LOG = logging.getLogger(__name__)
 
 
-def _process_line(fields: Sequence[str], changes: typing.Changes) -> Optional[typing.Lint]:
+def _process_line(fields: Sequence[str], changes: _typing.Changes) -> Optional[_typing.Lint]:
     """
     Process a single line message from MyPy report
     """
     if len(fields) == 4:
 
         file_name = fields[0]
         line_number = int(fields[1])
         message: str = fields[-1]
 
         contributor = changes.get(file_name, {}).get(line_number)
         if contributor:
 
-            return typing.Lint(
+            return _typing.Lint(
                 author='John Snow',
                 file_name=file_name,
                 line_number=int(line_number),
                 message=message.strip(),
                 email=contributor['email'],
                 date=contributor['date']
             )
@@ -128,15 +129,15 @@
     # test_b.py:78 Module has no attribute "git" [attr-defined]
     if all((
             f" [{errorcodes.ATTR_DEFINED.code}]" in message,
             mocking_line.search(line_content),
     )):
         return True
 
-    # if the line is split check previous lineform
+    # if the line is split check previous line
     if previous_line_content and all((
             f" [{errorcodes.ATTR_DEFINED.code}]" in message,
             mocking_line.search(previous_line_content),
     )):
         return True
 
     # It is normal practice to patch private api in tests
@@ -190,16 +191,16 @@
 
 
 def _parse_message_line(message: str) -> Sequence[str]:
     return message.split(":", 3)  # filepath, line number, level, message
 
 
 def compare_with_main_branch(
-        filters: Iterable[typing.FiltersType] = (_filter,)
-) -> Iterator[Union[typing.Lint, typing.FiltersType]]:
+        filters: Iterable[_typing.FiltersType] = (_filter,)
+) -> Iterator[Union[_typing.Lint, _typing.FiltersType]]:
     """
     Compare mypy output against target branch
     """
     # pylint: disable=too-many-locals
 
     changes = git.changes()
 
@@ -239,7 +240,12 @@
 
     for mypy_line in stdout.split("\n"):
         fields = _parse_message_line(mypy_line)
 
         results = _process_line(fields, changes)
         if results:
             yield results
+
+
+def cli(contributors: Contributors, halt_on_n_messages: int, halt: bool = True) -> int:
+    """Provide interface for mypy CLI"""
+    return generics.filer_output(compare_with_main_branch(), contributors, halt_on_n_messages, halt)
```

## custolint/pylint.py

```diff
@@ -30,15 +30,16 @@
 
 """
 from typing import Dict, Iterable, Iterator, Optional, Sequence, Union
 
 import re
 from pathlib import Path
 
-from . import env, generics, typing
+from . import _typing, env, generics
+from .contributors import Contributors
 
 
 def _filter_test_function(message: str, line_content: str) -> bool:  # pylint: disable=too-many-return-statements
     # :check-description: test methods does not require to provide docstring
     if "def test_" in line_content:
         if '(missing-function-docstring)' in message:
             return True
@@ -91,14 +92,27 @@
     # ignore all TODO marked with Jira reference
     if re.search(r"TODO: [A-Z]{3,}-\d+: ", message, re.IGNORECASE):
         return True
 
     return False
 
 
+def _filter_pydantic(message: str,
+                     previous_line_content: Optional[str]) -> bool:
+
+    # :check-description: if validator of pydantic then cls is ok
+    if all(
+            ('@validator(' in (previous_line_content or ''),
+             ' should have "self" as first argument (no-self-argument)' in message
+             )):
+        return True
+
+    return False
+
+
 def _filter(path: Path, message: str, line_number: int, cache: Dict[Path, Sequence[str]]) -> bool:
     """
     Return True if we want to skip the check else False if we want this check
     """
     # pylint: disable=too-many-return-statements
 
     if path not in cache:
@@ -110,24 +124,33 @@
     previous_line_content = content[line_number - 2] if line_number - 2 >= 0 else None
 
     if generics.TEST_FILES_REGEX.search(path.name):
         do_filter = _filter_test_function(message, line_content)
         if do_filter:
             return True
 
+    do_filter = _filter_pydantic(message, previous_line_content)
+    if do_filter:
+        return True
+
     return _filter_all_function(message, line_content, previous_line_content)
 
 
 def compare_with_main_branch(
-        filters: Iterable[typing.FiltersType] = (_filter, )
-) -> Iterator[Union[typing.Lint, typing.FiltersType]]:
+        filters: Iterable[_typing.FiltersType] = (_filter, )
+) -> Iterator[Union[_typing.Lint, _typing.FiltersType]]:
     """
     Compare all pylint messages against code different to target branch.
     """
     config = Path(env.CONFIG_D, 'pylintrc')
     config_argument = f"--rcfile={config}" if config.exists() else ""
     command = " ".join(("pylint", config_argument, "{lint_file}"))
 
     return generics.lint_compare_with_main_branch(
         execute_command=command,
         filters=filters
     )
+
+
+def cli(contributors: Contributors, halt_on_n_messages: int, halt: bool = True) -> int:
+    """Provide interface for pylint CLI"""
+    return generics.filer_output(compare_with_main_branch(), contributors, halt_on_n_messages, halt)
```

## Comparing `custolint/typing.py` & `custolint/_typing.py`

 * *Files identical despite different names*

## Comparing `custolint-0.3.0.dist-info/LICENSE.rst` & `custolint-0.3.1.dist-info/LICENSE.rst`

 * *Files identical despite different names*

## Comparing `custolint-0.3.0.dist-info/METADATA` & `custolint-0.3.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custolint
-Version: 0.3.0
+Version: 0.3.1
 Summary: Another custom linter layer
 License: MIT License
 Keywords: static code analysis,linter,python,lint,coverage,flake8
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -147,16 +147,15 @@
 
     cd custolint
 
     # prod
     $ make update_pip_and_wheel install
 
     # dev
-    $ make update_pip_and_wheel install
-    make update_pip_and_wheel install_dev
+    $ make update_pip_and_wheel install_dev
 
 
 How to run:
 -----------
 
 .. code-block::
```

## Comparing `custolint-0.3.0.dist-info/RECORD` & `custolint-0.3.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 custolint/__init__.py,sha256=9fc02KmLjgUd-xehhx946V28Vm1YAquYOyOhAD6Ogao,265
-custolint/cli.py,sha256=UC1YSM-PI152d2kvLzWoO1llh18DFKYH00UImOApwRM,3342
-custolint/contributors.py,sha256=dQTqymH66xhao7JjpVlsicK2YXfvWqQGAyNq8GRfQIo,2485
-custolint/coverage.py,sha256=Qnknxlu6CsrSBQVnw1M4-xD4USrKP4NIByehggY-JKw,4710
-custolint/env.py,sha256=4oi9sh5m1t1VSV2sqprGHn7ltRBqmJ4jFi31c0-GTJA,1969
-custolint/flake8.py,sha256=S9D4-uCpT40D4av39Gy-IL5O1BtYEojIkIN6ZrODxLU,1623
-custolint/generics.py,sha256=oN3LUS_oHr3FXrNO5QJVjP0yKzk44GFoeUxm48ud_m8,6908
-custolint/git.py,sha256=--rWMVyO0HDOuVoptf8vdZucLJCPvfX9-ma9Emd882M,7731
+custolint/_typing.py,sha256=PPxAtzh29Gsid4qw27_pNA6EoyDcEKKI8ezQFmd3E1w,2211
+custolint/cli.py,sha256=iawjCafsrWDfdUqhKru9B5V3WmDuL9-nDldKNNgGQpM,5208
+custolint/contributors.py,sha256=WcPnlY7E6jKlKh5mVW2jPkwPOzewrj_wjJrPMOAo5OU,2490
+custolint/coverage.py,sha256=sHv-DdpjphiqNBEmoON5NofM3z8d27Vnz0mII6MPIqY,5144
+custolint/env.py,sha256=sO0MLnXOshsKDGPO8b0kXT6FQsstdsHJooe4RG_JwTw,1979
+custolint/flake8.py,sha256=V_j4SYYhIsF1Y6WlbqJi2aUTwQkr8o28UgYs21WwCpk,1899
+custolint/generics.py,sha256=QxBo0UMieELDDC4PsEFB8Z6dgxpVQo6JAygZFgL9lKE,7394
+custolint/git.py,sha256=QcT7OGUpvBE4t990rJkCqK4_4zphuH8gz7K-yeozAPs,7747
 custolint/log.py,sha256=XxH5Klvwg8G8IYIt5Bd4Pr7aMbTCJcmFf-ls0DRP_RU,1574
-custolint/mypy.py,sha256=WBGafYSUzVDSk7qZ1j4mmkn-VATA4DUcnFEEnbR7m_I,7039
-custolint/pylint.py,sha256=Na2Yv40XEOHfuHrW8ZwJL9gj_O4VfUtBIbivp3rx4rg,4077
-custolint/typing.py,sha256=PPxAtzh29Gsid4qw27_pNA6EoyDcEKKI8ezQFmd3E1w,2211
-custolint-0.3.0.dist-info/LICENSE.rst,sha256=UswXytJM35MbBxnOiTSMqpnu85GOLUxRe6hvN41IEUI,1188
-custolint-0.3.0.dist-info/METADATA,sha256=GcR4xO7gga9wJuINBXEHkTjN8YIoYnsEAR_kH7VwR34,7330
-custolint-0.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-custolint-0.3.0.dist-info/entry_points.txt,sha256=FXto-Crn9co-sUFEXZumypVJpoDeWKvSJQgErDlQmao,48
-custolint-0.3.0.dist-info/top_level.txt,sha256=jVr0mMMpbEHcSe4AFaZfyfD3jXO6YAkM_kEsQ1LIWoc,10
-custolint-0.3.0.dist-info/RECORD,,
+custolint/mypy.py,sha256=s1b9rNKMPJzRSGJTkYoTmwdSkvqtttmrkgqKIXwOamE,7313
+custolint/pylint.py,sha256=GrY-5oRvqoT2K68UdrCbGMQR9Ld0gAHd-6Tao0Hz84I,4841
+custolint-0.3.1.dist-info/LICENSE.rst,sha256=UswXytJM35MbBxnOiTSMqpnu85GOLUxRe6hvN41IEUI,1188
+custolint-0.3.1.dist-info/METADATA,sha256=fJYwEX__cFGndCuckzc6O_7FDIZi922s7-9Gqjv2k3s,7292
+custolint-0.3.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+custolint-0.3.1.dist-info/entry_points.txt,sha256=FXto-Crn9co-sUFEXZumypVJpoDeWKvSJQgErDlQmao,48
+custolint-0.3.1.dist-info/top_level.txt,sha256=jVr0mMMpbEHcSe4AFaZfyfD3jXO6YAkM_kEsQ1LIWoc,10
+custolint-0.3.1.dist-info/RECORD,,
```

