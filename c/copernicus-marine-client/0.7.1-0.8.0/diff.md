# Comparing `tmp/copernicus_marine_client-0.7.1.tar.gz` & `tmp/copernicus_marine_client-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copernicus_marine_client-0.7.1.tar", max compression
+gzip compressed data, was "copernicus_marine_client-0.8.0.tar", max compression
```

## Comparing `copernicus_marine_client-0.7.1.tar` & `copernicus_marine_client-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     3142 2023-05-12 06:57:25.897183 copernicus_marine_client-0.7.1/copernicus_marine_client/__init__.py
--rw-r--r--   0        0        0       13 2023-02-28 10:55:38.193838 copernicus_marine_client-0.7.1/copernicus_marine_client/catalogue_parser/__init__.py
--rw-r--r--   0        0        0    22578 2023-05-12 06:57:25.899181 copernicus_marine_client-0.7.1/copernicus_marine_client/catalogue_parser/catalogue_parser.py
--rw-r--r--   0        0        0     6275 2023-05-12 06:57:25.901181 copernicus_marine_client-0.7.1/copernicus_marine_client/catalogue_parser/request_structure.py
--rw-r--r--   0        0        0       13 2023-03-27 15:21:46.450744 copernicus_marine_client-0.7.1/copernicus_marine_client/command_line_interface/__init__.py
--rw-r--r--   0        0        0      514 2023-04-04 08:48:14.516284 copernicus_marine_client-0.7.1/copernicus_marine_client/command_line_interface/copernicus_marine.py
--rw-r--r--   0        0        0     3282 2023-05-04 11:59:08.729763 copernicus_marine_client-0.7.1/copernicus_marine_client/command_line_interface/group_describe.py
--rw-r--r--   0        0        0     6727 2023-05-12 06:57:25.903183 copernicus_marine_client-0.7.1/copernicus_marine_client/command_line_interface/group_native.py
--rw-r--r--   0        0        0    15676 2023-05-12 06:57:25.906185 copernicus_marine_client-0.7.1/copernicus_marine_client/command_line_interface/group_subset.py
--rw-r--r--   0        0        0     7691 2023-05-10 15:49:41.108051 copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_ftp.py
--rw-r--r--   0        0        0     3856 2023-05-12 06:57:25.908292 copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_motu.py
--rw-r--r--   0        0        0    10327 2023-05-12 06:57:25.911185 copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_opendap.py
--rw-r--r--   0        0        0     7365 2023-05-25 07:55:34.881556 copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_s3native.py
--rw-r--r--   0        0        0     6419 2023-05-12 06:57:25.913182 copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_zarr.py
--rwxr-xr-x   0        0        0 16950784 2022-07-05 02:58:00.000000 copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/s5cmd.exe
--rw-r--r--   0        0        0      887 2023-05-25 13:42:10.141400 copernicus_marine_client-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    14302 2023-05-12 06:57:25.895201 copernicus_marine_client-0.7.1/README.md
--rw-r--r--   0        0        0    15574 1970-01-01 00:00:00.000000 copernicus_marine_client-0.7.1/setup.py
--rw-r--r--   0        0        0    14857 1970-01-01 00:00:00.000000 copernicus_marine_client-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    16970 2023-07-03 09:04:50.547368 copernicus_marine_client-0.8.0/README.md
+-rw-r--r--   0        0        0     3074 2023-07-03 07:22:16.275799 copernicus_marine_client-0.8.0/copernicus_marine_client/__init__.py
+-rw-r--r--   0        0        0       10 2023-06-29 09:51:23.544268 copernicus_marine_client-0.8.0/copernicus_marine_client/catalogue_parser/__init__.py
+-rw-r--r--   0        0        0    22216 2023-06-30 15:09:13.269129 copernicus_marine_client-0.8.0/copernicus_marine_client/catalogue_parser/catalogue_parser.py
+-rw-r--r--   0        0        0     6167 2023-07-03 09:04:50.547514 copernicus_marine_client-0.8.0/copernicus_marine_client/catalogue_parser/request_structure.py
+-rw-r--r--   0        0        0       10 2023-06-29 09:51:23.544602 copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/__init__.py
+-rw-r--r--   0        0        0      858 2023-07-03 09:04:50.547623 copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/copernicus_marine.py
+-rw-r--r--   0        0        0     3707 2023-07-03 09:04:50.547754 copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/group_describe.py
+-rw-r--r--   0        0        0     4424 2023-07-03 09:04:50.547827 copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/group_login.py
+-rw-r--r--   0        0        0     8886 2023-07-03 09:04:50.548072 copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/group_native.py
+-rw-r--r--   0        0        0    18276 2023-07-03 09:04:50.548396 copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/group_subset.py
+-rw-r--r--   0        0        0     4798 2023-07-03 09:04:50.548576 copernicus_marine_client-0.8.0/copernicus_marine_client/configuration_files_creator.py
+-rw-r--r--   0        0        0     7524 2023-07-03 09:04:50.548740 copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_ftp.py
+-rw-r--r--   0        0        0     4542 2023-07-03 09:04:50.548845 copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_motu.py
+-rw-r--r--   0        0        0    10512 2023-07-03 09:04:50.548971 copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_opendap.py
+-rw-r--r--   0        0        0     6304 2023-07-03 09:04:50.549080 copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_s3native.py
+-rw-r--r--   0        0        0     6453 2023-07-03 09:04:50.549222 copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_zarr.py
+-rw-r--r--   0        0        0      917 2023-06-29 09:51:23.593091 copernicus_marine_client-0.8.0/copernicus_marine_client/logging_conf.json
+-rw-r--r--   0        0        0      870 2023-07-03 09:13:25.036758 copernicus_marine_client-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    18710 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.0/setup.py
+-rw-r--r--   0        0        0    17909 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.0/PKG-INFO
```

### Comparing `copernicus_marine_client-0.7.1/copernicus_marine_client/catalogue_parser/catalogue_parser.py` & `copernicus_marine_client-0.8.0/copernicus_marine_client/catalogue_parser/catalogue_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,710 +1,724 @@
-from copy import deepcopy
-from dataclasses import dataclass
-from datetime import timedelta
-from itertools import groupby
-from json import loads
-from multiprocessing import Pool
-from typing import Any, Callable, Iterable, Optional, Tuple, TypeVar, Union
-
-import requests
-from cachier import cachier
-from pystac import Asset, Catalog, Collection, Item, Link, STACError
-from tqdm import tqdm
-
-
-@dataclass
-class CopernicusMarineDatasetService:
-    protocol: str
-    uri: str
-
-
-@dataclass
-class CopernicusMarineDatasetCoordinates:
-    coordinates_id: str
-    units: str
-    minimum_value: float
-    maximum_value: float
-    step: Optional[float]
-    values: Optional[str]
-
-
-@dataclass
-class CopernicusMarineDatasetVariable:
-    short_name: str
-    standard_name: str
-    units: str
-    bbox: Tuple[float, float, float, float]
-    coordinates: list[CopernicusMarineDatasetCoordinates]
-
-
-@dataclass
-class CopernicusMarineProductDataset:
-    dataset_id: str
-    dataset_name: str
-    services: list[CopernicusMarineDatasetService]
-    variables: list[CopernicusMarineDatasetVariable]
-
-
-@dataclass
-class CopernicusMarineProductProvider:
-    name: str
-    roles: list[str]
-    url: str
-    email: str
-
-
-@dataclass
-class CopernicusMarineProduct:
-    title: str
-    product_id: str
-    thumbnail_url: str
-    description: str
-    production_center: str
-    creation_datetime: str
-    modified_datetime: Optional[str]
-    keywords: dict[str, str]
-    datasets: list[CopernicusMarineProductDataset]
-
-
-@dataclass
-class CopernicusMarineCatalogue:
-    products: list[CopernicusMarineProduct]
-
-    def filter(self, tokens: list[str]):
-        return filter_catalogue_with_strings(self, tokens)
-
-
-OPENDAP_KEY = "opendap"
-MOTU_KEY = "motu"
-FTP_KEY = "ftp"
-GEOCHUNKED_KEY = "geoChunked"
-TIMECHUNKED_KEY = "timeChunked"
-S3NATIVE_KEY = "native"
-DOWNSAMPLED4_KEY = "downsampled4"
-
-_S = TypeVar("_S")
-_T = TypeVar("_T")
-
-
-def map_parallel(
-    function: Callable[[_S], _T], iterable: Iterable[_S]
-) -> list[_T]:
-    parallel_processes = 20
-    with Pool(parallel_processes) as pool:
-        return pool.map(function, iterable)
-
-
-def map_reject_none(
-    function: Callable[[_S], Optional[_T]], iterable: Iterable[_S]
-) -> Iterable[_T]:
-    return (element for element in map(function, iterable) if element)
-
-
-def parse_catalogue(
-    overwrite_cache: bool = False,
-) -> CopernicusMarineCatalogue:
-    return merge_catalogues(
-        parse_dissemination_unit_catalogue(overwrite_cache=overwrite_cache),
-        parse_marine_data_store_catalogue(overwrite_cache=overwrite_cache),
-    )
-
-
-# --------------------------------------------------------
-# --- Function specific for cmems-be.lobelia catalogue ---
-# --------------------------------------------------------
-@cachier(stale_after=timedelta(hours=3))
-def _fetch_raw_products() -> list[dict[str, Any]]:
-    response = requests.post(
-        "https://cmems-be.lobelia.earth/api/datasets",
-        json={"size": 1000, "includeOmis": True},
-    )
-    assert response.ok, response.text
-    raw_catalogue: dict[str, Any] = loads(response.text)
-    return map_parallel(
-        _fetch_raw_product,
-        tqdm(
-            raw_catalogue["datasets"].keys(),
-            desc="Fetching dissemination unit raw products",
-        ),
-    )
-
-
-def _fetch_raw_product(product_id: str) -> dict[str, Any]:
-    response = requests.get(product_url(product_id))
-    assert response.ok, response.text
-    return loads(response.text)
-
-
-def product_url(product_id: str) -> str:
-    return (
-        f"https://cmems-be.lobelia.earth/api/dataset/{product_id}"
-        + "?variant=detailed-v2"
-    )
-
-
-def variable_title_to_standard_name(variable_title: str) -> str:
-    return variable_title.lower().replace(" ", "_")
-
-
-def variable_to_pick(layer: dict[str, Any]) -> bool:
-    return (
-        layer["variableId"] != "__DEFAULT__"
-        and layer["subsetVariableIds"]
-        and len(layer["subsetVariableIds"]) == 1
-    )
-
-
-def to_datasets(
-    raw_services: dict[str, dict[str, str]], layers: dict[str, dict[str, Any]]
-) -> list[CopernicusMarineProductDataset]:
-    def to_service(
-        protocol_uri: Tuple[str, str]
-    ) -> CopernicusMarineDatasetService:
-        return CopernicusMarineDatasetService(
-            protocol=protocol_uri[0], uri=protocol_uri[1]
-        )
-
-    def to_variable(layer: dict[str, Any]) -> CopernicusMarineDatasetVariable:
-        def to_coordinates(
-            subset_attributes: Tuple[str, dict[str, Any]]
-        ) -> CopernicusMarineDatasetCoordinates:
-            coordinate_name = subset_attributes[0]
-            values: Optional[str]
-            if coordinate_name == "depth":
-                values = layer.get("zValues")
-            elif coordinate_name == "time":
-                values = layer.get("tValues")
-            else:
-                values = None
-            return CopernicusMarineDatasetCoordinates(
-                coordinates_id=subset_attributes[0],
-                units=subset_attributes[1]["units"],
-                minimum_value=subset_attributes[1]["min"],
-                maximum_value=subset_attributes[1]["max"],
-                step=subset_attributes[1].get("step"),
-                values=values,
-            )
-
-        return CopernicusMarineDatasetVariable(
-            short_name=layer["variableId"],
-            standard_name=variable_title_to_standard_name(
-                layer["variableTitle"]
-            ),
-            units=layer["units"],
-            bbox=layer["bbox"],
-            coordinates=list(
-                map(to_coordinates, layer["subsetAttrs"].items())
-            ),
-        )
-
-    def to_dataset(
-        dataset_group: Tuple[str, Iterable[dict[str, Any]]],
-    ) -> CopernicusMarineProductDataset:
-        dataset_id = dataset_group[0]
-        layer_elements = list(dataset_group[1])
-        return CopernicusMarineProductDataset(
-            dataset_id=dataset_id,
-            dataset_name=layer_elements[0]["subdatasetTitle"],
-            services=list(map(to_service, raw_services[dataset_id].items())),
-            variables=list(
-                map(to_variable, filter(variable_to_pick, layer_elements))
-            ),
-        )
-
-    groups = groupby(layers.values(), key=lambda layer: layer["subdatasetId"])
-    return sorted(
-        map(to_dataset, groups), key=lambda dataset: dataset.dataset_id
-    )
-
-
-def _parse_product(raw_product: dict[str, Any]) -> CopernicusMarineProduct:
-    return CopernicusMarineProduct(
-        title=raw_product["title"],
-        product_id=raw_product["id"],
-        thumbnail_url=raw_product["thumbnailUrl"],
-        description=raw_product["abstract"],
-        production_center=raw_product["originatingCenter"],
-        creation_datetime=raw_product["creationDate"],
-        modified_datetime=raw_product.get("modifiedDate"),
-        keywords=raw_product["keywords"],
-        datasets=to_datasets(raw_product["services"], raw_product["layers"]),
-    )
-
-
-def parse_dissemination_unit_catalogue(
-    overwrite_cache: bool = False,
-) -> CopernicusMarineCatalogue:
-    raw_products: list[dict[str, Any]] = _fetch_raw_products(
-        overwrite_cache=overwrite_cache
-    )
-
-    return CopernicusMarineCatalogue(
-        products=sorted(
-            map(_parse_product, raw_products),
-            key=lambda product: product.product_id,
-        ),
-    )
-
-
-# ------------------------------------------------
-# --- Function specific for MDS STAC catalogue ---
-# ------------------------------------------------
-
-MDS_STAC_BASE_URL = (
-    "https://s3.waw3-1.cloudferro.com/mdl-metadata/metadata/catalog.stac.json"
-)
-
-
-@cachier(stale_after=timedelta(hours=3))
-def _fetch_stac_raw_data() -> list[Tuple[Collection, list[Item]]]:
-    stac_catalogue = Catalog.from_file(MDS_STAC_BASE_URL)
-    products = [
-        stac_product
-        for stac_product in map_parallel(
-            _create_collection,
-            tqdm(
-                stac_catalogue.get_child_links(),
-                desc="Fetching marine data store raw products",
-            ),
-        )
-        if stac_product
-    ]
-    return map_parallel(
-        _fetch_stac_datasets,
-        tqdm(products, desc="Fetching marine data store raw datasets"),
-    )
-
-
-def _fetch_stac_datasets(
-    stac_product: Collection,
-) -> Tuple[Collection, list[Item]]:
-    return (
-        stac_product,
-        [
-            stac_dataset
-            for stac_dataset in map(
-                _create_item, stac_product.get_item_links()
-            )
-            if stac_dataset
-        ],
-    )
-
-
-def _create_collection(link: Link) -> Union[Collection, None]:
-    try:
-        return Collection.from_file(link.get_absolute_href())
-    except KeyError as e:
-        messages = ["spatial", "temporal"]
-        if e.args[0] not in messages:
-            raise KeyError(e.args)
-        return None
-
-
-def _create_item(link: Link) -> Union[Item, None]:
-    try:
-        return Item.from_file(link.get_absolute_href())
-    except STACError as e:
-        message = (
-            "Invalid Item: If datetime is None, a start_datetime "
-            + "and end_datetime must be supplied."
-        )
-        if e.args[0] != message:
-            raise STACError(e.args)
-        return None
-
-
-def parse_marine_data_store_catalogue(
-    overwrite_cache: bool = False,
-) -> CopernicusMarineCatalogue:
-    stac_raw_data = _fetch_stac_raw_data(overwrite_cache=overwrite_cache)
-    products = map_reject_none(_construct_mds_product, stac_raw_data)
-    return CopernicusMarineCatalogue(
-        products=sorted(
-            [product for product in products if product],
-            key=lambda product: product.product_id,
-        )
-    )
-
-
-def _construct_mds_product(
-    stac_tuple: Tuple[Collection, list[Item]],
-) -> CopernicusMarineProduct:
-    stac_product, stac_datasets = stac_tuple
-    datasets = map_reject_none(_construct_mds_dataset, stac_datasets)
-    production_center = [
-        provider.name
-        for provider in stac_product.providers
-        if "producer" in provider.roles
-    ][0]
-    return CopernicusMarineProduct(
-        title=stac_product.title,
-        product_id=stac_product.id,
-        thumbnail_url=stac_product.assets["thumbnail"].get_absolute_href(),
-        description=stac_product.description,
-        production_center=production_center,
-        creation_datetime=stac_product.extra_fields["properties"][
-            "creationDate"
-        ],
-        modified_datetime=stac_product.extra_fields["properties"].get(
-            "modifiedDate"
-        ),
-        keywords=stac_product.keywords,
-        datasets=sorted(
-            [dataset for dataset in datasets],
-            key=lambda dataset: dataset.dataset_id,
-        ),
-    )
-
-
-def _construct_mds_dataset(
-    stac_dataset: Item,
-) -> CopernicusMarineProductDataset:
-    dataset_id = stac_dataset.id.rsplit("_", maxsplit=1)[
-        0
-    ]  # Remove the tag e.g.: '_202211'
-    return CopernicusMarineProductDataset(
-        dataset_id=dataset_id,
-        dataset_name=stac_dataset.properties["title"],
-        services=_get_services(stac_dataset.get_assets()),
-        variables=_get_variables(stac_dataset),
-    )
-
-
-def _get_services(
-    stac_assets_dict: dict[str, Asset],
-) -> list[CopernicusMarineDatasetService]:
-
-    only_data_stac_assets = [
-        CopernicusMarineDatasetService(
-            protocol=key,
-            uri=value.get_absolute_href(),
-        )
-        for key, value in stac_assets_dict.items()
-        if "data" in value.roles
-    ]
-    return only_data_stac_assets
-
-
-def _get_variables(
-    stac_dataset: Item,
-) -> list[CopernicusMarineDatasetVariable]:
-    def _create_variable(
-        variable_cube: dict[str, Any],
-        bbox: tuple[float, float, float, float],
-        coordinates_dict: dict[str, CopernicusMarineDatasetCoordinates],
-    ) -> Union[CopernicusMarineDatasetVariable, None]:
-        coordinates = variable_cube["dimensions"]
-        return CopernicusMarineDatasetVariable(
-            short_name=variable_cube["id"],
-            standard_name=variable_cube["standardName"],
-            units=variable_cube.get("unit") or "",
-            bbox=bbox,
-            coordinates=[coordinates_dict[key] for key in coordinates],
-        )
-
-    coordinates_dict = _get_coordinates(
-        stac_dataset.properties["cube:dimensions"]
-    )
-    bbox = stac_dataset.bbox
-    variables: list[Optional[CopernicusMarineDatasetVariable]] = []
-    for var_cube in stac_dataset.properties["cube:variables"].values():
-        variables += [_create_variable(var_cube, bbox, coordinates_dict)]
-    return [var for var in variables if var]
-
-
-def _get_coordinates(
-    dimensions_cube: dict,
-) -> dict[str, CopernicusMarineDatasetCoordinates]:
-    def _create_coordinate(
-        key: str, value: dict
-    ) -> CopernicusMarineDatasetCoordinates:
-        return CopernicusMarineDatasetCoordinates(
-            coordinates_id="depth" if key == "elevation" else key,
-            units=value.get("unit") or "",
-            minimum_value=value["extent"][0],
-            maximum_value=value["extent"][1],
-            step=value.get("step"),
-            values=value.get("values"),
-        )
-
-    coordinates_dict = {}
-    for key, value in dimensions_cube.items():
-        coordinates_dict[key] = _create_coordinate(key, value)
-    return coordinates_dict
-
-
-# ---------------------------------------
-# --- Utils function on any catalogue ---
-# ---------------------------------------
-
-
-def get_protocol_url_from_id(
-    dataset_id: str, protocol_key_order: list[str]
-) -> Tuple[str, str]:
-    catalogue = parse_catalogue()
-    dataset_urls = (
-        get_dataset_url_from_id(catalogue, dataset_id, protocol)
-        for protocol in protocol_key_order
-    )
-    try:
-        dataset_url = next(filter(lambda dataset: dataset, dataset_urls))
-        protocol = get_protocol_from_url(dataset_url)
-    except StopIteration as exception:
-        raise KeyError(
-            f"Dataset {dataset_id} does not have a valid protocol "
-            f"for subset function. Available protocols: {protocol_key_order}"
-        ) from exception
-    return protocol, dataset_url
-
-
-def get_dataset_from_id(
-    catalogue: CopernicusMarineCatalogue, dataset_id: str
-) -> CopernicusMarineProductDataset:
-    for product in catalogue.products:
-        for dataset in product.datasets:
-            if dataset_id == dataset.dataset_id:
-                return dataset
-    raise KeyError(
-        f"The requested dataset '{dataset_id}' was not found in the catalogue,"
-        " you can use 'copernicus-marine describe --include-datasets "
-        "-c <search_token>' to find the dataset id"
-    )
-
-
-def get_product_from_url(
-    catalogue: CopernicusMarineCatalogue, dataset_url: str
-) -> CopernicusMarineProduct:
-    """
-    Return the product object, with its dataset list filtered
-    """
-    filtered_catalogue = filter_catalogue_with_strings(
-        catalogue, [dataset_url]
-    )
-    if filtered_catalogue is None:
-        raise TypeError("filtered catalogue is empty")
-    return filtered_catalogue.products[0]
-
-
-def get_protocol_from_url(dataset_url) -> str:
-    if dataset_url.startswith("ftp://"):
-        protocol = FTP_KEY
-    elif "/motu-web/Motu" in dataset_url:
-        protocol = MOTU_KEY
-    elif "/wms/" in dataset_url:
-        protocol = "OGC:WMS:getCapabilities"
-    elif "/thredds/dodsC/" in dataset_url:
-        protocol = OPENDAP_KEY
-    elif "/mdl-arco-time/" in dataset_url:
-        protocol = TIMECHUNKED_KEY
-    elif "/mdl-arco-geo/" in dataset_url:
-        protocol = GEOCHUNKED_KEY
-    elif "/mdl-native/" in dataset_url:
-        protocol = S3NATIVE_KEY
-    else:
-        raise ValueError(f"No protocol matching url: {dataset_url}")
-    return protocol
-
-
-def get_service_url(
-    dataset: CopernicusMarineProductDataset, protocol: str
-) -> str:
-    service_urls = iter(
-        [
-            service.uri
-            for service in dataset.services
-            if service.protocol == protocol
-        ]
-    )
-    return next(service_urls, "")
-
-
-def get_dataset_url_from_id(
-    catalogue: CopernicusMarineCatalogue, dataset_id: str, protocol: str
-) -> str:
-    dataset = get_dataset_from_id(catalogue, dataset_id)
-    return get_service_url(dataset, protocol)
-
-
-def filter_catalogue_with_strings(
-    catalogue: CopernicusMarineCatalogue, tokens: list[str]
-) -> Optional[CopernicusMarineCatalogue]:
-    filtered_catalogue = deepcopy(catalogue)
-    return find_match_object(filtered_catalogue, tokens)
-
-
-def find_match_object(value: Any, tokens: list[str]) -> Any:
-    match: Any
-    if isinstance(value, str):
-        match = find_match_string(value, tokens)
-    elif isinstance(value, list):
-        match = find_match_list(value, tokens)
-    elif hasattr(value, "__dict__"):
-        match = find_match_dict(value, tokens)
-    else:
-        match = None
-    return match
-
-
-def find_match_string(string: str, tokens: list[str]) -> Optional[str]:
-    return string if any(token in string for token in tokens) else None
-
-
-def find_match_list(object_list: list[Any], tokens) -> Optional[list[Any]]:
-    def find_match(element: Any) -> Optional[Any]:
-        return find_match_object(element, tokens)
-
-    filtered_list: list[Any] = list(map_reject_none(find_match, object_list))
-    return filtered_list if filtered_list else None
-
-
-def find_match_dict(
-    structure: dict[str, Any], tokens
-) -> Optional[dict[str, Any]]:
-    filtered_dict = {
-        key: find_match_object(value, tokens)
-        for key, value in structure.__dict__.items()
-        if find_match_object(value, tokens)
-    }
-
-    found_match = any(filtered_dict.values())
-    if found_match:
-        new_dict = dict(structure.__dict__, **filtered_dict)
-        structure.__dict__ = new_dict
-    return structure if found_match else None
-
-
-def _merge_object(obj1: Any, obj2: Any) -> Any:
-    """Function called to merge catalogues
-    Redirect either to _merge_list or to _merge_dict functions
-    _merge_dict is also used to merge custom_class attributes
-    """
-    if isinstance(obj1, list):
-        return _merge_list(obj1, obj2)
-    elif hasattr(obj1, "__dict__"):
-        merged_obj = obj1
-        merged_obj.__dict__ = _merge_dict(obj1.__dict__, obj2.__dict__)
-        return merged_obj
-    else:
-        return obj1
-
-
-def _merge_dict(
-    dict1: dict[str, Any], dict2: dict[str, Any]
-) -> dict[str, Any]:
-    """Merge dictionnaries key by key"""
-    keys = set(list(dict1.keys()) + list(dict2.keys()))
-    return {key: _merge_object(dict1[key], dict2[key]) for key in keys}
-
-
-def _merge_list(list1: list[Any], list2: list[Any]) -> list[Any]:
-    """Merge lists
-    If it is a list of one of our custom class, we want to append new objects to list
-    and merge matches between the two lists
-    Otherwise keep first non-empty list
-    """
-
-    def _objects_match(args: Tuple[Any, str, str]) -> Union[Any, None]:
-        """Filter to check if an object's attribute match a value"""
-        obj, attribute, value = args
-        return True if obj.__dict__[attribute] == value else False
-
-    class_id_attribute_dict = {
-        CopernicusMarineProduct: "product_id",
-        CopernicusMarineProductDataset: "dataset_id",
-        CopernicusMarineDatasetService: "protocol",
-        CopernicusMarineDatasetVariable: "short_name",
-    }
-    if not list1:
-        if not list2:
-            return []
-        else:
-            main_list = list2
-    else:
-        main_list = list1
-    if isinstance(
-        main_list[0],
-        (
-            CopernicusMarineProduct,
-            CopernicusMarineProductDataset,
-            CopernicusMarineDatasetService,
-            CopernicusMarineDatasetVariable,
-        ),
-    ):
-        id_attribute = class_id_attribute_dict[type(main_list[0])]
-        object_ids = set(
-            [object1.__dict__[id_attribute] for object1 in list1]
-            + [object2.__dict__[id_attribute] for object2 in list2]
-        )
-        merged_list = []
-        for object_id in object_ids:
-            list1_match = list(
-                filter(
-                    _objects_match,
-                    zip(
-                        list1,
-                        [id_attribute] * len(list1),
-                        [object_id] * len(list1),
-                    ),
-                )
-            )
-            list2_match = list(
-                filter(
-                    _objects_match,
-                    zip(
-                        list2,
-                        [id_attribute] * len(list2),
-                        [object_id] * len(list2),
-                    ),
-                )
-            )
-            if list1_match and list2_match:
-                merged_list += [
-                    _merge_object(list1_match[0][0], list2_match[0][0])
-                ]
-            elif list1_match:
-                merged_list += [list1_match[0][0]]
-            elif list2_match:
-                merged_list += [list2_match[0][0]]
-            else:
-                pass
-        return sorted(
-            merged_list, key=lambda elem: elem.__dict__[id_attribute]
-        )
-    else:
-        return main_list
-
-
-def merge_catalogues(
-    catalogue1: CopernicusMarineCatalogue,
-    catalogue2: CopernicusMarineCatalogue,
-) -> CopernicusMarineCatalogue:
-    """Function to combine two catalogues, with priority given to
-    catalogue1 in case of conflicts"""
-    catalogue = _merge_object(catalogue1, catalogue2)
-    return catalogue
-
-
-def get_all_dataset_ids() -> list[str]:
-    catalogue = parse_catalogue()
-    return [
-        dataset.dataset_id
-        for product in catalogue.products
-        for dataset in product.datasets
-    ]
-
-
-if __name__ == "__main__":
-    import cProfile
-    import io
-    import pstats
-    from pstats import SortKey
-
-    pr = cProfile.Profile()
-    pr.enable()
-    parse_catalogue()
-    pr.disable()
-    s = io.StringIO()
-    sortby = SortKey.CUMULATIVE
-    ps = pstats.Stats(pr, stream=s).sort_stats(sortby)
-    ps.print_stats(50)
-    print(s.getvalue())
+import logging
+import logging.config
+from copy import deepcopy
+from dataclasses import dataclass
+from datetime import timedelta
+from itertools import groupby
+from json import loads
+from multiprocessing import Pool
+from typing import Any, Callable, Iterable, Optional, Tuple, TypeVar, Union
+
+import requests
+from cachier import cachier
+from pystac import Asset, Catalog, Collection, Item, Link, STACError
+from tqdm import tqdm
+
+
+@dataclass
+class CopernicusMarineDatasetService:
+    protocol: str
+    uri: str
+
+
+@dataclass
+class CopernicusMarineDatasetCoordinates:
+    coordinates_id: str
+    units: str
+    minimum_value: float
+    maximum_value: float
+    step: Optional[float]
+    values: Optional[str]
+
+
+@dataclass
+class CopernicusMarineDatasetVariable:
+    short_name: str
+    standard_name: str
+    units: str
+    bbox: Tuple[float, float, float, float]
+    coordinates: list[CopernicusMarineDatasetCoordinates]
+
+
+@dataclass
+class CopernicusMarineProductDataset:
+    dataset_id: str
+    dataset_name: str
+    services: list[CopernicusMarineDatasetService]
+    variables: list[CopernicusMarineDatasetVariable]
+
+
+@dataclass
+class CopernicusMarineProductProvider:
+    name: str
+    roles: list[str]
+    url: str
+    email: str
+
+
+@dataclass
+class CopernicusMarineProduct:
+    title: str
+    product_id: str
+    thumbnail_url: str
+    description: str
+    production_center: str
+    creation_datetime: str
+    modified_datetime: Optional[str]
+    keywords: dict[str, str]
+    datasets: list[CopernicusMarineProductDataset]
+
+
+@dataclass
+class CopernicusMarineCatalogue:
+    products: list[CopernicusMarineProduct]
+
+    def filter(self, tokens: list[str]):
+        return filter_catalogue_with_strings(self, tokens)
+
+
+OPENDAP_KEY = "opendap"
+MOTU_KEY = "motu"
+FTP_KEY = "ftp"
+GEOCHUNKED_KEY = "geoChunked"
+TIMECHUNKED_KEY = "timeChunked"
+S3NATIVE_KEY = "native"
+DOWNSAMPLED4_KEY = "downsampled4"
+
+_S = TypeVar("_S")
+_T = TypeVar("_T")
+
+
+def map_parallel(
+    function: Callable[[_S], _T], iterable: Iterable[_S]
+) -> list[_T]:
+    parallel_processes = 20
+    with Pool(parallel_processes) as pool:
+        return pool.map(function, iterable)
+
+
+def map_reject_none(
+    function: Callable[[_S], Optional[_T]], iterable: Iterable[_S]
+) -> Iterable[_T]:
+    return (element for element in map(function, iterable) if element)
+
+
+def parse_catalogue(
+    overwrite_cache: bool = False,
+) -> CopernicusMarineCatalogue:
+    return merge_catalogues(
+        parse_dissemination_unit_catalogue(overwrite_cache=overwrite_cache),
+        parse_marine_data_store_catalogue(overwrite_cache=overwrite_cache),
+    )
+
+
+# --------------------------------------------------------
+# --- Function specific for cmems-be.lobelia catalogue ---
+# --------------------------------------------------------
+@cachier(stale_after=timedelta(hours=3))
+def _fetch_raw_products() -> list[dict[str, Any]]:
+    response = requests.post(
+        "https://cmems-be.lobelia.earth/api/datasets",
+        json={"size": 1000, "includeOmis": True},
+    )
+    assert response.ok, response.text
+    raw_catalogue: dict[str, Any] = loads(response.text)
+    return map_parallel(
+        _fetch_raw_product,
+        tqdm(
+            raw_catalogue["datasets"].keys(),
+            desc="Fetching metadata for dissemination unit raw products",
+        ),
+    )
+
+
+def _fetch_raw_product(product_id: str) -> dict[str, Any]:
+    response = requests.get(product_url(product_id))
+    assert response.ok, response.text
+    return loads(response.text)
+
+
+def product_url(product_id: str) -> str:
+    return (
+        f"https://cmems-be.lobelia.earth/api/dataset/{product_id}"
+        + "?variant=detailed-v2"
+    )
+
+
+def variable_title_to_standard_name(variable_title: str) -> str:
+    return variable_title.lower().replace(" ", "_")
+
+
+def variable_to_pick(layer: dict[str, Any]) -> bool:
+    return (
+        layer["variableId"] != "__DEFAULT__"
+        and layer["subsetVariableIds"]
+        and len(layer["subsetVariableIds"]) == 1
+    )
+
+
+def to_datasets(
+    raw_services: dict[str, dict[str, str]], layers: dict[str, dict[str, Any]]
+) -> list[CopernicusMarineProductDataset]:
+    def to_service(
+        protocol_uri: Tuple[str, str]
+    ) -> CopernicusMarineDatasetService:
+        return CopernicusMarineDatasetService(
+            protocol=protocol_uri[0], uri=protocol_uri[1]
+        )
+
+    def to_variable(layer: dict[str, Any]) -> CopernicusMarineDatasetVariable:
+        def to_coordinates(
+            subset_attributes: Tuple[str, dict[str, Any]]
+        ) -> CopernicusMarineDatasetCoordinates:
+            coordinate_name = subset_attributes[0]
+            values: Optional[str]
+            if coordinate_name == "depth":
+                values = layer.get("zValues")
+            elif coordinate_name == "time":
+                values = layer.get("tValues")
+            else:
+                values = None
+            return CopernicusMarineDatasetCoordinates(
+                coordinates_id=subset_attributes[0],
+                units=subset_attributes[1]["units"],
+                minimum_value=subset_attributes[1]["min"],
+                maximum_value=subset_attributes[1]["max"],
+                step=subset_attributes[1].get("step"),
+                values=values,
+            )
+
+        return CopernicusMarineDatasetVariable(
+            short_name=layer["variableId"],
+            standard_name=variable_title_to_standard_name(
+                layer["variableTitle"]
+            ),
+            units=layer["units"],
+            bbox=layer["bbox"],
+            coordinates=list(
+                map(to_coordinates, layer["subsetAttrs"].items())
+            ),
+        )
+
+    def to_dataset(
+        dataset_group: Tuple[str, Iterable[dict[str, Any]]],
+    ) -> CopernicusMarineProductDataset:
+        dataset_id = dataset_group[0]
+        layer_elements = list(dataset_group[1])
+        return CopernicusMarineProductDataset(
+            dataset_id=dataset_id,
+            dataset_name=layer_elements[0]["subdatasetTitle"],
+            services=list(map(to_service, raw_services[dataset_id].items())),
+            variables=list(
+                map(to_variable, filter(variable_to_pick, layer_elements))
+            ),
+        )
+
+    groups = groupby(layers.values(), key=lambda layer: layer["subdatasetId"])
+    return sorted(
+        map(to_dataset, groups), key=lambda dataset: dataset.dataset_id
+    )
+
+
+def _parse_product(raw_product: dict[str, Any]) -> CopernicusMarineProduct:
+    return CopernicusMarineProduct(
+        title=raw_product["title"],
+        product_id=raw_product["id"],
+        thumbnail_url=raw_product["thumbnailUrl"],
+        description=raw_product["abstract"],
+        production_center=raw_product["originatingCenter"],
+        creation_datetime=raw_product["creationDate"],
+        modified_datetime=raw_product.get("modifiedDate"),
+        keywords=raw_product["keywords"],
+        datasets=to_datasets(raw_product["services"], raw_product["layers"]),
+    )
+
+
+def parse_dissemination_unit_catalogue(
+    overwrite_cache: bool = False,
+) -> CopernicusMarineCatalogue:
+    raw_products: list[dict[str, Any]] = _fetch_raw_products(
+        overwrite_cache=overwrite_cache
+    )
+
+    return CopernicusMarineCatalogue(
+        products=sorted(
+            map(_parse_product, raw_products),
+            key=lambda product: product.product_id,
+        ),
+    )
+
+
+# ------------------------------------------------
+# --- Function specific for MDS STAC catalogue ---
+# ------------------------------------------------
+
+MDS_STAC_BASE_URL = (
+    "https://s3.waw3-1.cloudferro.com/mdl-metadata/metadata/catalog.stac.json"
+)
+
+
+@cachier(stale_after=timedelta(hours=3))
+def _fetch_stac_raw_data() -> list[Tuple[Collection, list[Item]]]:
+    stac_catalogue = Catalog.from_file(MDS_STAC_BASE_URL)
+    products = [
+        stac_product
+        for stac_product in map_parallel(
+            _create_collection,
+            tqdm(
+                stac_catalogue.get_child_links(),
+                desc="Fetching metadata for marine data store raw products",
+            ),
+        )
+        if stac_product
+    ]
+    return map_parallel(
+        _fetch_stac_datasets,
+        tqdm(
+            products,
+            desc="Fetching metadata for marine data store raw datasets",
+        ),
+    )
+
+
+def _fetch_stac_datasets(
+    stac_product: Collection,
+) -> Tuple[Collection, list[Item]]:
+    return (
+        stac_product,
+        [
+            stac_dataset
+            for stac_dataset in map(
+                _create_item, stac_product.get_item_links()
+            )
+            if stac_dataset
+        ],
+    )
+
+
+def _create_collection(link: Link) -> Union[Collection, None]:
+    try:
+        return Collection.from_file(link.get_absolute_href())
+    except KeyError as e:
+        messages = ["spatial", "temporal"]
+        if e.args[0] not in messages:
+            logging.error(e)
+            raise KeyError(e.args)
+        return None
+
+
+def _create_item(link: Link) -> Union[Item, None]:
+    try:
+        return Item.from_file(link.get_absolute_href())
+    except STACError as e:
+        message = (
+            "Invalid Item: If datetime is None, a start_datetime "
+            + "and end_datetime must be supplied."
+        )
+        if e.args[0] != message:
+            logging.error(e)
+            raise STACError(e.args)
+        return None
+
+
+def parse_marine_data_store_catalogue(
+    overwrite_cache: bool = False,
+) -> CopernicusMarineCatalogue:
+    stac_raw_data = _fetch_stac_raw_data(overwrite_cache=overwrite_cache)
+    products = map_reject_none(_construct_mds_product, stac_raw_data)
+    return CopernicusMarineCatalogue(
+        products=sorted(
+            [product for product in products if product],
+            key=lambda product: product.product_id,
+        )
+    )
+
+
+def _construct_mds_product(
+    stac_tuple: Tuple[Collection, list[Item]],
+) -> CopernicusMarineProduct:
+    stac_product, stac_datasets = stac_tuple
+    datasets = map_reject_none(_construct_mds_dataset, stac_datasets)
+    production_center = [
+        provider.name
+        for provider in stac_product.providers
+        if "producer" in provider.roles
+    ][0]
+    return CopernicusMarineProduct(
+        title=stac_product.title,
+        product_id=stac_product.id,
+        thumbnail_url=stac_product.assets["thumbnail"].get_absolute_href(),
+        description=stac_product.description,
+        production_center=production_center,
+        creation_datetime=stac_product.extra_fields["properties"][
+            "creationDate"
+        ],
+        modified_datetime=stac_product.extra_fields["properties"].get(
+            "modifiedDate"
+        ),
+        keywords=stac_product.keywords,
+        datasets=sorted(
+            [dataset for dataset in datasets],
+            key=lambda dataset: dataset.dataset_id,
+        ),
+    )
+
+
+def _construct_mds_dataset(
+    stac_dataset: Item,
+) -> CopernicusMarineProductDataset:
+    dataset_id = stac_dataset.id.rsplit("_", maxsplit=1)[
+        0
+    ]  # Remove the tag e.g.: '_202211'
+    return CopernicusMarineProductDataset(
+        dataset_id=dataset_id,
+        dataset_name=stac_dataset.properties["title"],
+        services=_get_services(stac_dataset.get_assets()),
+        variables=_get_variables(stac_dataset),
+    )
+
+
+def _get_services(
+    stac_assets_dict: dict[str, Asset],
+) -> list[CopernicusMarineDatasetService]:
+
+    only_data_stac_assets = [
+        CopernicusMarineDatasetService(
+            protocol=key,
+            uri=value.get_absolute_href(),
+        )
+        for key, value in stac_assets_dict.items()
+        if "data" in value.roles
+    ]
+    return only_data_stac_assets
+
+
+def _get_variables(
+    stac_dataset: Item,
+) -> list[CopernicusMarineDatasetVariable]:
+    def _create_variable(
+        variable_cube: dict[str, Any],
+        bbox: tuple[float, float, float, float],
+        coordinates_dict: dict[str, CopernicusMarineDatasetCoordinates],
+    ) -> Union[CopernicusMarineDatasetVariable, None]:
+        coordinates = variable_cube["dimensions"]
+        return CopernicusMarineDatasetVariable(
+            short_name=variable_cube["id"],
+            standard_name=variable_cube["standardName"],
+            units=variable_cube.get("unit") or "",
+            bbox=bbox,
+            coordinates=[coordinates_dict[key] for key in coordinates],
+        )
+
+    coordinates_dict = _get_coordinates(
+        stac_dataset.properties["cube:dimensions"]
+    )
+    bbox = stac_dataset.bbox
+    variables: list[Optional[CopernicusMarineDatasetVariable]] = []
+    for var_cube in stac_dataset.properties["cube:variables"].values():
+        variables += [_create_variable(var_cube, bbox, coordinates_dict)]
+    return [var for var in variables if var]
+
+
+def _get_coordinates(
+    dimensions_cube: dict,
+) -> dict[str, CopernicusMarineDatasetCoordinates]:
+    def _create_coordinate(
+        key: str, value: dict
+    ) -> CopernicusMarineDatasetCoordinates:
+        return CopernicusMarineDatasetCoordinates(
+            coordinates_id="depth" if key == "elevation" else key,
+            units=value.get("unit") or "",
+            minimum_value=value["extent"][0],
+            maximum_value=value["extent"][1],
+            step=value.get("step"),
+            values=value.get("values"),
+        )
+
+    coordinates_dict = {}
+    for key, value in dimensions_cube.items():
+        coordinates_dict[key] = _create_coordinate(key, value)
+    return coordinates_dict
+
+
+# ---------------------------------------
+# --- Utils function on any catalogue ---
+# ---------------------------------------
+
+
+def get_protocol_url_from_id(
+    dataset_id: str, protocol_key_order: list[str]
+) -> Tuple[str, str]:
+    catalogue = parse_catalogue()
+    dataset_urls = (
+        get_dataset_url_from_id(catalogue, dataset_id, protocol)
+        for protocol in protocol_key_order
+    )
+    try:
+        dataset_url = next(filter(lambda dataset: dataset, dataset_urls))
+        protocol = get_protocol_from_url(dataset_url)
+    except StopIteration as exception:
+        error = KeyError(
+            f"Dataset {dataset_id} does not have a valid protocol "
+            f"for subset function. Available protocols: {protocol_key_order}"
+        )
+        logging.error(error)
+        raise error from exception
+    return protocol, dataset_url
+
+
+def get_dataset_from_id(
+    catalogue: CopernicusMarineCatalogue, dataset_id: str
+) -> CopernicusMarineProductDataset:
+    for product in catalogue.products:
+        for dataset in product.datasets:
+            if dataset_id == dataset.dataset_id:
+                return dataset
+    error = KeyError(
+        f"The requested dataset '{dataset_id}' was not found in the catalogue,"
+        " you can use 'copernicus-marine describe --include-datasets "
+        "-c <search_token>' to find the dataset id"
+    )
+    logging.error(error)
+    raise error
+
+
+def get_product_from_url(
+    catalogue: CopernicusMarineCatalogue, dataset_url: str
+) -> CopernicusMarineProduct:
+    """
+    Return the product object, with its dataset list filtered
+    """
+    filtered_catalogue = filter_catalogue_with_strings(
+        catalogue, [dataset_url]
+    )
+    if filtered_catalogue is None:
+        error = TypeError("filtered catalogue is empty")
+        raise error
+    return filtered_catalogue.products[0]
+
+
+def get_protocol_from_url(dataset_url) -> str:
+    if dataset_url.startswith("ftp://"):
+        protocol = FTP_KEY
+    elif "/motu-web/Motu" in dataset_url:
+        protocol = MOTU_KEY
+    elif "/wms/" in dataset_url:
+        protocol = "OGC:WMS:getCapabilities"
+    elif "/thredds/dodsC/" in dataset_url:
+        protocol = OPENDAP_KEY
+    elif "/mdl-arco-time/" in dataset_url:
+        protocol = TIMECHUNKED_KEY
+    elif "/mdl-arco-geo/" in dataset_url:
+        protocol = GEOCHUNKED_KEY
+    elif "/mdl-native/" in dataset_url:
+        protocol = S3NATIVE_KEY
+    else:
+        exception = ValueError(f"No protocol matching url: {dataset_url}")
+        logging.error(exception)
+        raise exception
+    return protocol
+
+
+def get_service_url(
+    dataset: CopernicusMarineProductDataset, protocol: str
+) -> str:
+    service_urls = iter(
+        [
+            service.uri
+            for service in dataset.services
+            if service.protocol == protocol
+        ]
+    )
+    return next(service_urls, "")
+
+
+def get_dataset_url_from_id(
+    catalogue: CopernicusMarineCatalogue, dataset_id: str, protocol: str
+) -> str:
+    dataset = get_dataset_from_id(catalogue, dataset_id)
+    return get_service_url(dataset, protocol)
+
+
+def filter_catalogue_with_strings(
+    catalogue: CopernicusMarineCatalogue, tokens: list[str]
+) -> Optional[CopernicusMarineCatalogue]:
+    filtered_catalogue = deepcopy(catalogue)
+    return find_match_object(filtered_catalogue, tokens)
+
+
+def find_match_object(value: Any, tokens: list[str]) -> Any:
+    match: Any
+    if isinstance(value, str):
+        match = find_match_string(value, tokens)
+    elif isinstance(value, list):
+        match = find_match_list(value, tokens)
+    elif hasattr(value, "__dict__"):
+        match = find_match_dict(value, tokens)
+    else:
+        match = None
+    return match
+
+
+def find_match_string(string: str, tokens: list[str]) -> Optional[str]:
+    return string if any(token in string for token in tokens) else None
+
+
+def find_match_list(object_list: list[Any], tokens) -> Optional[list[Any]]:
+    def find_match(element: Any) -> Optional[Any]:
+        return find_match_object(element, tokens)
+
+    filtered_list: list[Any] = list(map_reject_none(find_match, object_list))
+    return filtered_list if filtered_list else None
+
+
+def find_match_dict(
+    structure: dict[str, Any], tokens
+) -> Optional[dict[str, Any]]:
+    filtered_dict = {
+        key: find_match_object(value, tokens)
+        for key, value in structure.__dict__.items()
+        if find_match_object(value, tokens)
+    }
+
+    found_match = any(filtered_dict.values())
+    if found_match:
+        new_dict = dict(structure.__dict__, **filtered_dict)
+        structure.__dict__ = new_dict
+    return structure if found_match else None
+
+
+def _merge_object(obj1: Any, obj2: Any) -> Any:
+    """Function called to merge catalogues
+    Redirect either to _merge_list or to _merge_dict functions
+    _merge_dict is also used to merge custom_class attributes
+    """
+    if isinstance(obj1, list):
+        return _merge_list(obj1, obj2)
+    elif hasattr(obj1, "__dict__"):
+        merged_obj = obj1
+        merged_obj.__dict__ = _merge_dict(obj1.__dict__, obj2.__dict__)
+        return merged_obj
+    else:
+        return obj1
+
+
+def _merge_dict(
+    dict1: dict[str, Any], dict2: dict[str, Any]
+) -> dict[str, Any]:
+    """Merge dictionnaries key by key"""
+    keys = set(list(dict1.keys()) + list(dict2.keys()))
+    return {key: _merge_object(dict1[key], dict2[key]) for key in keys}
+
+
+def _merge_list(list1: list[Any], list2: list[Any]) -> list[Any]:
+    """Merge lists
+    If it is a list of one of our custom class, we want to append new objects to list
+    and merge matches between the two lists
+    Otherwise keep first non-empty list
+    """
+
+    def _objects_match(args: Tuple[Any, str, str]) -> Union[Any, None]:
+        """Filter to check if an object's attribute match a value"""
+        obj, attribute, value = args
+        return True if obj.__dict__[attribute] == value else False
+
+    class_id_attribute_dict = {
+        CopernicusMarineProduct: "product_id",
+        CopernicusMarineProductDataset: "dataset_id",
+        CopernicusMarineDatasetService: "protocol",
+        CopernicusMarineDatasetVariable: "short_name",
+    }
+    if not list1:
+        if not list2:
+            return []
+        else:
+            main_list = list2
+    else:
+        main_list = list1
+    if isinstance(
+        main_list[0],
+        (
+            CopernicusMarineProduct,
+            CopernicusMarineProductDataset,
+            CopernicusMarineDatasetService,
+            CopernicusMarineDatasetVariable,
+        ),
+    ):
+        id_attribute = class_id_attribute_dict[type(main_list[0])]
+        object_ids = set(
+            [object1.__dict__[id_attribute] for object1 in list1]
+            + [object2.__dict__[id_attribute] for object2 in list2]
+        )
+        merged_list = []
+        for object_id in object_ids:
+            list1_match = list(
+                filter(
+                    _objects_match,
+                    zip(
+                        list1,
+                        [id_attribute] * len(list1),
+                        [object_id] * len(list1),
+                    ),
+                )
+            )
+            list2_match = list(
+                filter(
+                    _objects_match,
+                    zip(
+                        list2,
+                        [id_attribute] * len(list2),
+                        [object_id] * len(list2),
+                    ),
+                )
+            )
+            if list1_match and list2_match:
+                merged_list += [
+                    _merge_object(list1_match[0][0], list2_match[0][0])
+                ]
+            elif list1_match:
+                merged_list += [list1_match[0][0]]
+            elif list2_match:
+                merged_list += [list2_match[0][0]]
+            else:
+                pass
+        return sorted(
+            merged_list, key=lambda elem: elem.__dict__[id_attribute]
+        )
+    else:
+        return main_list
+
+
+def merge_catalogues(
+    catalogue1: CopernicusMarineCatalogue,
+    catalogue2: CopernicusMarineCatalogue,
+) -> CopernicusMarineCatalogue:
+    """Function to combine two catalogues, with priority given to
+    catalogue1 in case of conflicts"""
+    catalogue = _merge_object(catalogue1, catalogue2)
+    return catalogue
+
+
+def get_all_dataset_ids() -> list[str]:
+    catalogue = parse_catalogue()
+    return [
+        dataset.dataset_id
+        for product in catalogue.products
+        for dataset in product.datasets
+    ]
+
+
+if __name__ == "__main__":
+    import cProfile
+    import io
+    import pstats
+    from pstats import SortKey
+
+    pr = cProfile.Profile()
+    pr.enable()
+    parse_catalogue()
+    pr.disable()
+    s = io.StringIO()
+    sortby = SortKey.CUMULATIVE
+    ps = pstats.Stats(pr, stream=s).sort_stats(sortby)
+    ps.print_stats(50)
+    print(s.getvalue())
```

### Comparing `copernicus_marine_client-0.7.1/copernicus_marine_client/command_line_interface/group_describe.py` & `copernicus_marine_client-0.8.0/copernicus_marine_client/command_line_interface/group_describe.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,122 +1,140 @@
-from json import dumps
-from typing import Any
-
-import click
-
-from copernicus_marine_client.catalogue_parser.catalogue_parser import (
-    CopernicusMarineCatalogue,
-    filter_catalogue_with_strings,
-    parse_catalogue,
-)
-
-
-@click.group()
-def cli_group_describe() -> None:
-    pass
-
-
-@cli_group_describe.command(
-    "describe",
-    help="""
-    Parse the Copernicus Marine catalogue, then display a
-    JSON-ified version of the corresponding python object.
-
-    The default display contains information on the products, and more data
-    can be displayed using the _include-<argument>_ flags (see Usage section).
-
-    The _contains_ option allows the user to specify one or several strings to
-    filter through the catalogue display. The search is performed recursively
-    on all attributes of the catalogue, and the tokens only need to be
-    contained in one of the attributes (i.e. not exact match).
-
-    Example:
-
-    > copernicus-marine describe --contains METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
-    --include-datasets
-
-    > copernicus-marine describe -c METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
-        """,
-)
-@click.option(
-    "--one-line",
-    type=bool,
-    is_flag=True,
-    default=False,
-    help="Output JSON on one line",
-)
-@click.option(
-    "--include-description",
-    type=bool,
-    is_flag=True,
-    default=False,
-    help="Include product description in output",
-)
-@click.option(
-    "--include-datasets",
-    type=bool,
-    is_flag=True,
-    default=False,
-    help="Include product dataset details in output",
-)
-@click.option(
-    "--include-keywords",
-    type=bool,
-    is_flag=True,
-    default=False,
-    help="Include product keyword details in output",
-)
-@click.option(
-    "--contains",
-    "-c",
-    type=str,
-    multiple=True,
-    help="Filter catalogue output. Returns products with attributes "
-    "matching a string token",
-)
-@click.option(
-    "--overwrite-cache",
-    type=bool,
-    is_flag=True,
-    default=False,
-    help="Force to refresh the catalogue by overwriting the local cache",
-)
-def describe(
-    include_description: bool,
-    include_datasets: bool,
-    include_keywords: bool,
-    one_line: bool,
-    contains: list[str],
-    overwrite_cache: bool,
-) -> None:
-    base_catalogue: CopernicusMarineCatalogue = parse_catalogue(
-        overwrite_cache=overwrite_cache
-    )
-    catalogue: Any
-    if contains:
-        filtered_catalogue = filter_catalogue_with_strings(
-            base_catalogue, contains
-        )
-        catalogue = filtered_catalogue or {}
-    else:
-        catalogue = base_catalogue
-
-    def default_filter(obj):
-        attributes = obj.__dict__
-        if not include_description:
-            attributes.pop("description", None)
-        if not include_datasets:
-            attributes.pop("datasets", None)
-        if not include_keywords:
-            attributes.pop("keywords", None)
-        return obj.__dict__
-
-    json_dump = (
-        dumps(catalogue, default=default_filter, sort_keys=True)
-        if one_line
-        else dumps(catalogue, default=default_filter, sort_keys=True, indent=2)
-    )
-    click.echo(json_dump)
-
-
-if __name__ == "__main__":
-    cli_group_describe()
+import logging
+import logging.config
+from json import dumps
+from typing import Any
+
+import click
+
+from copernicus_marine_client.catalogue_parser.catalogue_parser import (
+    CopernicusMarineCatalogue,
+    filter_catalogue_with_strings,
+    parse_catalogue,
+)
+
+
+@click.group()
+def cli_group_describe() -> None:
+    pass
+
+
+@cli_group_describe.command(
+    "describe",
+    help="""
+    Parse the Copernicus Marine catalogue, then display a
+    JSON-ified version of the corresponding python object.
+
+    The default display contains information on the products, and more data
+    can be displayed using the _include-<argument>_ flags (see Usage section).
+
+    The _contains_ option allows the user to specify one or several strings to
+    filter through the catalogue display. The search is performed recursively
+    on all attributes of the catalogue, and the tokens only need to be
+    contained in one of the attributes (i.e. not exact match).
+
+    Example:
+
+    > copernicus-marine describe --contains METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
+    --include-datasets
+
+    > copernicus-marine describe -c METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
+        """,
+)
+@click.option(
+    "--one-line",
+    type=bool,
+    is_flag=True,
+    default=False,
+    help="Output JSON on one line",
+)
+@click.option(
+    "--include-description",
+    type=bool,
+    is_flag=True,
+    default=False,
+    help="Include product description in output",
+)
+@click.option(
+    "--include-datasets",
+    type=bool,
+    is_flag=True,
+    default=False,
+    help="Include product dataset details in output",
+)
+@click.option(
+    "--include-keywords",
+    type=bool,
+    is_flag=True,
+    default=False,
+    help="Include product keyword details in output",
+)
+@click.option(
+    "--contains",
+    "-c",
+    type=str,
+    multiple=True,
+    help="Filter catalogue output. Returns products with attributes "
+    "matching a string token",
+)
+@click.option(
+    "--overwrite-cache",
+    type=bool,
+    is_flag=True,
+    default=False,
+    help="Force to refresh the catalogue by overwriting the local cache",
+)
+@click.option(
+    "--log-level",
+    type=click.Choice(["DEBUG", "INFO", "WARN", "ERROR", "CRITICAL", "QUIET"]),
+    default="INFO",
+    help=(
+        "Set the details printed to console by the command "
+        "(based on standard logging library)."
+    ),
+)
+def describe(
+    include_description: bool,
+    include_datasets: bool,
+    include_keywords: bool,
+    one_line: bool,
+    contains: list[str],
+    overwrite_cache: bool,
+    log_level: str = "INFO",
+) -> None:
+    if log_level == "QUIET":
+        logging.root.disabled = True
+        logging.root.setLevel(level="CRITICAL")
+    else:
+        logging.root.setLevel(level=log_level)
+    base_catalogue: CopernicusMarineCatalogue = parse_catalogue(
+        overwrite_cache=overwrite_cache
+    )
+    catalogue: Any
+    if contains:
+        filtered_catalogue = filter_catalogue_with_strings(
+            base_catalogue, contains
+        )
+        catalogue = filtered_catalogue or {}
+    else:
+        catalogue = base_catalogue
+
+    def default_filter(obj):
+        attributes = obj.__dict__
+        if not include_description:
+            attributes.pop("description", None)
+        if not include_datasets:
+            attributes.pop("datasets", None)
+        if not include_keywords:
+            attributes.pop("keywords", None)
+        return obj.__dict__
+
+    json_dump = (
+        dumps(catalogue, default=default_filter, sort_keys=True)
+        if one_line
+        else dumps(catalogue, default=default_filter, sort_keys=True, indent=2)
+    )
+    logger = logging.getLogger("blank_logger")
+    logger.warn(json_dump)
+
+
+if __name__ == "__main__":
+    cli_group_describe()
```

### Comparing `copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_ftp.py` & `copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_ftp.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,238 +1,240 @@
-import os
-from ftplib import FTP
-from multiprocessing.pool import ThreadPool
-from typing import Any, Tuple
-
-import click
-from numpy import append, arange
-from tqdm import tqdm
-
-from copernicus_marine_client.catalogue_parser.request_structure import (
-    NativeRequest,
-)
-
-# /////////////////////////////
-# ---Using ftplib
-# /////////////////////////////
-
-
-def download_ftp(
-    login: str,
-    password: str,
-    native_request: NativeRequest,
-) -> str:
-    message, host, filenames_in = download_header(
-        [str(native_request.dataset_url)], login, password
-    )
-    filenames_out = create_filenames_out(
-        filenames_in,
-        native_request.output_directory,
-        native_request.no_directories,
-    )
-    click.echo(message)
-    if native_request.show_outputnames:
-        click.echo("Output filenames:")
-        [click.echo(filename_out) for filename_out in filenames_out]
-    if not native_request.assume_yes:
-        click.confirm("Do you want to continue?", abort=True)
-    pool = ThreadPool()
-    nfiles_per_process, nfiles = 1, len(filenames_in)
-    indexes = append(
-        arange(0, nfiles, nfiles_per_process, dtype=int),
-        nfiles,
-    )
-    groups_in_files = [
-        filenames_in[indexes[i] : indexes[i + 1]]
-        for i in range(len(indexes) - 1)
-    ]
-    groups_out_files = [
-        filenames_out[indexes[i] : indexes[i + 1]]
-        for i in range(len(indexes) - 1)
-    ]
-    download_summary_list = pool.map(
-        download_files,
-        zip(
-            [host] * len(groups_in_files),
-            [login] * len(groups_in_files),
-            [password] * len(groups_in_files),
-            groups_in_files,
-            groups_out_files,
-        ),
-    )
-    download_summary = "".join(map(str, download_summary_list))
-    return download_summary
-
-
-def download_header(
-    data_paths: list[str], login: str, password: str
-) -> Tuple[str, str, list[str]]:
-
-    path_dict = parse_ftp_dataset_url(data_paths)
-    message = "You requested the download of the following files:\n"
-    total_size = 0
-    for host, paths in path_dict.items():
-        with FTP(host) as ftp:
-            ftp.login(user=login, passwd=password)
-            for path in paths:
-                filenames = get_filenames_recursively(ftp, path)
-        pool = ThreadPool()
-        nfilenames_per_process, nfilenames = 100, len(filenames)
-        indexes = append(
-            arange(0, nfilenames, nfilenames_per_process, dtype=int),
-            nfilenames,
-        )
-        groups_filenames = [
-            filenames[indexes[i] : indexes[i + 1]]
-            for i in range(len(indexes) - 1)
-        ]
-        results = pool.map(
-            get_filename_size_tuple,
-            zip(
-                [host] * len(groups_filenames),
-                [login] * len(groups_filenames),
-                [password] * len(groups_filenames),
-                groups_filenames,
-            ),
-        )
-        flattened_results = [r for res in results for r in res]
-        total_size += sum([int(res[1]) for res in flattened_results])
-        for result in flattened_results[:20]:
-            message += str(result[0])
-            message += f" - {format_file_size(float(result[1]))}\n"
-        if len(flattened_results) > 20:
-            message += f"Printed 20 out of {len(flattened_results)} files\n"
-    message += (
-        f"\nTotal size of the download: {format_file_size(total_size)}\n\n"
-    )
-    return (message, host, filenames)
-
-
-def get_filenames_recursively(
-    ftp: FTP, path: str, extensions: list[str] = [".nc"]
-) -> list[str]:
-    if any(extension in path for extension in extensions):
-        # path is a file
-        return [path]
-    elif len(ftp.nlst(path)) == 0:
-        # empty dir
-        return []
-    elif ftp.nlst(path)[0] == path:
-        # path is a file
-        return [path]
-    else:
-        # path is a dir
-        return [
-            filename
-            for element in ftp.nlst(path)
-            for filename in get_filenames_recursively(ftp, element)
-        ]
-
-
-def get_filename_size_tuple(
-    tuple_ftp_filename: Tuple[str, str, str, list[str]]
-) -> list[Tuple[str, Any]]:
-    host, login, password, filenames = tuple_ftp_filename
-    with FTP(host) as ftp:
-        ftp.login(user=login, passwd=password)
-        list_tuples = [
-            (filename, ftp.size(filename)) for filename in filenames
-        ]
-    return list_tuples
-
-
-def download_files(
-    tuple_ftp_filename: Tuple[str, str, str, list[str], list[str]],
-) -> str:
-    def _ftp_file_download(ftp, file_in, file_out):
-        """
-        Download ONE file and return a string of the result
-        """
-        os.makedirs(os.path.dirname(file_out), exist_ok=True)
-        with open(file_out, "wb") as fp:
-            size = ftp.size(file_in)
-            with tqdm(
-                total=size,
-                unit_scale=True,
-                desc=file_in.split("/")[-1],
-            ) as pbar:
-
-                def callback(data):
-                    pbar.update(len(data))
-                    fp.write(data)
-
-                res = ftp.retrbinary(f"RETR {file_in}", callback)
-            if not res.startswith("226 Transfer complete"):
-                print(f"Download {file_in}failed")
-                if os.path.isfile(file_out):
-                    os.remove(file_out)
-                summary_string = f"Could not download {file_in}!\n"
-            else:
-                summary_string = f"File {file_out} created\n"
-        return summary_string
-
-    host, login, password, filenames_in, filenames_out = tuple_ftp_filename
-    download_summary = ""
-    with FTP(host) as ftp:
-        ftp.login(user=login, passwd=password)
-        for file_in, file_out in zip(filenames_in, filenames_out):
-            download_summary += _ftp_file_download(ftp, file_in, file_out)
-    return download_summary
-
-
-# /////////////////////////////
-# --- Tools
-# /////////////////////////////
-
-
-def parse_ftp_dataset_url(data_paths: list[str]) -> dict:
-    path_dict: dict[str, list[str]] = {}
-    for data_path in data_paths:
-        host = data_path[len("ftp://") :].split("/")[0]
-        path = data_path[len("ftp://" + host + "/") :]
-        if host in path_dict.keys():
-            path_dict[host].append(path)
-        else:
-            path_dict[host] = [path]
-    return path_dict
-
-
-def create_filenames_out(
-    filenames_in: list[str], output_directory: str = "", no_directories=False
-) -> list[str]:
-    filenames_out = []
-    for filename_in in filenames_in:
-        filename_out = f"{output_directory}/"
-        if no_directories:
-            filenames_out += [filename_out + filename_in.split("/")[-1]]
-        elif filename_in.startswith("Core/"):
-            filenames_out += [filename_out + filename_in[len("Core/") :]]
-    return filenames_out
-
-
-def format_file_size(
-    size: float, decimals: int = 2, binary_system: bool = False
-) -> str:
-    if binary_system:
-        units: list[str] = [
-            "B",
-            "KiB",
-            "MiB",
-            "GiB",
-            "TiB",
-            "PiB",
-            "EiB",
-            "ZiB",
-        ]
-        largest_unit: str = "YiB"
-        step: int = 1024
-    else:
-        units = ["B", "kB", "MB", "GB", "TB", "PB", "EB", "ZB"]
-        largest_unit = "YB"
-        step = 1000
-
-    for unit in units:
-        if size < step:
-            return ("%." + str(decimals) + "f %s") % (size, unit)
-        size /= step
-
-    return ("%." + str(decimals) + "f %s") % (size, largest_unit)
+import logging
+import os
+from ftplib import FTP
+from multiprocessing.pool import ThreadPool
+from typing import Any, Tuple
+
+import click
+from numpy import append, arange
+from tqdm import tqdm
+
+from copernicus_marine_client.catalogue_parser.request_structure import (
+    NativeRequest,
+)
+
+# /////////////////////////////
+# ---Using ftplib
+# /////////////////////////////
+
+
+def download_ftp(
+    username: str,
+    password: str,
+    native_request: NativeRequest,
+) -> str:
+    message, host, filenames_in = download_header(
+        [str(native_request.dataset_url)], username, password
+    )
+    filenames_out = create_filenames_out(
+        filenames_in,
+        native_request.output_directory,
+        native_request.no_directories,
+    )
+    logging.info(message)
+    if native_request.show_outputnames:
+        logging.info("Output filenames:")
+        for filename_out in filenames_out:
+            logging.info(filename_out)
+    if not native_request.assume_yes:
+        click.confirm("Do you want to continue?", abort=True)
+    pool = ThreadPool()
+    nfiles_per_process, nfiles = 1, len(filenames_in)
+    indexes = append(
+        arange(0, nfiles, nfiles_per_process, dtype=int),
+        nfiles,
+    )
+    groups_in_files = [
+        filenames_in[indexes[i] : indexes[i + 1]]
+        for i in range(len(indexes) - 1)
+    ]
+    groups_out_files = [
+        filenames_out[indexes[i] : indexes[i + 1]]
+        for i in range(len(indexes) - 1)
+    ]
+    download_summary_list = pool.map(
+        download_files,
+        zip(
+            [host] * len(groups_in_files),
+            [username] * len(groups_in_files),
+            [password] * len(groups_in_files),
+            groups_in_files,
+            groups_out_files,
+        ),
+    )
+    download_summary = "".join(map(str, download_summary_list))
+    return download_summary
+
+
+def download_header(
+    data_paths: list[str], username: str, password: str
+) -> Tuple[str, str, list[str]]:
+
+    path_dict = parse_ftp_dataset_url(data_paths)
+    message = "You requested the download of the following files:\n"
+    total_size = 0
+    for host, paths in path_dict.items():
+        with FTP(host) as ftp:
+            ftp.login(user=username, passwd=password)
+            for path in paths:
+                filenames = get_filenames_recursively(ftp, path)
+        pool = ThreadPool()
+        nfilenames_per_process, nfilenames = 100, len(filenames)
+        indexes = append(
+            arange(0, nfilenames, nfilenames_per_process, dtype=int),
+            nfilenames,
+        )
+        groups_filenames = [
+            filenames[indexes[i] : indexes[i + 1]]
+            for i in range(len(indexes) - 1)
+        ]
+        results = pool.map(
+            get_filename_size_tuple,
+            zip(
+                [host] * len(groups_filenames),
+                [username] * len(groups_filenames),
+                [password] * len(groups_filenames),
+                groups_filenames,
+            ),
+        )
+        flattened_results = [r for res in results for r in res]
+        total_size += sum([int(res[1]) for res in flattened_results])
+        for result in flattened_results[:20]:
+            message += str(result[0])
+            message += f" - {format_file_size(float(result[1]))}\n"
+        if len(flattened_results) > 20:
+            message += f"Printed 20 out of {len(flattened_results)} files\n"
+    message += (
+        f"\nTotal size of the download: {format_file_size(total_size)}\n\n"
+    )
+    return (message, host, filenames)
+
+
+def get_filenames_recursively(
+    ftp: FTP, path: str, extensions: list[str] = [".nc"]
+) -> list[str]:
+    if any(extension in path for extension in extensions):
+        # path is a file
+        return [path]
+    elif len(ftp.nlst(path)) == 0:
+        # empty dir
+        return []
+    elif ftp.nlst(path)[0] == path:
+        # path is a file
+        return [path]
+    else:
+        # path is a dir
+        return [
+            filename
+            for element in ftp.nlst(path)
+            for filename in get_filenames_recursively(ftp, element)
+        ]
+
+
+def get_filename_size_tuple(
+    tuple_ftp_filename: Tuple[str, str, str, list[str]]
+) -> list[Tuple[str, Any]]:
+    host, username, password, filenames = tuple_ftp_filename
+    with FTP(host) as ftp:
+        ftp.login(user=username, passwd=password)
+        list_tuples = [
+            (filename, ftp.size(filename)) for filename in filenames
+        ]
+    return list_tuples
+
+
+def download_files(
+    tuple_ftp_filename: Tuple[str, str, str, list[str], list[str]],
+) -> str:
+    def _ftp_file_download(ftp, file_in, file_out):
+        """
+        Download ONE file and return a string of the result
+        """
+        os.makedirs(os.path.dirname(file_out), exist_ok=True)
+        with open(file_out, "wb") as fp:
+            size = ftp.size(file_in)
+            with tqdm(
+                total=size,
+                unit_scale=True,
+                desc=file_in.split("/")[-1],
+            ) as pbar:
+
+                def callback(data):
+                    pbar.update(len(data))
+                    fp.write(data)
+
+                res = ftp.retrbinary(f"RETR {file_in}", callback)
+            if not res.startswith("226 Transfer complete"):
+                logging.error(f"Download {file_in} failed")
+                if os.path.isfile(file_out):
+                    os.remove(file_out)
+                summary_string = f"Could not download {file_in}!\n"
+            else:
+                summary_string = f"File {file_out} created\n"
+        return summary_string
+
+    host, username, password, filenames_in, filenames_out = tuple_ftp_filename
+    download_summary = ""
+    with FTP(host) as ftp:
+        ftp.login(user=username, passwd=password)
+        for file_in, file_out in zip(filenames_in, filenames_out):
+            download_summary += _ftp_file_download(ftp, file_in, file_out)
+    return download_summary
+
+
+# /////////////////////////////
+# --- Tools
+# /////////////////////////////
+
+
+def parse_ftp_dataset_url(data_paths: list[str]) -> dict:
+    path_dict: dict[str, list[str]] = {}
+    for data_path in data_paths:
+        host = data_path[len("ftp://") :].split("/")[0]
+        path = data_path[len("ftp://" + host + "/") :]
+        if host in path_dict.keys():
+            path_dict[host].append(path)
+        else:
+            path_dict[host] = [path]
+    return path_dict
+
+
+def create_filenames_out(
+    filenames_in: list[str], output_directory: str = "", no_directories=False
+) -> list[str]:
+    filenames_out = []
+    for filename_in in filenames_in:
+        filename_out = f"{output_directory}/"
+        if no_directories:
+            filenames_out += [filename_out + filename_in.split("/")[-1]]
+        elif filename_in.startswith("Core/"):
+            filenames_out += [filename_out + filename_in[len("Core/") :]]
+    return filenames_out
+
+
+def format_file_size(
+    size: float, decimals: int = 2, binary_system: bool = False
+) -> str:
+    if binary_system:
+        units: list[str] = [
+            "B",
+            "KiB",
+            "MiB",
+            "GiB",
+            "TiB",
+            "PiB",
+            "EiB",
+            "ZiB",
+        ]
+        largest_unit: str = "YiB"
+        step: int = 1024
+    else:
+        units = ["B", "kB", "MB", "GB", "TB", "PB", "EB", "ZB"]
+        largest_unit = "YB"
+        step = 1000
+
+    for unit in units:
+        if size < step:
+            return ("%." + str(decimals) + "f %s") % (size, unit)
+        size /= step
+
+    return ("%." + str(decimals) + "f %s") % (size, largest_unit)
```

### Comparing `copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_s3native.py` & `copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_s3native.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,223 +1,205 @@
-import os
-import subprocess
-from multiprocessing.pool import ThreadPool
-from subprocess import CompletedProcess
-from typing import Tuple
-
-import click
-from numpy import append, arange
-from tqdm import tqdm
-
-from copernicus_marine_client.catalogue_parser.request_structure import (
-    NativeRequest,
-)
-
-
-def download_s3native(
-    login: str,
-    password: str,
-    native_request: NativeRequest,
-) -> str:
-    message, endpoint_url, filenames_in = download_header(
-        [str(native_request.dataset_url)], login, password
-    )
-    filenames_out = create_filenames_out(
-        filenames_in,
-        native_request.output_directory,
-        native_request.no_directories,
-    )
-    click.echo(message)
-    if native_request.show_outputnames:
-        click.echo("Output filenames:")
-        [click.echo(filename_out) for filename_out in filenames_out]
-    if not native_request.assume_yes:
-        click.confirm("Do you want to continue?", abort=True)
-    pool = ThreadPool()
-    nfiles_per_process, nfiles = 1, len(filenames_in)
-    indexes = append(
-        arange(0, nfiles, nfiles_per_process, dtype=int),
-        nfiles,
-    )
-    groups_in_files = [
-        filenames_in[indexes[i] : indexes[i + 1]]
-        for i in range(len(indexes) - 1)
-    ]
-    groups_out_files = [
-        filenames_out[indexes[i] : indexes[i + 1]]
-        for i in range(len(indexes) - 1)
-    ]
-    download_summary_list = pool.map(
-        download_files,
-        zip(
-            [endpoint_url] * len(groups_in_files),
-            groups_in_files,
-            groups_out_files,
-        ),
-    )
-    download_summary = "".join(map(str, download_summary_list))
-    return download_summary
-
-
-def download_header(
-    data_paths: list[str], login: str, password: str
-) -> Tuple[str, str, list[str]]:
-
-    path_dict = parse_s3native_dataset_url(data_paths)
-    message = "You requested the download of the following files:\n"
-    filenames, sizes, total_size = [], [], 0.0
-    for endpoint_url, paths in path_dict.items():
-        for path in paths:
-            files_name_size = get_filenames_recursively(endpoint_url, path)
-            for filename, size in files_name_size:
-                filenames += [filename]
-                sizes += [float(size)]
-                total_size += float(size)
-    for filename, size in files_name_size[:20]:
-        message += str(filename)
-        message += f" - {format_file_size(float(size))}\n"
-        if len(filenames) > 20:
-            message += f"Printed 20 out of {len(filenames)} files\n"
-    message += (
-        f"\nTotal size of the download: {format_file_size(total_size)}\n\n"
-    )
-    return (message, endpoint_url, filenames)
-
-
-def get_filenames_recursively(
-    endpoint_url: str,
-    path: str,
-    files_already_found: list[tuple[str, str]] = [],
-) -> list[tuple[str, str]]:
-    if not path.endswith("/"):
-        path += "/"
-    path_to_s5cmd_exe = os.path.join(os.path.dirname(__file__), r".\s5cmd.exe")
-    bash_command: str = (
-        f"{path_to_s5cmd_exe} --endpoint-url {endpoint_url}"
-        f" --no-sign-request ls {path}"
-    )
-    raw_output: CompletedProcess[bytes] = subprocess.run(
-        bash_command, shell=True, capture_output=True
-    )
-    cleaned_output: str = raw_output.stdout.decode("utf-8").strip()
-    lines: list[str] = [
-        substr.strip() for substr in cleaned_output.split("\n")
-    ]
-    for line in lines:
-        if not line:
-            pass
-        elif line.startswith("DIR"):
-            files_already_found.extend(
-                get_filenames_recursively(
-                    endpoint_url, path + line.split(" ")[-1].strip(), []
-                )
-            )
-        elif line.endswith(".nc"):
-            files_already_found.extend(
-                [
-                    (
-                        path + line.split(" ")[-1].split("/")[-1],
-                        line.split(" ")[-2],
-                    )
-                ]
-            )
-        else:
-            raise ValueError(f"Unable to handle line: {line}")
-    return files_already_found
-
-
-def download_files(
-    tuple_s3native_filename: Tuple[str, list[str], list[str]],
-) -> str:
-    def _s3native_file_download(
-        endpoint_url: str, file_in: str, file_out: str
-    ) -> str:
-        """
-        Download ONE file and return a string of the result
-        """
-        path_to_s5cmd_exe = os.path.join(
-            os.path.dirname(__file__), r".\s5cmd.exe"
-        )
-        bash_command = (
-            f"{path_to_s5cmd_exe} --endpoint-url {endpoint_url} --no-sign-request "
-            f"cp --no-clobber {file_in} {file_out}"
-        )
-        with tqdm(desc=file_in.split("/")[-1]) as t:
-            """
-            Comment: for now s5cmd does not seem to have a way to display progress
-            (see https://github.com/peak/s5cmd/issues/51)
-            """
-            raw_output: CompletedProcess[bytes] = subprocess.run(
-                bash_command, shell=True, capture_output=True
-            )
-            t.update()
-        if not raw_output.stdout.decode("utf-8"):
-            summary_string = f"File {file_out} already exists\n"
-        else:
-            summary_string = f"File {file_out} created\n"
-        return summary_string
-
-    endpoint_url, filenames_in, filenames_out = tuple_s3native_filename
-    download_summary = ""
-    for file_in, file_out in zip(filenames_in, filenames_out):
-        download_summary += _s3native_file_download(
-            endpoint_url, file_in, file_out
-        )
-    return download_summary
-
-
-# /////////////////////////////
-# --- Tools
-# /////////////////////////////
-
-
-def parse_s3native_dataset_url(data_paths: list[str]) -> dict:
-    path_dict: dict[str, list[str]] = {}
-    for data_path in data_paths:
-        endpoint_url, path = data_path.split("/mdl-native/", maxsplit=1)
-        path = "s3://mdl-native/" + path
-        path_dict.setdefault(endpoint_url, []).append(path)
-    return path_dict
-
-
-def create_filenames_out(
-    filenames_in: list[str], output_directory: str = "", no_directories=False
-) -> list[str]:
-    filenames_out = []
-    for filename_in in filenames_in:
-        filename_out = f"{output_directory}/"
-        if no_directories:
-            filenames_out += [filename_out + filename_in.split("/")[-1]]
-        elif filename_in.startswith("s3://mdl-native/native/"):
-            filenames_out += [
-                filename_out + filename_in[len("s3://mdl-native/native/") :]
-            ]
-    return filenames_out
-
-
-def format_file_size(
-    size: float, decimals: int = 2, binary_system: bool = False
-) -> str:
-    if binary_system:
-        units: list[str] = [
-            "B",
-            "KiB",
-            "MiB",
-            "GiB",
-            "TiB",
-            "PiB",
-            "EiB",
-            "ZiB",
-        ]
-        largest_unit: str = "YiB"
-        step: int = 1024
-    else:
-        units = ["B", "kB", "MB", "GB", "TB", "PB", "EB", "ZB"]
-        largest_unit = "YB"
-        step = 1000
-
-    for unit in units:
-        if size < step:
-            return ("%." + str(decimals) + "f %s") % (size, unit)
-        size /= step
-
-    return ("%." + str(decimals) + "f %s") % (size, largest_unit)
+import logging
+from multiprocessing.pool import ThreadPool
+from typing import Tuple
+
+import click
+import s3fs
+from numpy import append, arange
+from tqdm import tqdm
+
+from copernicus_marine_client.catalogue_parser.request_structure import (
+    NativeRequest,
+)
+
+
+def download_s3native(
+    username: str,
+    password: str,
+    native_request: NativeRequest,
+) -> str:
+    message, endpoint_url, filenames_in = download_header(
+        [str(native_request.dataset_url)], username, password
+    )
+    filenames_out = create_filenames_out(
+        filenames_in,
+        native_request.output_directory,
+        native_request.no_directories,
+    )
+    logging.info(message)
+    if native_request.show_outputnames:
+        logging.info("Output filenames:")
+        for filename_out in filenames_out:
+            logging.info(filename_out)
+    if not native_request.assume_yes:
+        click.confirm("Do you want to continue?", abort=True)
+    pool = ThreadPool()
+    nfiles_per_process, nfiles = 1, len(filenames_in)
+    indexes = append(
+        arange(0, nfiles, nfiles_per_process, dtype=int),
+        nfiles,
+    )
+    groups_in_files = [
+        filenames_in[indexes[i] : indexes[i + 1]]
+        for i in range(len(indexes) - 1)
+    ]
+    groups_out_files = [
+        filenames_out[indexes[i] : indexes[i + 1]]
+        for i in range(len(indexes) - 1)
+    ]
+    download_summary_list = pool.imap(
+        download_files,
+        zip(
+            [endpoint_url] * len(groups_in_files),
+            groups_in_files,
+            groups_out_files,
+        ),
+    )
+    list(tqdm(download_summary_list, total=len(groups_in_files)))
+    download_summary = "Download complete"
+    return download_summary
+
+
+def download_header(
+    data_paths: list[str], username: str, password: str
+) -> Tuple[str, str, list[str]]:
+    path_dict = parse_s3native_dataset_url(data_paths)
+    message = "You requested the download of the following files:\n"
+    filenames, sizes, total_size = [], [], 0.0
+    for endpoint_url, paths in path_dict.items():
+        for path in paths:
+            files_name_size = get_filenames_recursively(endpoint_url, path)
+            for filename, size in files_name_size:
+                filenames += [filename]
+                sizes += [float(size)]
+                total_size += float(size)
+    for filename, size in files_name_size[:20]:
+        message += str(filename)
+        message += f" - {format_file_size(float(size))}\n"
+    if len(filenames) > 20:
+        message += f"Printed 20 out of {len(filenames)} files\n"
+    message += (
+        f"\nTotal size of the download: {format_file_size(total_size)}\n\n"
+    )
+    return (message, endpoint_url, filenames)
+
+
+def get_filenames_recursively(
+    endpoint_url: str,
+    path: str,
+    files_already_found: list[tuple[str, int]] = [],
+) -> list[tuple[str, int]]:
+    if not path.endswith("/"):
+        path += "/"
+
+    s3: s3fs.S3FileSystem = s3fs.S3FileSystem(
+        anon=True, endpoint_url=endpoint_url
+    )
+    objects_at_path = s3.ls(path, detail=True)
+
+    for object_at_path in objects_at_path:
+        if object_at_path["type"] == "directory":
+            files_already_found.extend(
+                get_filenames_recursively(
+                    endpoint_url, object_at_path["name"], []
+                )
+            )
+        elif object_at_path["type"] == "file" and object_at_path[
+            "name"
+        ].endswith(".nc"):
+            files_already_found.extend(
+                [
+                    (
+                        "s3://" + object_at_path["name"],
+                        object_at_path["size"],
+                    )
+                ]
+            )
+        else:
+            value_error = ValueError(
+                f"Unable to handle line: {object_at_path['name']}"
+            )
+            logging.error(value_error)
+            raise value_error
+    return files_already_found
+
+
+def download_files(
+    tuple_s3native_filename: Tuple[str, list[str], list[str]],
+) -> str:
+    def _s3native_file_download(
+        endpoint_url: str, file_in: str, file_out: str
+    ) -> str:
+        """
+        Download ONE file and return a string of the result
+        """
+        s3: s3fs.S3FileSystem = s3fs.S3FileSystem(
+            anon=True, endpoint_url=endpoint_url
+        )
+        s3.download(file_in, file_out)
+        return f"File {file_out} created\n"
+
+    endpoint_url, filenames_in, filenames_out = tuple_s3native_filename
+    download_summary = ""
+    for file_in, file_out in zip(filenames_in, filenames_out):
+        download_summary += _s3native_file_download(
+            endpoint_url, file_in, file_out
+        )
+    return download_summary
+
+
+# /////////////////////////////
+# --- Tools
+# /////////////////////////////
+
+
+def parse_s3native_dataset_url(data_paths: list[str]) -> dict:
+    path_dict: dict[str, list[str]] = {}
+    for data_path in data_paths:
+        endpoint_url, path = data_path.split("/mdl-native/", maxsplit=1)
+        path = "s3://mdl-native/" + path
+        path_dict.setdefault(endpoint_url, []).append(path)
+    return path_dict
+
+
+def create_filenames_out(
+    filenames_in: list[str], output_directory: str = "", no_directories=False
+) -> list[str]:
+    filenames_out = []
+    for filename_in in filenames_in:
+        filename_out = f"{output_directory}/"
+        if no_directories:
+            filenames_out += [filename_out + filename_in.split("/")[-1]]
+        elif filename_in.startswith("s3://mdl-native/native/"):
+            filenames_out += [
+                filename_out + filename_in[len("s3://mdl-native/native/") :]
+            ]
+    return filenames_out
+
+
+def format_file_size(
+    size: float, decimals: int = 2, binary_system: bool = False
+) -> str:
+    if binary_system:
+        units: list[str] = [
+            "B",
+            "KiB",
+            "MiB",
+            "GiB",
+            "TiB",
+            "PiB",
+            "EiB",
+            "ZiB",
+        ]
+        largest_unit: str = "YiB"
+        step: int = 1024
+    else:
+        units = ["B", "kB", "MB", "GB", "TB", "PB", "EB", "ZB"]
+        largest_unit = "YB"
+        step = 1000
+
+    for unit in units:
+        if size < step:
+            return ("%." + str(decimals) + "f %s") % (size, unit)
+        size /= step
+
+    return ("%." + str(decimals) + "f %s") % (size, largest_unit)
```

### Comparing `copernicus_marine_client-0.7.1/copernicus_marine_client/download_functions/download_zarr.py` & `copernicus_marine_client-0.8.0/copernicus_marine_client/download_functions/download_zarr.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,200 +1,206 @@
-from datetime import datetime
-from os import path
-from typing import List, Optional, Tuple
-
-import click
-import numpy as np
-import xarray as xr
-import zarr
-
-from copernicus_marine_client.catalogue_parser.request_structure import (
-    SubsetRequest,
-)
-
-
-def subset(
-    ds,
-    variables: Optional[List[str]] = None,
-    geographical_subset: Optional[
-        Tuple[
-            Optional[float], Optional[float], Optional[float], Optional[float]
-        ]
-    ] = None,
-    temporal_subset: Optional[
-        Tuple[Optional[datetime], Optional[datetime]]
-    ] = None,
-    depth_range: Optional[Tuple[Optional[float], Optional[float]]] = None,
-) -> xr.Dataset:
-
-    if variables:
-        ds = ds[np.array(variables)]
-
-    if geographical_subset:
-        (
-            minimal_latitude,
-            maximal_latitude,
-            minimal_longitude,
-            maximal_longitude,
-        ) = geographical_subset
-        if ("latitude" in ds.coords) and any(geographical_subset):
-            ds = ds.sel(
-                latitude=slice(minimal_latitude, maximal_latitude),
-                longitude=slice(minimal_longitude, maximal_longitude),
-            )
-        elif ("nav_lat" in ds.coords) and any(geographical_subset):
-            mask = (
-                (ds.nav_lon > minimal_longitude)
-                & (ds.nav_lon < maximal_longitude)
-                & (ds.nav_lat > minimal_latitude)
-                & (ds.nav_lat < maximal_latitude)
-            )
-            geoindex = np.argwhere(mask.values)
-            xmin = min(geoindex[:, 1])
-            xmax = max(geoindex[:, 1])
-            ymin = min(geoindex[:, 0])
-            ymax = max(geoindex[:, 0])
-
-            ds = ds.isel(
-                x=slice(xmin, xmax),
-                y=slice(ymin, ymax),
-            )
-        else:
-            ds = ds.sel(
-                lat=slice(minimal_latitude, maximal_latitude),
-                lon=slice(minimal_longitude, maximal_longitude),
-            )
-
-    if temporal_subset:
-        (start_datetime, end_datetime) = temporal_subset
-        if "time_counter" in ds.coords:
-            ds = ds.sel(time_counter=slice(start_datetime, end_datetime))
-        else:
-            ds = ds.sel(time=slice(start_datetime, end_datetime))
-
-    if (("depth" in ds.dims) or ("deptht" in ds.dims)) and (
-        depth_range is not None and any(depth_range)
-    ):
-        (
-            minimal_depth,
-            maximal_depth,
-        ) = depth_range
-        if "deptht" in ds.dims:
-            ds = ds.sel(deptht=slice(minimal_depth, maximal_depth))
-        else:
-            ds = ds.sel(depth=slice(minimal_depth, maximal_depth))
-    elif ("elevation" in ds.dims) and (
-        depth_range is not None and any(depth_range)
-    ):
-        (
-            minimal_depth,
-            maximal_depth,
-        ) = depth_range
-        minimal_depth = minimal_depth * -1.0 if minimal_depth else None
-        maximal_depth = maximal_depth * -1.0 if maximal_depth else None
-        ds = ds.sel(elevation=slice(maximal_depth, minimal_depth))
-
-    return ds
-
-
-def get_optimized_chunking(subset_request: SubsetRequest) -> str:
-    """Function to calculate the optimized type of chunking,
-    based on a subset_request.
-    Returns a str: "map" if time-chunking is optimized,
-    "timeserie" if geo-chunking is optimized
-    """
-    print(
-        "WARNING: THIS CHUNKING OPTIMIZATION FUNCTION IS "
-        + "A PLACEHOLDER, DO NOT RELY ON IT!!"
-    )
-    chunking_selected = "map"
-    if (
-        isinstance(subset_request.minimal_latitude, float)
-        and isinstance(subset_request.maximal_latitude, float)
-        and isinstance(subset_request.minimal_longitude, float)
-        and isinstance(subset_request.maximal_longitude, float)
-    ):
-        surface = abs(
-            subset_request.maximal_longitude - subset_request.minimal_longitude
-        ) * abs(
-            subset_request.maximal_latitude - subset_request.minimal_latitude
-        )
-
-        if surface < 20:
-            chunking_selected = "timeserie"
-    return chunking_selected
-
-
-def download_dataset(
-    login: str,
-    password: str,
-    geographical_subset: Optional[
-        tuple[
-            Optional[float], Optional[float], Optional[float], Optional[float]
-        ]
-    ],
-    temporal_subset: Optional[tuple[Optional[datetime], Optional[datetime]]],
-    depth_range: Optional[tuple[Optional[float], Optional[float]]],
-    dataset_url: str,
-    output_directory: str,
-    output_filename: str,
-    variables: Optional[list[str]],
-    assume_yes: bool = False,
-):
-
-    dataset = xr.open_zarr(dataset_url)
-    dataset = subset(
-        dataset, variables, geographical_subset, temporal_subset, depth_range
-    )
-
-    if not assume_yes:
-        print(dataset)
-        click.confirm("Do you want to continue?", abort=True, default=True)
-
-    store = zarr.DirectoryStore(path.join(output_directory, output_filename))
-    dataset.to_zarr(store)
-
-
-def download_zarr(
-    login: str,
-    password: str,
-    subset_request: SubsetRequest,
-):
-
-    geographical_subset = (
-        subset_request.minimal_latitude,
-        subset_request.maximal_latitude,
-        subset_request.minimal_longitude,
-        subset_request.maximal_longitude,
-    )
-    temporal_subset = (
-        subset_request.start_datetime,
-        subset_request.end_datetime,
-    )
-    depth_range = (subset_request.minimal_depth, subset_request.maximal_depth)
-    dataset_url = str(subset_request.dataset_url)
-    output_directory = (
-        subset_request.output_directory
-        if subset_request.output_directory
-        else "."
-    )
-    output_filename = (
-        subset_request.output_filename
-        if subset_request.output_filename
-        else "data.zarr"
-    )
-    variables = subset_request.variables
-    assume_yes = subset_request.assume_yes
-
-    download_dataset(
-        login=login,
-        password=password,
-        geographical_subset=geographical_subset,
-        temporal_subset=temporal_subset,
-        depth_range=depth_range,
-        dataset_url=dataset_url,
-        output_directory=output_directory,
-        output_filename=output_filename,
-        variables=variables,
-        assume_yes=assume_yes,
-    )
-    return path.join(output_directory, output_filename)
+import logging
+from datetime import datetime
+from os import path
+from typing import List, Optional, Tuple
+
+import click
+import numpy as np
+import xarray as xr
+import zarr
+
+from copernicus_marine_client.catalogue_parser.request_structure import (
+    SubsetRequest,
+)
+
+
+def subset(
+    ds,
+    variables: Optional[List[str]] = None,
+    geographical_subset: Optional[
+        Tuple[
+            Optional[float], Optional[float], Optional[float], Optional[float]
+        ]
+    ] = None,
+    temporal_subset: Optional[
+        Tuple[Optional[datetime], Optional[datetime]]
+    ] = None,
+    depth_range: Optional[Tuple[Optional[float], Optional[float]]] = None,
+) -> xr.Dataset:
+
+    if variables:
+        ds = ds[np.array(variables)]
+
+    if geographical_subset:
+        (
+            minimal_latitude,
+            maximal_latitude,
+            minimal_longitude,
+            maximal_longitude,
+        ) = geographical_subset
+        if ("latitude" in ds.coords) and any(geographical_subset):
+            ds = ds.sel(
+                latitude=slice(minimal_latitude, maximal_latitude),
+                longitude=slice(minimal_longitude, maximal_longitude),
+            )
+        elif ("nav_lat" in ds.coords) and any(geographical_subset):
+            mask = (
+                (ds.nav_lon > minimal_longitude)
+                & (ds.nav_lon < maximal_longitude)
+                & (ds.nav_lat > minimal_latitude)
+                & (ds.nav_lat < maximal_latitude)
+            )
+            geoindex = np.argwhere(mask.values)
+            xmin = min(geoindex[:, 1])
+            xmax = max(geoindex[:, 1])
+            ymin = min(geoindex[:, 0])
+            ymax = max(geoindex[:, 0])
+
+            ds = ds.isel(
+                x=slice(xmin, xmax),
+                y=slice(ymin, ymax),
+            )
+        else:
+            ds = ds.sel(
+                lat=slice(minimal_latitude, maximal_latitude),
+                lon=slice(minimal_longitude, maximal_longitude),
+            )
+
+    if temporal_subset:
+        (start_datetime, end_datetime) = temporal_subset
+        if "time_counter" in ds.coords:
+            ds = ds.sel(time_counter=slice(start_datetime, end_datetime))
+        else:
+            ds = ds.sel(time=slice(start_datetime, end_datetime))
+
+    if (("depth" in ds.dims) or ("deptht" in ds.dims)) and (
+        depth_range is not None and any(depth_range)
+    ):
+        (
+            minimal_depth,
+            maximal_depth,
+        ) = depth_range
+        if "deptht" in ds.dims:
+            ds = ds.sel(deptht=slice(minimal_depth, maximal_depth))
+        else:
+            ds = ds.sel(depth=slice(minimal_depth, maximal_depth))
+    elif ("elevation" in ds.dims) and (
+        depth_range is not None and any(depth_range)
+    ):
+        (
+            minimal_depth,
+            maximal_depth,
+        ) = depth_range
+        minimal_depth = minimal_depth * -1.0 if minimal_depth else None
+        maximal_depth = maximal_depth * -1.0 if maximal_depth else None
+        ds = ds.sel(elevation=slice(maximal_depth, minimal_depth))
+
+    return ds
+
+
+def get_optimized_chunking(subset_request: SubsetRequest) -> str:
+    """Function to calculate the optimized type of chunking,
+    based on a subset_request.
+    Returns a str: "map" if time-chunking is optimized,
+    "timeserie" if geo-chunking is optimized
+    """
+    logging.info(
+        "THIS CHUNKING OPTIMIZATION FUNCTION IS "
+        + "A PLACEHOLDER, DO NOT RELY ON IT!!"
+    )
+    chunking_selected = "map"
+    if (
+        isinstance(subset_request.minimal_latitude, float)
+        and isinstance(subset_request.maximal_latitude, float)
+        and isinstance(subset_request.minimal_longitude, float)
+        and isinstance(subset_request.maximal_longitude, float)
+    ):
+        surface = abs(
+            subset_request.maximal_longitude - subset_request.minimal_longitude
+        ) * abs(
+            subset_request.maximal_latitude - subset_request.minimal_latitude
+        )
+
+        if surface < 20:
+            chunking_selected = "timeserie"
+    return chunking_selected
+
+
+def download_dataset(
+    username: str,
+    password: str,
+    geographical_subset: Optional[
+        tuple[
+            Optional[float], Optional[float], Optional[float], Optional[float]
+        ]
+    ],
+    temporal_subset: Optional[tuple[Optional[datetime], Optional[datetime]]],
+    depth_range: Optional[tuple[Optional[float], Optional[float]]],
+    dataset_url: str,
+    output_directory: str,
+    output_filename: str,
+    variables: Optional[list[str]],
+    assume_yes: bool = False,
+):
+
+    dataset = xr.open_zarr(dataset_url)
+    dataset = subset(
+        dataset, variables, geographical_subset, temporal_subset, depth_range
+    )
+    dataset = dataset.chunk(chunks="auto")
+
+    if not assume_yes:
+        logger = logging.getLogger("blank_logger")
+        logger.warn(dataset)
+        click.confirm("Do you want to continue?", abort=True, default=True)
+
+    store = zarr.DirectoryStore(path.join(output_directory, output_filename))
+    dataset.to_zarr(store)
+    logging.info(
+        f"Successfully downloaded to {path.join(output_directory, output_filename)}"
+    )
+
+
+def download_zarr(
+    username: str,
+    password: str,
+    subset_request: SubsetRequest,
+):
+
+    geographical_subset = (
+        subset_request.minimal_latitude,
+        subset_request.maximal_latitude,
+        subset_request.minimal_longitude,
+        subset_request.maximal_longitude,
+    )
+    temporal_subset = (
+        subset_request.start_datetime,
+        subset_request.end_datetime,
+    )
+    depth_range = (subset_request.minimal_depth, subset_request.maximal_depth)
+    dataset_url = str(subset_request.dataset_url)
+    output_directory = (
+        subset_request.output_directory
+        if subset_request.output_directory
+        else "."
+    )
+    output_filename = (
+        subset_request.output_filename
+        if subset_request.output_filename
+        else "data.zarr"
+    )
+    variables = subset_request.variables
+    assume_yes = subset_request.assume_yes
+
+    download_dataset(
+        username=username,
+        password=password,
+        geographical_subset=geographical_subset,
+        temporal_subset=temporal_subset,
+        depth_range=depth_range,
+        dataset_url=dataset_url,
+        output_directory=output_directory,
+        output_filename=output_filename,
+        variables=variables,
+        assume_yes=assume_yes,
+    )
+    return path.join(output_directory, output_filename)
```

### Comparing `copernicus_marine_client-0.7.1/pyproject.toml` & `copernicus_marine_client-0.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-[tool.poetry]
-name = "copernicus-marine-client"
-version = "0.7.1"
-description = ""
-authors = ["jsouchard <jsouchard@mercator-ocean.fr>"]
-readme = "README.md"
-packages = [{include = "copernicus_marine_client"}]
-
-[tool.poetry.dependencies]
-python = ">=3.9"
-owslib = ">=0.27.2"
-click = ">=8.0.4"
-numpy = ">=1.0"
-requests = ">=2.27.1"
-aiohttp = ">=3.8.3"
-setuptools = ">=62.0.0"
-motuclient = "1.8.4"
-cachier = ">=2.0.2"
-pystac = ">=1.7.2"
-xarray = ">=2023.3.0"
-tqdm = ">=4.65.0"
-zarr = ">=2.13.3"
-pydap = ">=3.2.2"
-dask = ">=2022.1.1"
-netCDF4 = ">=1.6.3"
-
-[tool.poetry.dev-dependencies]
-pre-commit = "2.20.0"
-types-requests = "2.27.11"
-
-[tool.poetry.scripts]
-copernicus-marine = 'copernicus_marine_client.command_line_interface.copernicus_marine:command_line_interface'
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "copernicus-marine-client"
+version = "0.8.0"
+description = ""
+authors = ["jsouchard <jsouchard@mercator-ocean.fr>"]
+readme = "README.md"
+packages = [{include = "copernicus_marine_client"}]
+
+[tool.poetry.dependencies]
+python = ">=3.9"
+owslib = ">=0.27.2"
+click = ">=8.0.4"
+numpy = ">=1.0"
+requests = ">=2.27.1"
+aiohttp = ">=3.8.3"
+setuptools = ">=62.0.0"
+motuclient = "1.8.4"
+cachier = ">=2.0.2"
+pystac = ">=1.7.2"
+xarray = ">=2023.3.0"
+tqdm = ">=4.65.0"
+zarr = ">=2.13.3"
+pydap = ">=3.2.2"
+dask = ">=2022.1.1"
+netCDF4 = ">=1.6.3"
+s3fs = "^2023.6.0"
+
+[tool.poetry.dev-dependencies]
+pre-commit = "2.20.0"
+types-requests = "2.27.11"
+
+[tool.poetry.scripts]
+copernicus-marine = 'copernicus_marine_client.command_line_interface.copernicus_marine:command_line_interface'
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `copernicus_marine_client-0.7.1/README.md` & `copernicus_marine_client-0.8.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,341 +1,418 @@
-# Copernicus Marine Service client
-
-A library to facilitate the access of Copernicus Marine Service products and datasets.
-
-## Introduction
-
-This package allows to recover products and datasets information from Command Line Interface or with Python code,
-as well as download subsets and native files.
-
-## Command Line Interface (CLI)
-
-### Command *describe*
-Retrieve information about products as JSON:
-
-```
-> copernicus-marine describe
-{
-  "products": [
-    {
-      "title": "Antarctic Sea Ice Extent from Reanalysis",
-      "product_id": "ANTARCTIC_OMI_SI_extent",
-      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",
-      "production_center": "Mercator Oc\u00e9an International",
-      "creation_datetime": "2018-02-12",
-      "modified_datetime": "2018-02-12",
-    }
-    ...
-  ]
-}
-```
-
-Retrieve all information about datasets as JSON:
-
-```
-> copernicus-marine describe --include-datasets
-{
-  "products": [
-    {
-      "title": "Antarctic Sea Ice Extent from Reanalysis",
-      "product_id": "ANTARCTIC_OMI_SI_extent",
-      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",
-      "production_center": "Mercator Oc\u00e9an International",
-      "creation_datetime": "2018-02-12",
-      "modified_datetime": "2018-02-12",
-      "datasets": [
-        {
-          "dataset_id": "antarctic_omi_si_extent",
-          "dataset_name": "antarctic_omi_si_extent",
-          "services": [
-            {
-              "protocol": "ftp",
-              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"
-            }
-          ],
-          "variables": []
-        }
-      ]
-    },
-    ...
-  ]
-}
-
-```
-
-Check out the help:
-
-```
-> copernicus-marine describe --help
-Usage: copernicus-marine describe [OPTIONS]
-
-Options:
-  --one-line             Output JSON on one line
-  --include-description  Include product description in output
-  --include-datasets     Include product dataset details in output
-  --include-keywords     Include product keyword details in output
-  -c, --contains TEXT    Filter catalogue output. Returns products with
-                         attributes matching a string token
-  --overwrite-cache      Force to refresh the catalogue by overwriting the
-                         local cache
-  --help                 Show this message and exit.
-```
-
-### Command *subset*
-
-Download a dataset subset, based on dataset id, variable names and attributes slices:
-
-```
-> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1
-
-< Login:
-< Password:
-< Trying to download as one file...
-```
-
-File downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options).
-
-Check out the help:
-
-```
-> copernicus-marine subset --help
-
-Usage: copernicus-marine subset [OPTIONS]
-
-  Downloads subsets of datasets as NetCDF files or Zarr store.     Either one of 'dataset-
-  id' or 'dataset-url' is required     (can be found via the 'copernicus-
-  marine describe' command).     The arguments value passed individually
-  through the CLI take precedence     over the values from the "motu-api-
-  request" option, which takes precedence     over the ones from the "request-
-  file" option
-
-  Example:
-
-    copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
-    --variable analysed_sst --variable sea_ice_fraction --start-datetime
-    2021-01-01 --end-datetime 2021-01-02 --minimal-longitude 0.0 --maximal-
-    longitude 0.1 --minimal-latitude 0.0 --maximal-latitude 0.1
-
-    copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v
-    analysed_sst   -v sea_ice_fraction -t 2021-01-01 -T 2021-01-02 -x 0.0 -X
-    0.1 -y 0.0 -Y 0.1
-
-Options:
-  -u, --dataset-url TEXT          The full dataset URL
-  -i, --dataset-id TEXT           The dataset id
-  --login TEXT
-  --password TEXT
-  -v, --variable TEXT             Specify dataset variables
-  -x, --minimal-longitude FLOAT RANGE
-                                  Minimal longitude for the subset. Requires a
-                                  float whithin this range:  [-180<=x<=180]
-  -X, --maximal-longitude FLOAT RANGE
-                                  Maximal longitude for the subset. Requires a
-                                  float whithin this range:  [-180<=x<=180]
-  -y, --minimal-latitude FLOAT RANGE
-                                  Minimal latitude for the subset. Requires a
-                                  float whithin this range:  [-90<=x<=90]
-  -Y, --maximal-latitude FLOAT RANGE
-                                  Maximal latitude for the subset. Requires a
-                                  float whithin this range:  [-90<=x<=90]
-  -z, --minimal-depth FLOAT RANGE
-                                  Minimal depth for the subset. Requires a
-                                  float whithin this range:  [x>=0]
-  -Z, --maximal-depth FLOAT RANGE
-                                  Maximal depth for the subset. Requires a
-                                  float whithin this range:  [x>=0]
-  -t, --start-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
-                                  The start datetime of the temporal subset
-  -T, --end-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
-                                  The end datetime of the temporal subset
-  -o, --output-directory PATH     The destination folder for the downloaded
-                                  files. Default is the current directory
-  -f, --output-filename PATH      Concatenate the downloaded data in the given
-                                  file name (under the output directory)
-  --assume-yes                    Flag to skip confirmation before download
-  --force-protocol [zarr|zarr-map|zarr-timeserie|opendap|motu]
-                                  Force download through one of the available
-                                  protocols
-  --dry-run                       Flag to specify NOT to send the request to
-                                  external server. Returns the request instead
-  --request-file PATH             Option to pass a filename corresponding to a
-                                  file containg CLI arguments. The file MUST
-                                  follow the structure of dataclass
-                                  'SubsetRequest'.
-  --motu-api-request TEXT         Option to pass a complete MOTU api request
-                                  as a string. Caution, user has to replace
-                                  double quotes " with single quotes ' in the
-                                  request
-  --help                          Show this message and exit.
-```
-
-### Command *native*
-
-Download a native file (or files), based on dataset id or path to files:
-
-Example:
-```
-> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/
-
-< Login:
-< Password:
-< You requested the download of the following files:
-Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB
-Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB
-Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB
-Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB
-Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB
-Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB
-
-Total size of the download: 19.62 MB
-
-
-Do you want to continue? [y/N]:
-```
-
-File(s) downloaded to ./{path}/{filename} if not specified otherwise:
-- "--output-path" specifies a directory to dump the files in
-- "--no-directories" to not recreate the folder structure
-
-If not specified otherwise, after the header display with a summary of the request,
-the user is asked for confirmation:
-- "--no-confirmation" to turn down the confirmation prompt
-- "--show-outputnames" to display the full paths of the outputs files
-
-Check out the help:
-
-```
-> copernicus-marine native --help
-
-Usage: copernicus-marine native [OPTIONS]
-
-  Downloads native data files based on     dataset_id or datafiles url path.
-  The function fetches the files recursively if a folder path is passed as
-  url.     When provided a dataset id,     all the files in the corresponding
-  folder will be downloaded.
-
-      By default for any download request, a summary of the request result is
-      displayed to the user and a confirmation is asked.     This can be
-      turned down. Example:
-
-    copernicus-marine native -nd -o data_folder --dataset-id
-    cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m
-
-    copernicus-marine native -nd -o data_folder --dataset-url
-    ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-
-    pft_myint_7km-3D-diato_P1M-m
-
-Options:
-  -u, --dataset-url TEXT       Path to the data files
-  -i, --dataset-id TEXT        The dataset id
-  --login TEXT
-  --password TEXT
-  -nd, --no-directories        Option to not recreate folder hierarchy in
-                               ouput directory.
-  --show-outputnames           Option to display the names of the output files
-                               before download.
-  -o, --output-directory PATH  The destination directory for the downloaded
-                               files. Default is the current directory
-                               [required]
-  --assume-yes                 Whether to ask for confirmation before
-                               download, after header display. If 'True',
-                               skips confirmation.
-  --dry-run                    Flag to specify NOT to send the request to
-                               external server. Returns the request instead
-  --request-file PATH          Option to pass a file containg CLI arguments.
-                               The file MUST follow the structure of dataclass
-                               'SubsetRequest'. ANY PARAMETER SPECIFIED ASIDE
-                               FROM FILE WILL NOT BE TAKEN INTO CONSIDERATION
-                               FOR THE REQUEST IF FILE IS SPECIFIED.
-  --help                       Show this message and exit.
-```
-
-## Python functions
-
-The library also provide python functions to help with catalogue
-browsing and datasets download in scripts.
-
-### Basic example:
-
-In this example 4 steps are performed:
-  1- Fetch the catalogue to select a dataset
-  2- Construct a SubsetRequest for this dataset
-  3- Download the subset as a zarr store
-  4- Open the subset as an xarray dataset
-
-```
-import copernicus_marine_client as cmc
-
-# Step 1: Fetch catalogue and parse information on dataset
-catalogue = cmc.fetch_catalogue()
-dataset_id = 'cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m'
-assert(dataset_id in cmc.get_all_dataset_ids())
-dataset = catalogue.filter([dataset_id]).products[0].datasets[0]
-# Object "dataset" can be used to display all the metadata necessary to build a SubsetRequest
-variable = [variable for variable in dataset.variables if variable.short_name in ['zooc']][0]
-coordinates = {coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value) for coordinate in variable.coordinates}
-
-# Step 2: Construct the request based on parsed information
-subset_request = cmc.SubsetRequest(
-  dataset_id='cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m',
-  start_datetime="2023-04-20",
-  end_datetime='2023-04-21',
-  minimal_latitude= 30.0,
-  maximal_latitude=30.1,
-  minimal_longitude=0.1,
-  maximal_longitude=0.2,
-  minimal_depth=100,
-  maximal_depth=1000,
-  variables = ['zooc'],
-  force_protocol = "zarr-map",
-  output_directory = 'data_folder',
-  output_filename = 'datastore.zarr',
-  assume_yes = True,
-)
-
-# Step 3: Download the subset based on request content
-filename = cmc.download_subset(login='FAKE_LOGIN', password='FAKE_PASSWORD', subset_request=subset_request)
-
-# Step 4: Open the downloaded subset as an xarray dataset
-subset = cmc.open_dataset(filepath=filename, engine='zarr', out_type='xarray')
-```
-
-## Installation
-
-Using pip, for example:
-```
-pip install copernicus-marine-client
-```
-## Technical details
-
-This module is organized around two capabilities:
-- a catalogue, parsed from web requests, that contains informations on the available datasets
-- a downloader, to simplify the download of dataset files or subsets
-
-The catalogue can be displayed by the user and is used by the downloader to link the user
-requests with files or subset of files to retrieve.
-The downloader will help the user download the needed datasets.
-
-A rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.
-
-For subset command, the format is:
-
-```
-@dataclass
-class SubsetRequest:
-    dataset_url: Optional[str] = None
-    dataset_id: Optional[str] = None
-    variables: Optional[List[str]] = None
-    minimal_longitude: Optional[float] = None
-    maximal_longitude: Optional[float] = None
-    minimal_latitude: Optional[float] = None
-    maximal_latitude: Optional[float] = None
-    minimal_depth: Optional[float] = None
-    maximal_depth: Optional[float] = None
-    start_datetime: Optional[datetime] = None
-    end_datetime: Optional[datetime] = None
-    output_directory: Optional[str] = None
-    output_filename: Optional[str] = None
-    assume_yes: Optional[bool] = None
-    force_protocol: Optional[str] = None
-    dry_run: Optional[bool] = None
-```
+# Copernicus Marine Service client
+
+A library to facilitate the access of Copernicus Marine Service products and datasets.
+
+## Introduction
+
+This package allows to recover products and datasets information from Command Line Interface or with Python code,
+as well as download subsets and native files.
+
+## Command Line Interface (CLI)
+
+### Command *describe*
+Retrieve information about products as JSON:
+
+```
+> copernicus-marine describe
+{
+  "products": [
+    {
+      "title": "Antarctic Sea Ice Extent from Reanalysis",
+      "product_id": "ANTARCTIC_OMI_SI_extent",
+      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",
+      "production_center": "Mercator Oc\u00e9an International",
+      "creation_datetime": "2018-02-12",
+      "modified_datetime": "2018-02-12",
+    }
+    ...
+  ]
+}
+```
+
+Retrieve all information about datasets as JSON:
+
+```
+> copernicus-marine describe --include-datasets
+{
+  "products": [
+    {
+      "title": "Antarctic Sea Ice Extent from Reanalysis",
+      "product_id": "ANTARCTIC_OMI_SI_extent",
+      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",
+      "production_center": "Mercator Oc\u00e9an International",
+      "creation_datetime": "2018-02-12",
+      "modified_datetime": "2018-02-12",
+      "datasets": [
+        {
+          "dataset_id": "antarctic_omi_si_extent",
+          "dataset_name": "antarctic_omi_si_extent",
+          "services": [
+            {
+              "protocol": "ftp",
+              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"
+            }
+          ],
+          "variables": []
+        }
+      ]
+    },
+    ...
+  ]
+}
+
+```
+
+Check out the help:
+
+```
+> copernicus-marine describe --help
+Usage: copernicus-marine describe [OPTIONS]
+
+Options:
+  --one-line             Output JSON on one line
+  --include-description  Include product description in output
+  --include-datasets     Include product dataset details in output
+  --include-keywords     Include product keyword details in output
+  -c, --contains TEXT    Filter catalogue output. Returns products with
+                         attributes matching a string token
+  --overwrite-cache      Force to refresh the catalogue by overwriting the
+                         local cache
+  --help                 Show this message and exit.
+```
+
+### Command *login*
+
+Create the configuration files for access to the copernicus marine service:
+'.dodsrc', '.netrc', '.motuclient-python.ini'.
+The directory to store these configuration files can be modified by the user using the "config-file-directory" option
+but beware as it should also be passed to the *subset* and *native* command afterwards.
+By default, if the configuration files already exist, the user is asked for confirmation to overwrite them.
+
+Example:
+'''
+> copernicus marine login
+< Username :
+< Password :
+> INFO     - root - Configuration files stored in ${HOME}\.copernicus_marine_client
+'''
+
+
+Checkout the help:
+'''
+> copernicus-marine login --help
+Usage: copernicus-marine login [OPTIONS]
+
+  This command creates the configurations files used by the various download
+  services and store them in a directory that can be specified by the user. If
+  the user specified a different 'config_file_directory' from default one
+  ($HOME/.copernicus_marine_client), it needs to be passed also to the
+  download commands.
+
+  Examples:
+
+  Case 1 (Recommended):
+
+  With environment variables COPERNICUS_MARINE_CLIENT_USERNAME &
+  COPERNICUS_MARINE_CLIENT_PASSWORD specified:
+
+  > copernicus-marine login
+
+  Case 2:
+
+  > copernicus-marine login
+
+  < Username: [USER-INPUT]
+
+  < Password: [USER-INPUT]
+
+  Case 3:
+
+  > copernicus-marine login --username JOHN_DOE --password SECRETPASSWORD
+
+  Case 4: Specific directory for config_files
+
+  > copernicus-marine login --config-file-directory USER/SPECIFIED/PATH
+
+Options:
+  --username TEXT                 Search for environment variable:
+                                  COPERNICUS_MARINE_CLIENT_USERNAME if not,
+                                  ask for user input
+  --password TEXT                 Search for environment variable:
+                                  COPERNICUS_MARINE_CLIENT_PASSWORD if not,
+                                  ask for user input
+  --config-file-directory TEXT    Path to the directory where the
+                                  configuration files are stored
+  --assume-yes                    Flag to skip confirmation before overwriting
+                                  configuration files
+  --verbose [DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]
+                                  Set the details printed to console by the
+                                  command (based on standard logging library).
+  --help                          Show this message and exit.
+'''
+
+### Command *subset*
+
+Download a dataset subset, based on dataset id, variable names and attributes slices:
+
+```
+> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1
+
+< Username:
+< Password:
+< Trying to download as one file...
+```
+
+File downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options).
+
+Check out the help:
+
+```
+> copernicus-marine subset --help
+
+Usage: copernicus-marine subset [OPTIONS]
+
+  Downloads subsets of datasets as NetCDF files or Zarr stores.     Either one
+  of 'dataset-id' or 'dataset-url' is required     (can be found via the
+  'copernicus-marine describe' command).     The arguments value passed
+  individually through the CLI take precedence     over the values from the
+  "motu-api-request" option, which takes precedence     over the ones from the
+  "request-file" option
+
+  Example:
+
+    copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
+    --variable analysed_sst --variable sea_ice_fraction --start-datetime
+    2021-01-01 --end-datetime 2021-01-02 --minimal-longitude 0.0 --maximal-
+    longitude 0.1 --minimal-latitude 0.0 --maximal-latitude 0.1
+
+    copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v
+    analysed_sst   -v sea_ice_fraction -t "2021-01-01 01:00:00" -T "2021-01-02
+    13:00:00" -x 0.0 -X 0.1 -y 0.0 -Y 0.1
+
+Options:
+  -u, --dataset-url TEXT          The full dataset URL
+  -i, --dataset-id TEXT           The dataset id
+  --username TEXT
+  --password TEXT
+  -v, --variable TEXT             Specify dataset variables
+  -x, --minimal-longitude FLOAT RANGE
+                                  Minimal longitude for the subset. Requires a
+                                  float within this range:  [-180<=x<=180]
+  -X, --maximal-longitude FLOAT RANGE
+                                  Maximal longitude for the subset. Requires a
+                                  float within this range:  [-180<=x<=180]
+  -y, --minimal-latitude FLOAT RANGE
+                                  Minimal latitude for the subset. Requires a
+                                  float within this range:  [-90<=x<=90]
+  -Y, --maximal-latitude FLOAT RANGE
+                                  Maximal latitude for the subset. Requires a
+                                  float within this range:  [-90<=x<=90]
+  -z, --minimal-depth FLOAT RANGE
+                                  Minimal depth for the subset. Requires a
+                                  float within this range:  [x>=0]
+  -Z, --maximal-depth FLOAT RANGE
+                                  Maximal depth for the subset. Requires a
+                                  float within this range:  [x>=0]
+  -t, --start-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
+                                  The start datetime of the temporal subset.
+                                  Caution: encapsulate date with " " to ensure
+                                  valid format for format "%Y-%m-%d %H:%M:%S"
+  -T, --end-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
+                                  The end datetime of the temporal subset.
+                                  Caution: encapsulate date with " " to ensure
+                                  valid format for format "%Y-%m-%d %H:%M:%S"
+  -o, --output-directory PATH     The destination folder for the downloaded
+                                  files. Default is the current directory
+  -f, --output-filename PATH      Concatenate the downloaded data in the given
+                                  file name (under the output directory)
+  --assume-yes                    Flag to skip confirmation before download
+  --force-protocol [zarr|zarr-map|zarr-timeserie|opendap|motu]
+                                  Force download through one of the available
+                                  protocols
+  --dry-run                       Flag to specify NOT to send the request to
+                                  external server. Returns the request instead
+  --request-file PATH             Option to pass a filename corresponding to a
+                                  file containg CLI arguments. The file MUST
+                                  follow the structure of dataclass
+                                  'SubsetRequest'.
+  --motu-api-request TEXT         Option to pass a complete MOTU api request
+                                  as a string. Caution, user has to replace
+                                  double quotes " with single quotes ' in the
+                                  request
+  --log-level [DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]
+                                  Set the details printed to console by the
+                                  command (based on standard logging library).
+  --help                          Show this message and exit
+```
+
+### Command *native*
+
+Download a native file (or files), based on dataset id or path to files:
+
+Example:
+```
+> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/
+
+< Username:
+< Password:
+< You requested the download of the following files:
+Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB
+Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB
+Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB
+Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB
+Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB
+Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB
+
+Total size of the download: 19.62 MB
+
+
+Do you want to continue? [y/N]:
+```
+
+File(s) downloaded to ./{path}/{filename} if not specified otherwise:
+- "--output-path" specifies a directory to dump the files in
+- "--no-directories" to not recreate the folder structure
+
+If not specified otherwise, after the header display with a summary of the request,
+the user is asked for confirmation:
+- "--no-confirmation" to turn down the confirmation prompt
+- "--show-outputnames" to display the full paths of the outputs files
+
+Check out the help:
+
+```
+> copernicus-marine native --help
+
+Usage: copernicus-marine native [OPTIONS]
+
+  Downloads native data files based on     dataset_id or datafiles url path.
+  The function fetches the files recursively if a folder path is passed as
+  url.     When provided a dataset id,     all the files in the corresponding
+  folder will be downloaded.
+
+      By default for any download request, a summary of the request result is
+      displayed to the user and a confirmation is asked.     This can be
+      turned down. Example:
+
+    copernicus-marine native -nd -o data_folder --dataset-id
+    cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m
+
+    copernicus-marine native -nd -o data_folder --dataset-url
+    ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-
+    pft_myint_7km-3D-diato_P1M-m
+
+Options:
+  -u, --dataset-url TEXT       Path to the data files
+  -i, --dataset-id TEXT        The dataset id
+  --username TEXT
+  --password TEXT
+  -nd, --no-directories        Option to not recreate folder hierarchy in
+                               ouput directory.
+  --show-outputnames           Option to display the names of the output files
+                               before download.
+  -o, --output-directory PATH  The destination directory for the downloaded
+                               files. Default is the current directory
+                               [required]
+  --assume-yes                 Whether to ask for confirmation before
+                               download, after header display. If 'True',
+                               skips confirmation.
+  --dry-run                    Flag to specify NOT to send the request to
+                               external server. Returns the request instead
+  --request-file PATH          Option to pass a file containg CLI arguments.
+                               The file MUST follow the structure of dataclass
+                               'SubsetRequest'. ANY PARAMETER SPECIFIED ASIDE
+                               FROM FILE WILL NOT BE TAKEN INTO CONSIDERATION
+                               FOR THE REQUEST IF FILE IS SPECIFIED.
+  --help                       Show this message and exit.
+```
+
+## Python functions
+
+The library also provide python functions to help with catalogue
+browsing and datasets download in scripts.
+
+### Basic example:
+
+In this example 4 steps are performed:
+  1- Fetch the catalogue to select a dataset
+  2- Construct a SubsetRequest for this dataset
+  3- Download the subset as a zarr store
+  4- Open the subset as an xarray dataset
+
+```
+import copernicus_marine_client as cmc
+
+# Step 1: Fetch catalogue and parse information on dataset
+catalogue = cmc.fetch_catalogue()
+dataset_id = 'cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m'
+assert(dataset_id in cmc.get_all_dataset_ids())
+dataset = catalogue.filter([dataset_id]).products[0].datasets[0]
+# Object "dataset" can be used to display all the metadata necessary to build a SubsetRequest
+variable = [variable for variable in dataset.variables if variable.short_name in ['zooc']][0]
+coordinates = {coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value) for coordinate in variable.coordinates}
+
+# Step 2: Construct the request based on parsed information
+subset_request = cmc.SubsetRequest(
+  dataset_id='cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m',
+  start_datetime="2023-04-20",
+  end_datetime='2023-04-21',
+  minimal_latitude= 30.0,
+  maximal_latitude=30.1,
+  minimal_longitude=0.1,
+  maximal_longitude=0.2,
+  minimal_depth=100,
+  maximal_depth=1000,
+  variables = ['zooc'],
+  force_protocol = "zarr-map",
+  output_directory = 'data_folder',
+  output_filename = 'datastore.zarr',
+  assume_yes = True,
+)
+
+# Step 3: Download the subset based on request content
+filename = cmc.download_subset(username='FAKE_USERNAME', password='FAKE_PASSWORD', subset_request=subset_request)
+
+# Step 4: Open the downloaded subset as an xarray dataset
+subset = cmc.open_dataset(filepath=filename, engine='zarr', out_type='xarray')
+```
+
+## Installation
+
+Using pip, for example:
+```
+pip install copernicus-marine-client
+```
+## Technical details
+
+This module is organized around two capabilities:
+- a catalogue, parsed from web requests, that contains informations on the available datasets
+- a downloader, to simplify the download of dataset files or subsets
+
+The catalogue can be displayed by the user and is used by the downloader to link the user
+requests with files or subset of files to retrieve.
+The downloader will help the user download the needed datasets.
+
+A rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.
+
+For subset command, the format is:
+
+```
+@dataclass
+class SubsetRequest:
+    dataset_url: Optional[str] = None
+    dataset_id: Optional[str] = None
+    variables: Optional[List[str]] = None
+    minimal_longitude: Optional[float] = None
+    maximal_longitude: Optional[float] = None
+    minimal_latitude: Optional[float] = None
+    maximal_latitude: Optional[float] = None
+    minimal_depth: Optional[float] = None
+    maximal_depth: Optional[float] = None
+    start_datetime: Optional[datetime] = None
+    end_datetime: Optional[datetime] = None
+    output_directory: Optional[str] = None
+    output_filename: Optional[str] = None
+    assume_yes: Optional[bool] = None
+    force_protocol: Optional[str] = None
+    dry_run: Optional[bool] = None
+```
```

### Comparing `copernicus_marine_client-0.7.1/setup.py` & `copernicus_marine_client-0.8.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,28 +18,29 @@
  'motuclient==1.8.4',
  'netCDF4>=1.6.3',
  'numpy>=1.0',
  'owslib>=0.27.2',
  'pydap>=3.2.2',
  'pystac>=1.7.2',
  'requests>=2.27.1',
+ 's3fs>=2023.6.0,<2024.0.0',
  'setuptools>=62.0.0',
  'tqdm>=4.65.0',
  'xarray>=2023.3.0',
  'zarr>=2.13.3']
 
 entry_points = \
 {'console_scripts': ['copernicus-marine = '
                      'copernicus_marine_client.command_line_interface.copernicus_marine:command_line_interface']}
 
 setup_kwargs = {
     'name': 'copernicus-marine-client',
-    'version': '0.7.1',
+    'version': '0.8.0',
     'description': '',
-    'long_description': '# Copernicus Marine Service client\n\nA library to facilitate the access of Copernicus Marine Service products and datasets.\n\n## Introduction\n\nThis package allows to recover products and datasets information from Command Line Interface or with Python code,\nas well as download subsets and native files.\n\n## Command Line Interface (CLI)\n\n### Command *describe*\nRetrieve information about products as JSON:\n\n```\n> copernicus-marine describe\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n    }\n    ...\n  ]\n}\n```\n\nRetrieve all information about datasets as JSON:\n\n```\n> copernicus-marine describe --include-datasets\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n      "datasets": [\n        {\n          "dataset_id": "antarctic_omi_si_extent",\n          "dataset_name": "antarctic_omi_si_extent",\n          "services": [\n            {\n              "protocol": "ftp",\n              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"\n            }\n          ],\n          "variables": []\n        }\n      ]\n    },\n    ...\n  ]\n}\n\n```\n\nCheck out the help:\n\n```\n> copernicus-marine describe --help\nUsage: copernicus-marine describe [OPTIONS]\n\nOptions:\n  --one-line             Output JSON on one line\n  --include-description  Include product description in output\n  --include-datasets     Include product dataset details in output\n  --include-keywords     Include product keyword details in output\n  -c, --contains TEXT    Filter catalogue output. Returns products with\n                         attributes matching a string token\n  --overwrite-cache      Force to refresh the catalogue by overwriting the\n                         local cache\n  --help                 Show this message and exit.\n```\n\n### Command *subset*\n\nDownload a dataset subset, based on dataset id, variable names and attributes slices:\n\n```\n> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\n< Login:\n< Password:\n< Trying to download as one file...\n```\n\nFile downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options).\n\nCheck out the help:\n\n```\n> copernicus-marine subset --help\n\nUsage: copernicus-marine subset [OPTIONS]\n\n  Downloads subsets of datasets as NetCDF files or Zarr store.     Either one of \'dataset-\n  id\' or \'dataset-url\' is required     (can be found via the \'copernicus-\n  marine describe\' command).     The arguments value passed individually\n  through the CLI take precedence     over the values from the "motu-api-\n  request" option, which takes precedence     over the ones from the "request-\n  file" option\n\n  Example:\n\n    copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2\n    --variable analysed_sst --variable sea_ice_fraction --start-datetime\n    2021-01-01 --end-datetime 2021-01-02 --minimal-longitude 0.0 --maximal-\n    longitude 0.1 --minimal-latitude 0.0 --maximal-latitude 0.1\n\n    copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v\n    analysed_sst   -v sea_ice_fraction -t 2021-01-01 -T 2021-01-02 -x 0.0 -X\n    0.1 -y 0.0 -Y 0.1\n\nOptions:\n  -u, --dataset-url TEXT          The full dataset URL\n  -i, --dataset-id TEXT           The dataset id\n  --login TEXT\n  --password TEXT\n  -v, --variable TEXT             Specify dataset variables\n  -x, --minimal-longitude FLOAT RANGE\n                                  Minimal longitude for the subset. Requires a\n                                  float whithin this range:  [-180<=x<=180]\n  -X, --maximal-longitude FLOAT RANGE\n                                  Maximal longitude for the subset. Requires a\n                                  float whithin this range:  [-180<=x<=180]\n  -y, --minimal-latitude FLOAT RANGE\n                                  Minimal latitude for the subset. Requires a\n                                  float whithin this range:  [-90<=x<=90]\n  -Y, --maximal-latitude FLOAT RANGE\n                                  Maximal latitude for the subset. Requires a\n                                  float whithin this range:  [-90<=x<=90]\n  -z, --minimal-depth FLOAT RANGE\n                                  Minimal depth for the subset. Requires a\n                                  float whithin this range:  [x>=0]\n  -Z, --maximal-depth FLOAT RANGE\n                                  Maximal depth for the subset. Requires a\n                                  float whithin this range:  [x>=0]\n  -t, --start-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]\n                                  The start datetime of the temporal subset\n  -T, --end-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]\n                                  The end datetime of the temporal subset\n  -o, --output-directory PATH     The destination folder for the downloaded\n                                  files. Default is the current directory\n  -f, --output-filename PATH      Concatenate the downloaded data in the given\n                                  file name (under the output directory)\n  --assume-yes                    Flag to skip confirmation before download\n  --force-protocol [zarr|zarr-map|zarr-timeserie|opendap|motu]\n                                  Force download through one of the available\n                                  protocols\n  --dry-run                       Flag to specify NOT to send the request to\n                                  external server. Returns the request instead\n  --request-file PATH             Option to pass a filename corresponding to a\n                                  file containg CLI arguments. The file MUST\n                                  follow the structure of dataclass\n                                  \'SubsetRequest\'.\n  --motu-api-request TEXT         Option to pass a complete MOTU api request\n                                  as a string. Caution, user has to replace\n                                  double quotes " with single quotes \' in the\n                                  request\n  --help                          Show this message and exit.\n```\n\n### Command *native*\n\nDownload a native file (or files), based on dataset id or path to files:\n\nExample:\n```\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/\n\n< Login:\n< Password:\n< You requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB\n\nTotal size of the download: 19.62 MB\n\n\nDo you want to continue? [y/N]:\n```\n\nFile(s) downloaded to ./{path}/{filename} if not specified otherwise:\n- "--output-path" specifies a directory to dump the files in\n- "--no-directories" to not recreate the folder structure\n\nIf not specified otherwise, after the header display with a summary of the request,\nthe user is asked for confirmation:\n- "--no-confirmation" to turn down the confirmation prompt\n- "--show-outputnames" to display the full paths of the outputs files\n\nCheck out the help:\n\n```\n> copernicus-marine native --help\n\nUsage: copernicus-marine native [OPTIONS]\n\n  Downloads native data files based on     dataset_id or datafiles url path.\n  The function fetches the files recursively if a folder path is passed as\n  url.     When provided a dataset id,     all the files in the corresponding\n  folder will be downloaded.\n\n      By default for any download request, a summary of the request result is\n      displayed to the user and a confirmation is asked.     This can be\n      turned down. Example:\n\n    copernicus-marine native -nd -o data_folder --dataset-id\n    cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m\n\n    copernicus-marine native -nd -o data_folder --dataset-url\n    ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-\n    pft_myint_7km-3D-diato_P1M-m\n\nOptions:\n  -u, --dataset-url TEXT       Path to the data files\n  -i, --dataset-id TEXT        The dataset id\n  --login TEXT\n  --password TEXT\n  -nd, --no-directories        Option to not recreate folder hierarchy in\n                               ouput directory.\n  --show-outputnames           Option to display the names of the output files\n                               before download.\n  -o, --output-directory PATH  The destination directory for the downloaded\n                               files. Default is the current directory\n                               [required]\n  --assume-yes                 Whether to ask for confirmation before\n                               download, after header display. If \'True\',\n                               skips confirmation.\n  --dry-run                    Flag to specify NOT to send the request to\n                               external server. Returns the request instead\n  --request-file PATH          Option to pass a file containg CLI arguments.\n                               The file MUST follow the structure of dataclass\n                               \'SubsetRequest\'. ANY PARAMETER SPECIFIED ASIDE\n                               FROM FILE WILL NOT BE TAKEN INTO CONSIDERATION\n                               FOR THE REQUEST IF FILE IS SPECIFIED.\n  --help                       Show this message and exit.\n```\n\n## Python functions\n\nThe library also provide python functions to help with catalogue\nbrowsing and datasets download in scripts.\n\n### Basic example:\n\nIn this example 4 steps are performed:\n  1- Fetch the catalogue to select a dataset\n  2- Construct a SubsetRequest for this dataset\n  3- Download the subset as a zarr store\n  4- Open the subset as an xarray dataset\n\n```\nimport copernicus_marine_client as cmc\n\n# Step 1: Fetch catalogue and parse information on dataset\ncatalogue = cmc.fetch_catalogue()\ndataset_id = \'cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m\'\nassert(dataset_id in cmc.get_all_dataset_ids())\ndataset = catalogue.filter([dataset_id]).products[0].datasets[0]\n# Object "dataset" can be used to display all the metadata necessary to build a SubsetRequest\nvariable = [variable for variable in dataset.variables if variable.short_name in [\'zooc\']][0]\ncoordinates = {coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value) for coordinate in variable.coordinates}\n\n# Step 2: Construct the request based on parsed information\nsubset_request = cmc.SubsetRequest(\n  dataset_id=\'cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m\',\n  start_datetime="2023-04-20",\n  end_datetime=\'2023-04-21\',\n  minimal_latitude= 30.0,\n  maximal_latitude=30.1,\n  minimal_longitude=0.1,\n  maximal_longitude=0.2,\n  minimal_depth=100,\n  maximal_depth=1000,\n  variables = [\'zooc\'],\n  force_protocol = "zarr-map",\n  output_directory = \'data_folder\',\n  output_filename = \'datastore.zarr\',\n  assume_yes = True,\n)\n\n# Step 3: Download the subset based on request content\nfilename = cmc.download_subset(login=\'FAKE_LOGIN\', password=\'FAKE_PASSWORD\', subset_request=subset_request)\n\n# Step 4: Open the downloaded subset as an xarray dataset\nsubset = cmc.open_dataset(filepath=filename, engine=\'zarr\', out_type=\'xarray\')\n```\n\n## Installation\n\nUsing pip, for example:\n```\npip install copernicus-marine-client\n```\n## Technical details\n\nThis module is organized around two capabilities:\n- a catalogue, parsed from web requests, that contains informations on the available datasets\n- a downloader, to simplify the download of dataset files or subsets\n\nThe catalogue can be displayed by the user and is used by the downloader to link the user\nrequests with files or subset of files to retrieve.\nThe downloader will help the user download the needed datasets.\n\nA rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.\n\nFor subset command, the format is:\n\n```\n@dataclass\nclass SubsetRequest:\n    dataset_url: Optional[str] = None\n    dataset_id: Optional[str] = None\n    variables: Optional[List[str]] = None\n    minimal_longitude: Optional[float] = None\n    maximal_longitude: Optional[float] = None\n    minimal_latitude: Optional[float] = None\n    maximal_latitude: Optional[float] = None\n    minimal_depth: Optional[float] = None\n    maximal_depth: Optional[float] = None\n    start_datetime: Optional[datetime] = None\n    end_datetime: Optional[datetime] = None\n    output_directory: Optional[str] = None\n    output_filename: Optional[str] = None\n    assume_yes: Optional[bool] = None\n    force_protocol: Optional[str] = None\n    dry_run: Optional[bool] = None\n```\n',
+    'long_description': '# Copernicus Marine Service client\n\nA library to facilitate the access of Copernicus Marine Service products and datasets.\n\n## Introduction\n\nThis package allows to recover products and datasets information from Command Line Interface or with Python code,\nas well as download subsets and native files.\n\n## Command Line Interface (CLI)\n\n### Command *describe*\nRetrieve information about products as JSON:\n\n```\n> copernicus-marine describe\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n    }\n    ...\n  ]\n}\n```\n\nRetrieve all information about datasets as JSON:\n\n```\n> copernicus-marine describe --include-datasets\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n      "datasets": [\n        {\n          "dataset_id": "antarctic_omi_si_extent",\n          "dataset_name": "antarctic_omi_si_extent",\n          "services": [\n            {\n              "protocol": "ftp",\n              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"\n            }\n          ],\n          "variables": []\n        }\n      ]\n    },\n    ...\n  ]\n}\n\n```\n\nCheck out the help:\n\n```\n> copernicus-marine describe --help\nUsage: copernicus-marine describe [OPTIONS]\n\nOptions:\n  --one-line             Output JSON on one line\n  --include-description  Include product description in output\n  --include-datasets     Include product dataset details in output\n  --include-keywords     Include product keyword details in output\n  -c, --contains TEXT    Filter catalogue output. Returns products with\n                         attributes matching a string token\n  --overwrite-cache      Force to refresh the catalogue by overwriting the\n                         local cache\n  --help                 Show this message and exit.\n```\n\n### Command *login*\n\nCreate the configuration files for access to the copernicus marine service:\n\'.dodsrc\', \'.netrc\', \'.motuclient-python.ini\'.\nThe directory to store these configuration files can be modified by the user using the "config-file-directory" option\nbut beware as it should also be passed to the *subset* and *native* command afterwards.\nBy default, if the configuration files already exist, the user is asked for confirmation to overwrite them.\n\nExample:\n\'\'\'\n> copernicus marine login\n< Username :\n< Password :\n> INFO     - root - Configuration files stored in ${HOME}\\.copernicus_marine_client\n\'\'\'\n\n\nCheckout the help:\n\'\'\'\n> copernicus-marine login --help\nUsage: copernicus-marine login [OPTIONS]\n\n  This command creates the configurations files used by the various download\n  services and store them in a directory that can be specified by the user. If\n  the user specified a different \'config_file_directory\' from default one\n  ($HOME/.copernicus_marine_client), it needs to be passed also to the\n  download commands.\n\n  Examples:\n\n  Case 1 (Recommended):\n\n  With environment variables COPERNICUS_MARINE_CLIENT_USERNAME &\n  COPERNICUS_MARINE_CLIENT_PASSWORD specified:\n\n  > copernicus-marine login\n\n  Case 2:\n\n  > copernicus-marine login\n\n  < Username: [USER-INPUT]\n\n  < Password: [USER-INPUT]\n\n  Case 3:\n\n  > copernicus-marine login --username JOHN_DOE --password SECRETPASSWORD\n\n  Case 4: Specific directory for config_files\n\n  > copernicus-marine login --config-file-directory USER/SPECIFIED/PATH\n\nOptions:\n  --username TEXT                 Search for environment variable:\n                                  COPERNICUS_MARINE_CLIENT_USERNAME if not,\n                                  ask for user input\n  --password TEXT                 Search for environment variable:\n                                  COPERNICUS_MARINE_CLIENT_PASSWORD if not,\n                                  ask for user input\n  --config-file-directory TEXT    Path to the directory where the\n                                  configuration files are stored\n  --assume-yes                    Flag to skip confirmation before overwriting\n                                  configuration files\n  --verbose [DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]\n                                  Set the details printed to console by the\n                                  command (based on standard logging library).\n  --help                          Show this message and exit.\n\'\'\'\n\n### Command *subset*\n\nDownload a dataset subset, based on dataset id, variable names and attributes slices:\n\n```\n> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\n< Username:\n< Password:\n< Trying to download as one file...\n```\n\nFile downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options).\n\nCheck out the help:\n\n```\n> copernicus-marine subset --help\n\nUsage: copernicus-marine subset [OPTIONS]\n\n  Downloads subsets of datasets as NetCDF files or Zarr stores.     Either one\n  of \'dataset-id\' or \'dataset-url\' is required     (can be found via the\n  \'copernicus-marine describe\' command).     The arguments value passed\n  individually through the CLI take precedence     over the values from the\n  "motu-api-request" option, which takes precedence     over the ones from the\n  "request-file" option\n\n  Example:\n\n    copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2\n    --variable analysed_sst --variable sea_ice_fraction --start-datetime\n    2021-01-01 --end-datetime 2021-01-02 --minimal-longitude 0.0 --maximal-\n    longitude 0.1 --minimal-latitude 0.0 --maximal-latitude 0.1\n\n    copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v\n    analysed_sst   -v sea_ice_fraction -t "2021-01-01 01:00:00" -T "2021-01-02\n    13:00:00" -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\nOptions:\n  -u, --dataset-url TEXT          The full dataset URL\n  -i, --dataset-id TEXT           The dataset id\n  --username TEXT\n  --password TEXT\n  -v, --variable TEXT             Specify dataset variables\n  -x, --minimal-longitude FLOAT RANGE\n                                  Minimal longitude for the subset. Requires a\n                                  float within this range:  [-180<=x<=180]\n  -X, --maximal-longitude FLOAT RANGE\n                                  Maximal longitude for the subset. Requires a\n                                  float within this range:  [-180<=x<=180]\n  -y, --minimal-latitude FLOAT RANGE\n                                  Minimal latitude for the subset. Requires a\n                                  float within this range:  [-90<=x<=90]\n  -Y, --maximal-latitude FLOAT RANGE\n                                  Maximal latitude for the subset. Requires a\n                                  float within this range:  [-90<=x<=90]\n  -z, --minimal-depth FLOAT RANGE\n                                  Minimal depth for the subset. Requires a\n                                  float within this range:  [x>=0]\n  -Z, --maximal-depth FLOAT RANGE\n                                  Maximal depth for the subset. Requires a\n                                  float within this range:  [x>=0]\n  -t, --start-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]\n                                  The start datetime of the temporal subset.\n                                  Caution: encapsulate date with " " to ensure\n                                  valid format for format "%Y-%m-%d %H:%M:%S"\n  -T, --end-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]\n                                  The end datetime of the temporal subset.\n                                  Caution: encapsulate date with " " to ensure\n                                  valid format for format "%Y-%m-%d %H:%M:%S"\n  -o, --output-directory PATH     The destination folder for the downloaded\n                                  files. Default is the current directory\n  -f, --output-filename PATH      Concatenate the downloaded data in the given\n                                  file name (under the output directory)\n  --assume-yes                    Flag to skip confirmation before download\n  --force-protocol [zarr|zarr-map|zarr-timeserie|opendap|motu]\n                                  Force download through one of the available\n                                  protocols\n  --dry-run                       Flag to specify NOT to send the request to\n                                  external server. Returns the request instead\n  --request-file PATH             Option to pass a filename corresponding to a\n                                  file containg CLI arguments. The file MUST\n                                  follow the structure of dataclass\n                                  \'SubsetRequest\'.\n  --motu-api-request TEXT         Option to pass a complete MOTU api request\n                                  as a string. Caution, user has to replace\n                                  double quotes " with single quotes \' in the\n                                  request\n  --log-level [DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]\n                                  Set the details printed to console by the\n                                  command (based on standard logging library).\n  --help                          Show this message and exit\n```\n\n### Command *native*\n\nDownload a native file (or files), based on dataset id or path to files:\n\nExample:\n```\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/\n\n< Username:\n< Password:\n< You requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB\n\nTotal size of the download: 19.62 MB\n\n\nDo you want to continue? [y/N]:\n```\n\nFile(s) downloaded to ./{path}/{filename} if not specified otherwise:\n- "--output-path" specifies a directory to dump the files in\n- "--no-directories" to not recreate the folder structure\n\nIf not specified otherwise, after the header display with a summary of the request,\nthe user is asked for confirmation:\n- "--no-confirmation" to turn down the confirmation prompt\n- "--show-outputnames" to display the full paths of the outputs files\n\nCheck out the help:\n\n```\n> copernicus-marine native --help\n\nUsage: copernicus-marine native [OPTIONS]\n\n  Downloads native data files based on     dataset_id or datafiles url path.\n  The function fetches the files recursively if a folder path is passed as\n  url.     When provided a dataset id,     all the files in the corresponding\n  folder will be downloaded.\n\n      By default for any download request, a summary of the request result is\n      displayed to the user and a confirmation is asked.     This can be\n      turned down. Example:\n\n    copernicus-marine native -nd -o data_folder --dataset-id\n    cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m\n\n    copernicus-marine native -nd -o data_folder --dataset-url\n    ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-\n    pft_myint_7km-3D-diato_P1M-m\n\nOptions:\n  -u, --dataset-url TEXT       Path to the data files\n  -i, --dataset-id TEXT        The dataset id\n  --username TEXT\n  --password TEXT\n  -nd, --no-directories        Option to not recreate folder hierarchy in\n                               ouput directory.\n  --show-outputnames           Option to display the names of the output files\n                               before download.\n  -o, --output-directory PATH  The destination directory for the downloaded\n                               files. Default is the current directory\n                               [required]\n  --assume-yes                 Whether to ask for confirmation before\n                               download, after header display. If \'True\',\n                               skips confirmation.\n  --dry-run                    Flag to specify NOT to send the request to\n                               external server. Returns the request instead\n  --request-file PATH          Option to pass a file containg CLI arguments.\n                               The file MUST follow the structure of dataclass\n                               \'SubsetRequest\'. ANY PARAMETER SPECIFIED ASIDE\n                               FROM FILE WILL NOT BE TAKEN INTO CONSIDERATION\n                               FOR THE REQUEST IF FILE IS SPECIFIED.\n  --help                       Show this message and exit.\n```\n\n## Python functions\n\nThe library also provide python functions to help with catalogue\nbrowsing and datasets download in scripts.\n\n### Basic example:\n\nIn this example 4 steps are performed:\n  1- Fetch the catalogue to select a dataset\n  2- Construct a SubsetRequest for this dataset\n  3- Download the subset as a zarr store\n  4- Open the subset as an xarray dataset\n\n```\nimport copernicus_marine_client as cmc\n\n# Step 1: Fetch catalogue and parse information on dataset\ncatalogue = cmc.fetch_catalogue()\ndataset_id = \'cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m\'\nassert(dataset_id in cmc.get_all_dataset_ids())\ndataset = catalogue.filter([dataset_id]).products[0].datasets[0]\n# Object "dataset" can be used to display all the metadata necessary to build a SubsetRequest\nvariable = [variable for variable in dataset.variables if variable.short_name in [\'zooc\']][0]\ncoordinates = {coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value) for coordinate in variable.coordinates}\n\n# Step 2: Construct the request based on parsed information\nsubset_request = cmc.SubsetRequest(\n  dataset_id=\'cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m\',\n  start_datetime="2023-04-20",\n  end_datetime=\'2023-04-21\',\n  minimal_latitude= 30.0,\n  maximal_latitude=30.1,\n  minimal_longitude=0.1,\n  maximal_longitude=0.2,\n  minimal_depth=100,\n  maximal_depth=1000,\n  variables = [\'zooc\'],\n  force_protocol = "zarr-map",\n  output_directory = \'data_folder\',\n  output_filename = \'datastore.zarr\',\n  assume_yes = True,\n)\n\n# Step 3: Download the subset based on request content\nfilename = cmc.download_subset(username=\'FAKE_USERNAME\', password=\'FAKE_PASSWORD\', subset_request=subset_request)\n\n# Step 4: Open the downloaded subset as an xarray dataset\nsubset = cmc.open_dataset(filepath=filename, engine=\'zarr\', out_type=\'xarray\')\n```\n\n## Installation\n\nUsing pip, for example:\n```\npip install copernicus-marine-client\n```\n## Technical details\n\nThis module is organized around two capabilities:\n- a catalogue, parsed from web requests, that contains informations on the available datasets\n- a downloader, to simplify the download of dataset files or subsets\n\nThe catalogue can be displayed by the user and is used by the downloader to link the user\nrequests with files or subset of files to retrieve.\nThe downloader will help the user download the needed datasets.\n\nA rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.\n\nFor subset command, the format is:\n\n```\n@dataclass\nclass SubsetRequest:\n    dataset_url: Optional[str] = None\n    dataset_id: Optional[str] = None\n    variables: Optional[List[str]] = None\n    minimal_longitude: Optional[float] = None\n    maximal_longitude: Optional[float] = None\n    minimal_latitude: Optional[float] = None\n    maximal_latitude: Optional[float] = None\n    minimal_depth: Optional[float] = None\n    maximal_depth: Optional[float] = None\n    start_datetime: Optional[datetime] = None\n    end_datetime: Optional[datetime] = None\n    output_directory: Optional[str] = None\n    output_filename: Optional[str] = None\n    assume_yes: Optional[bool] = None\n    force_protocol: Optional[str] = None\n    dry_run: Optional[bool] = None\n```\n',
     'author': 'jsouchard',
     'author_email': 'jsouchard@mercator-ocean.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `copernicus_marine_client-0.7.1/PKG-INFO` & `copernicus_marine_client-0.8.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copernicus-marine-client
-Version: 0.7.1
+Version: 0.8.0
 Summary: 
 Author: jsouchard
 Author-email: jsouchard@mercator-ocean.fr
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -16,14 +16,15 @@
 Requires-Dist: motuclient (==1.8.4)
 Requires-Dist: netCDF4 (>=1.6.3)
 Requires-Dist: numpy (>=1.0)
 Requires-Dist: owslib (>=0.27.2)
 Requires-Dist: pydap (>=3.2.2)
 Requires-Dist: pystac (>=1.7.2)
 Requires-Dist: requests (>=2.27.1)
+Requires-Dist: s3fs (>=2023.6.0,<2024.0.0)
 Requires-Dist: setuptools (>=62.0.0)
 Requires-Dist: tqdm (>=4.65.0)
 Requires-Dist: xarray (>=2023.3.0)
 Requires-Dist: zarr (>=2.13.3)
 Description-Content-Type: text/markdown
 
 # Copernicus Marine Service client
@@ -104,81 +105,155 @@
   -c, --contains TEXT    Filter catalogue output. Returns products with
                          attributes matching a string token
   --overwrite-cache      Force to refresh the catalogue by overwriting the
                          local cache
   --help                 Show this message and exit.
 ```
 
+### Command *login*
+
+Create the configuration files for access to the copernicus marine service:
+'.dodsrc', '.netrc', '.motuclient-python.ini'.
+The directory to store these configuration files can be modified by the user using the "config-file-directory" option
+but beware as it should also be passed to the *subset* and *native* command afterwards.
+By default, if the configuration files already exist, the user is asked for confirmation to overwrite them.
+
+Example:
+'''
+> copernicus marine login
+< Username :
+< Password :
+> INFO     - root - Configuration files stored in ${HOME}\.copernicus_marine_client
+'''
+
+
+Checkout the help:
+'''
+> copernicus-marine login --help
+Usage: copernicus-marine login [OPTIONS]
+
+  This command creates the configurations files used by the various download
+  services and store them in a directory that can be specified by the user. If
+  the user specified a different 'config_file_directory' from default one
+  ($HOME/.copernicus_marine_client), it needs to be passed also to the
+  download commands.
+
+  Examples:
+
+  Case 1 (Recommended):
+
+  With environment variables COPERNICUS_MARINE_CLIENT_USERNAME &
+  COPERNICUS_MARINE_CLIENT_PASSWORD specified:
+
+  > copernicus-marine login
+
+  Case 2:
+
+  > copernicus-marine login
+
+  < Username: [USER-INPUT]
+
+  < Password: [USER-INPUT]
+
+  Case 3:
+
+  > copernicus-marine login --username JOHN_DOE --password SECRETPASSWORD
+
+  Case 4: Specific directory for config_files
+
+  > copernicus-marine login --config-file-directory USER/SPECIFIED/PATH
+
+Options:
+  --username TEXT                 Search for environment variable:
+                                  COPERNICUS_MARINE_CLIENT_USERNAME if not,
+                                  ask for user input
+  --password TEXT                 Search for environment variable:
+                                  COPERNICUS_MARINE_CLIENT_PASSWORD if not,
+                                  ask for user input
+  --config-file-directory TEXT    Path to the directory where the
+                                  configuration files are stored
+  --assume-yes                    Flag to skip confirmation before overwriting
+                                  configuration files
+  --verbose [DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]
+                                  Set the details printed to console by the
+                                  command (based on standard logging library).
+  --help                          Show this message and exit.
+'''
+
 ### Command *subset*
 
 Download a dataset subset, based on dataset id, variable names and attributes slices:
 
 ```
 > copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1
 
-< Login:
+< Username:
 < Password:
 < Trying to download as one file...
 ```
 
 File downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options).
 
 Check out the help:
 
 ```
 > copernicus-marine subset --help
 
 Usage: copernicus-marine subset [OPTIONS]
 
-  Downloads subsets of datasets as NetCDF files or Zarr store.     Either one of 'dataset-
-  id' or 'dataset-url' is required     (can be found via the 'copernicus-
-  marine describe' command).     The arguments value passed individually
-  through the CLI take precedence     over the values from the "motu-api-
-  request" option, which takes precedence     over the ones from the "request-
-  file" option
+  Downloads subsets of datasets as NetCDF files or Zarr stores.     Either one
+  of 'dataset-id' or 'dataset-url' is required     (can be found via the
+  'copernicus-marine describe' command).     The arguments value passed
+  individually through the CLI take precedence     over the values from the
+  "motu-api-request" option, which takes precedence     over the ones from the
+  "request-file" option
 
   Example:
 
     copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
     --variable analysed_sst --variable sea_ice_fraction --start-datetime
     2021-01-01 --end-datetime 2021-01-02 --minimal-longitude 0.0 --maximal-
     longitude 0.1 --minimal-latitude 0.0 --maximal-latitude 0.1
 
     copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v
-    analysed_sst   -v sea_ice_fraction -t 2021-01-01 -T 2021-01-02 -x 0.0 -X
-    0.1 -y 0.0 -Y 0.1
+    analysed_sst   -v sea_ice_fraction -t "2021-01-01 01:00:00" -T "2021-01-02
+    13:00:00" -x 0.0 -X 0.1 -y 0.0 -Y 0.1
 
 Options:
   -u, --dataset-url TEXT          The full dataset URL
   -i, --dataset-id TEXT           The dataset id
-  --login TEXT
+  --username TEXT
   --password TEXT
   -v, --variable TEXT             Specify dataset variables
   -x, --minimal-longitude FLOAT RANGE
                                   Minimal longitude for the subset. Requires a
-                                  float whithin this range:  [-180<=x<=180]
+                                  float within this range:  [-180<=x<=180]
   -X, --maximal-longitude FLOAT RANGE
                                   Maximal longitude for the subset. Requires a
-                                  float whithin this range:  [-180<=x<=180]
+                                  float within this range:  [-180<=x<=180]
   -y, --minimal-latitude FLOAT RANGE
                                   Minimal latitude for the subset. Requires a
-                                  float whithin this range:  [-90<=x<=90]
+                                  float within this range:  [-90<=x<=90]
   -Y, --maximal-latitude FLOAT RANGE
                                   Maximal latitude for the subset. Requires a
-                                  float whithin this range:  [-90<=x<=90]
+                                  float within this range:  [-90<=x<=90]
   -z, --minimal-depth FLOAT RANGE
                                   Minimal depth for the subset. Requires a
-                                  float whithin this range:  [x>=0]
+                                  float within this range:  [x>=0]
   -Z, --maximal-depth FLOAT RANGE
                                   Maximal depth for the subset. Requires a
-                                  float whithin this range:  [x>=0]
+                                  float within this range:  [x>=0]
   -t, --start-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
-                                  The start datetime of the temporal subset
+                                  The start datetime of the temporal subset.
+                                  Caution: encapsulate date with " " to ensure
+                                  valid format for format "%Y-%m-%d %H:%M:%S"
   -T, --end-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
-                                  The end datetime of the temporal subset
+                                  The end datetime of the temporal subset.
+                                  Caution: encapsulate date with " " to ensure
+                                  valid format for format "%Y-%m-%d %H:%M:%S"
   -o, --output-directory PATH     The destination folder for the downloaded
                                   files. Default is the current directory
   -f, --output-filename PATH      Concatenate the downloaded data in the given
                                   file name (under the output directory)
   --assume-yes                    Flag to skip confirmation before download
   --force-protocol [zarr|zarr-map|zarr-timeserie|opendap|motu]
                                   Force download through one of the available
@@ -189,26 +264,29 @@
                                   file containg CLI arguments. The file MUST
                                   follow the structure of dataclass
                                   'SubsetRequest'.
   --motu-api-request TEXT         Option to pass a complete MOTU api request
                                   as a string. Caution, user has to replace
                                   double quotes " with single quotes ' in the
                                   request
-  --help                          Show this message and exit.
+  --log-level [DEBUG|INFO|WARN|ERROR|CRITICAL|QUIET]
+                                  Set the details printed to console by the
+                                  command (based on standard logging library).
+  --help                          Show this message and exit
 ```
 
 ### Command *native*
 
 Download a native file (or files), based on dataset id or path to files:
 
 Example:
 ```
 > copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/
 
-< Login:
+< Username:
 < Password:
 < You requested the download of the following files:
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB
 Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB
@@ -251,15 +329,15 @@
     copernicus-marine native -nd -o data_folder --dataset-url
     ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-
     pft_myint_7km-3D-diato_P1M-m
 
 Options:
   -u, --dataset-url TEXT       Path to the data files
   -i, --dataset-id TEXT        The dataset id
-  --login TEXT
+  --username TEXT
   --password TEXT
   -nd, --no-directories        Option to not recreate folder hierarchy in
                                ouput directory.
   --show-outputnames           Option to display the names of the output files
                                before download.
   -o, --output-directory PATH  The destination directory for the downloaded
                                files. Default is the current directory
@@ -317,15 +395,15 @@
   force_protocol = "zarr-map",
   output_directory = 'data_folder',
   output_filename = 'datastore.zarr',
   assume_yes = True,
 )
 
 # Step 3: Download the subset based on request content
-filename = cmc.download_subset(login='FAKE_LOGIN', password='FAKE_PASSWORD', subset_request=subset_request)
+filename = cmc.download_subset(username='FAKE_USERNAME', password='FAKE_PASSWORD', subset_request=subset_request)
 
 # Step 4: Open the downloaded subset as an xarray dataset
 subset = cmc.open_dataset(filepath=filename, engine='zarr', out_type='xarray')
 ```
 
 ## Installation
```

