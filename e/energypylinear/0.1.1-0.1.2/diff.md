# Comparing `tmp/energypylinear-0.1.1.tar.gz` & `tmp/energypylinear-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energypylinear-0.1.1.tar", max compression
+gzip compressed data, was "energypylinear-0.1.2.tar", max compression
```

## Comparing `energypylinear-0.1.1.tar` & `energypylinear-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     6732 2023-02-23 05:18:40.568361 energypylinear-0.1.1/README.md
--rw-r--r--   0        0        0      554 2023-02-17 05:49:16.589398 energypylinear-0.1.1/energypylinear/__init__.py
--rw-r--r--   0        0        0      167 2023-02-17 05:49:16.589660 energypylinear-0.1.1/energypylinear/accounting/__init__.py
--rw-r--r--   0        0        0     4054 2023-02-17 05:49:16.589909 energypylinear-0.1.1/energypylinear/accounting/accounting.py
--rw-r--r--   0        0        0      112 2023-02-17 05:49:16.590148 energypylinear-0.1.1/energypylinear/assets/__init__.py
--rw-r--r--   0        0        0     1584 2023-02-17 05:49:16.590315 energypylinear-0.1.1/energypylinear/assets/asset.py
--rw-r--r--   0        0        0      366 2023-01-29 03:21:48.176369 energypylinear-0.1.1/energypylinear/assets/asset.py-doc
--rw-r--r--   0        0        0    11044 2023-02-17 11:58:31.659489 energypylinear-0.1.1/energypylinear/assets/battery.py
--rw-r--r--   0        0        0      566 2023-01-29 03:45:46.973074 energypylinear-0.1.1/energypylinear/assets/battery.py-doc
--rw-r--r--   0        0        0    11346 2023-02-17 05:49:16.590682 energypylinear-0.1.1/energypylinear/assets/chp.py
--rw-r--r--   0        0        0    13696 2023-02-17 05:49:16.590916 energypylinear-0.1.1/energypylinear/assets/evs.py
--rw-r--r--   0        0        0     4923 2023-02-23 02:00:16.409486 energypylinear-0.1.1/energypylinear/assets/site.py
--rw-r--r--   0        0        0     1669 2023-02-17 05:49:16.591159 energypylinear-0.1.1/energypylinear/assets/spill.py
--rw-r--r--   0        0        0     1642 2023-02-17 05:49:16.591273 energypylinear-0.1.1/energypylinear/assets/valve.py
--rw-r--r--   0        0        0     1418 2023-02-17 05:49:16.591496 energypylinear-0.1.1/energypylinear/data_generation.py
--rw-r--r--   0        0        0      644 2023-02-17 05:49:16.591699 energypylinear-0.1.1/energypylinear/defaults.py
--rw-r--r--   0        0        0      250 2023-02-17 05:49:16.591835 energypylinear-0.1.1/energypylinear/flags.py
--rw-r--r--   0        0        0      650 2023-02-17 05:49:16.591947 energypylinear-0.1.1/energypylinear/freq.py
--rw-r--r--   0        0        0     6219 2023-02-17 05:49:16.592079 energypylinear-0.1.1/energypylinear/interval_data.py
--rw-r--r--   0        0        0     4616 2023-02-17 05:49:16.592199 energypylinear-0.1.1/energypylinear/objectives.py
--rw-r--r--   0        0        0     5148 2023-02-23 02:00:16.410309 energypylinear-0.1.1/energypylinear/optimizer.py
--rw-r--r--   0        0        0     5992 2023-02-17 05:49:16.592456 energypylinear-0.1.1/energypylinear/plot.py
--rw-r--r--   0        0        0     8537 2023-02-17 05:49:16.592657 energypylinear-0.1.1/energypylinear/results.py
--rw-r--r--   0        0        0      946 2023-02-24 05:32:44.923045 energypylinear-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7871 1970-01-01 00:00:00.000000 energypylinear-0.1.1/setup.py
--rw-r--r--   0        0        0     7492 1970-01-01 00:00:00.000000 energypylinear-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2645 2023-07-03 10:23:55.944732 energypylinear-0.1.2/README.md
+-rw-r--r--   0        0        0      927 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/__init__.py
+-rw-r--r--   0        0        0      167 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/accounting/__init__.py
+-rw-r--r--   0        0        0     4014 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/accounting/accounting.py
+-rw-r--r--   0        0        0      134 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/__init__.py
+-rw-r--r--   0        0        0     1593 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/asset.py
+-rw-r--r--   0        0        0    11253 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/battery.py
+-rw-r--r--   0        0        0     3624 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/boiler.py
+-rw-r--r--   0        0        0     9910 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/chp.py
+-rw-r--r--   0        0        0    15201 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/evs.py
+-rw-r--r--   0        0        0    12290 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/site.py
+-rw-r--r--   0        0        0     2553 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/spill.py
+-rw-r--r--   0        0        0     2520 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/assets/valve.py
+-rw-r--r--   0        0        0     1418 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/data_generation.py
+-rw-r--r--   0        0        0      734 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/defaults.py
+-rw-r--r--   0        0        0      357 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/flags.py
+-rw-r--r--   0        0        0      650 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/freq.py
+-rw-r--r--   0        0        0     6627 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/interval_data.py
+-rw-r--r--   0        0        0     4723 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/objectives.py
+-rw-r--r--   0        0        0     5367 2023-07-03 10:23:55.948732 energypylinear-0.1.2/energypylinear/optimizer.py
+-rw-r--r--   0        0        0     6122 2023-07-03 10:23:55.952733 energypylinear-0.1.2/energypylinear/plot.py
+-rw-r--r--   0        0        0    15471 2023-07-03 10:23:55.952733 energypylinear-0.1.2/energypylinear/results.py
+-rw-r--r--   0        0        0      841 2023-07-03 10:23:55.952733 energypylinear-0.1.2/energypylinear/utils.py
+-rw-r--r--   0        0        0     1063 2023-07-03 10:23:55.952733 energypylinear-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3703 1970-01-01 00:00:00.000000 energypylinear-0.1.2/setup.py
+-rw-r--r--   0        0        0     3496 1970-01-01 00:00:00.000000 energypylinear-0.1.2/PKG-INFO
```

### Comparing `energypylinear-0.1.1/energypylinear/__init__.py` & `energypylinear-0.1.2/energypylinear/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,19 +3,33 @@
     accounting,
     assets,
     data_generation,
     defaults,
     interval_data,
     plot,
     results,
+    utils,
 )
 from energypylinear.accounting import get_accounts
 from energypylinear.assets import battery, chp, evs, site, spill, valve
 from energypylinear.assets.battery import Battery
+from energypylinear.assets.boiler import Boiler
+from energypylinear.assets.chp import Generator
+from energypylinear.assets.evs import EVs
+from energypylinear.assets.site import Site
+from energypylinear.freq import Freq
 from energypylinear.interval_data import IntervalData
 from energypylinear.objectives import objectives
+from energypylinear.optimizer import Optimizer
 
 __all__ = [
     "Battery",
+    "Generator",
+    "Boiler",
+    "Site",
+    "Optimizer",
+    "EVs",
+    "Freq",
     "IntervalData",
     "get_accounts",
+    "utils",
 ]
```

### Comparing `energypylinear-0.1.1/energypylinear/accounting/accounting.py` & `energypylinear-0.1.2/energypylinear/accounting/accounting.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,54 +64,54 @@
 
 def get_one_gas_account(
     interval_data: "epl.interval_data.IntervalData",
     results: pd.DataFrame,
 ) -> GasAccount:
     """Calculate a single gas account from interval data and results."""
     return GasAccount(
-        cost=(interval_data.gas_prices * results["gas_consumption_mwh"]).sum(),
+        cost=(interval_data.gas_prices * results["total-gas_consumption_mwh"]).sum(),
         emissions=(
-            defaults.gas_carbon_intensity * results["gas_consumption_mwh"]
+            defaults.gas_carbon_intensity * results["total-gas_consumption_mwh"]
         ).sum(),
     )
 
 
 def get_one_electricity_account(
     interval_data: "epl.interval_data.IntervalData",
     results: pd.DataFrame,
 ) -> ElectricityAccount:
     """Calculate a single electricity account from interval data and results."""
-    import_cost = (interval_data.electricity_prices * results["import_power_mwh"]).sum()
+    import_cost = (
+        interval_data.electricity_prices * results["site-import_power_mwh"]
+    ).sum()
     export_cost = -(
-        interval_data.electricity_prices * results["export_power_mwh"]
+        interval_data.electricity_prices * results["site-export_power_mwh"]
     ).sum()
 
     import_emissions = (
-        interval_data.electricity_carbon_intensities * results["import_power_mwh"]
+        interval_data.electricity_carbon_intensities * results["site-import_power_mwh"]
     ).sum()
     export_emissions = -(
-        interval_data.electricity_carbon_intensities * results["export_power_mwh"]
+        interval_data.electricity_carbon_intensities * results["site-export_power_mwh"]
     ).sum()
 
-    # id = interval_data.electricity_carbon_intensities
-    # pr = results["import_power_mwh"].values
-    # breakpoint()  # fmt: skip
     return ElectricityAccount(
         import_cost=import_cost,
         export_cost=export_cost,
         cost=import_cost + export_cost,
         import_emissions=import_emissions,
         export_emissions=export_emissions,
         emissions=import_emissions + export_emissions,
     )
 
 
 def get_accounts(
     interval_data: "epl.interval_data.IntervalData",
     simulation: pd.DataFrame,
+    validate: bool = True,
 ) -> Accounts:
     """
     Create one pair of gas and electricity accounts.
     for given of interval data and simulation results.
 
     `interval_data` gives the prices ($/MWh) and carbon intensities (tC/MWh) used
     in the calculation of cost and carbon emissions.
@@ -119,15 +119,16 @@
     `simulation` gives the energy quantities (MWh) used in the
     calculation of cost and carbon emissions.
 
     Args:
         interval_data: holds prices and carbon intensities.
         simulation: simulation results.
     """
-    epl.results.validate_results(interval_data, simulation)
+    if validate:
+        epl.results.validate_results(interval_data, simulation)
     electricity = get_one_electricity_account(interval_data, simulation)
     gas = get_one_gas_account(interval_data, simulation)
 
     return Accounts(
         electricity=electricity,
         gas=gas,
         cost=electricity.cost + gas.cost,
```

### Comparing `energypylinear-0.1.1/energypylinear/assets/asset.py` & `energypylinear-0.1.2/energypylinear/assets/asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         - high temperature heat,
         - low temperature heat,
         - charge & discharge of electricity,
         - gas consumption.
 
     These quantities are considered as both generation and consumption (load).
 
-    Charge and discharge are handled as accumulation terms.
+    Charge and discharge are handled as explicit accumulation terms.
     """
 
     electric_generation_mwh: typing.Union[pulp.LpVariable, float] = 0
     high_temperature_generation_mwh: typing.Union[pulp.LpVariable, float] = 0
     low_temperature_generation_mwh: typing.Union[pulp.LpVariable, float] = 0
     #  add cooling generation here TODO
```

### Comparing `energypylinear-0.1.1/energypylinear/assets/battery.py` & `energypylinear-0.1.2/energypylinear/assets/battery.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import typing
 
 import numpy as np
 import pulp
 import pydantic
 
 import energypylinear as epl
-from energypylinear.assets import site
 from energypylinear.assets.asset import AssetOneInterval
 from energypylinear.defaults import defaults
 from energypylinear.flags import Flags
 from energypylinear.freq import Freq
 from energypylinear.optimizer import Optimizer
 
 
@@ -25,14 +24,15 @@
     efficiency_pct: float
     initial_charge_mwh: float = 0
     final_charge_mwh: float = 0
 
     @pydantic.validator("name")
     def check_name(cls, name: str) -> str:
         """Check that name includes battery."""
+
         assert "battery" in name
         return name
 
 
 class BatteryOneInterval(AssetOneInterval):
     """Battery asset data for a single interval"""
 
@@ -43,82 +43,46 @@
     discharge_binary: typing.Union[pulp.LpVariable, int]
     losses_mwh: pulp.LpVariable
     initial_charge_mwh: pulp.LpVariable
     final_charge_mwh: pulp.LpVariable
     efficiency_pct: float
 
 
-def battery_one_interval(
-    optimizer: Optimizer, cfg: BatteryConfig, i: int, freq: Freq, flags: Flags
-) -> BatteryOneInterval:
-    """Create Battery asset data for a single interval."""
-
-    return BatteryOneInterval(
-        cfg=cfg,
-        charge_mwh=optimizer.continuous(
-            f"charge_mwh-{i}", up=freq.mw_to_mwh(cfg.power_mw)
-        ),
-        discharge_mwh=optimizer.continuous(
-            f"discharge_mwh-{i}", up=freq.mw_to_mwh(cfg.power_mw)
-        ),
-        charge_binary=optimizer.binary(f"charge_binary-{i}")
-        if flags.include_charge_discharge_binary_variables
-        else 0,
-        discharge_binary=optimizer.binary(f"discharge_binary-{i}")
-        if flags.include_charge_discharge_binary_variables
-        else 0,
-        losses_mwh=optimizer.continuous(f"losses_mwh-{i}"),
-        initial_charge_mwh=optimizer.continuous(
-            f"initial_charge_mwh-{i}", low=0, up=cfg.capacity_mwh
-        ),
-        final_charge_mwh=optimizer.continuous(
-            f"final_charge_mwh-{i}", low=0, up=cfg.capacity_mwh
-        ),
-        efficiency_pct=cfg.efficiency_pct,
-    )
-
-
-def constrain_within_interval(
-    optimizer: Optimizer,
-    vars: collections.defaultdict,
-    configs: list[BatteryConfig],
-    flags: Flags,
-) -> None:
-    """Constrain battery dispatch within a single interval"""
-    constrain_only_charge_or_discharge(optimizer, vars, configs, flags)
-    constrain_battery_electricity_balance(optimizer, vars)
-    constrain_connection_batteries_between_intervals(optimizer, vars)
-
-
 def constrain_only_charge_or_discharge(
     optimizer: Optimizer,
     vars: collections.defaultdict,
-    configs: list[BatteryConfig],
     flags: Flags,
 ) -> None:
     """Constrain battery to only charge or discharge.
 
     Usually flagged off - slows things down a lot (~2x as slow).
     """
     if flags.include_charge_discharge_binary_variables:
-        for battery, cfg in zip(vars["batteries"][-1], configs, strict=True):
+        batteries = epl.utils.filter_assets(vars, "battery")
+        for battery in batteries:
             optimizer.constrain_max(
-                battery.charge_mwh, battery.charge_binary, cfg.capacity_mwh
+                battery.charge_mwh, battery.charge_binary, battery.cfg.capacity_mwh
             )
             optimizer.constrain_max(
-                battery.discharge_mwh, battery.discharge_binary, cfg.capacity_mwh
+                battery.discharge_mwh,
+                battery.discharge_binary,
+                battery.cfg.capacity_mwh,
             )
             optimizer.constrain(battery.charge_binary + battery.discharge_binary <= 1)
 
 
 def constrain_battery_electricity_balance(
     optimizer: Optimizer, vars: collections.defaultdict
 ) -> None:
     """Constrain energy balance in a single interval - also calculates losses."""
-    for battery in vars["batteries"][-1]:
+
+    assets = vars["assets"][-1]
+    batteries = [a for a in assets if isinstance(a, epl.battery.BatteryOneInterval)]
+
+    for battery in batteries:
         optimizer.constrain(
             battery.initial_charge_mwh
             + battery.charge_mwh
             - battery.discharge_mwh
             - battery.losses_mwh
             == battery.final_charge_mwh
         )
@@ -127,167 +91,212 @@
         )
 
 
 def constrain_connection_batteries_between_intervals(
     optimizer: Optimizer, vars: collections.defaultdict
 ) -> None:
     """Constrain battery dispatch between two adjacent intervals."""
-    batteries = vars["batteries"]
+    batteries = epl.utils.filter_all_assets(vars, "battery")
 
     #  if in first interval, do nothing
     #  could also do something based on `i` here...
     if len(batteries) < 2:
         return None
 
     else:
         old = batteries[-2]
         new = batteries[-1]
         for alt, neu in zip(old, new, strict=True):
             optimizer.constrain(alt.final_charge_mwh == neu.initial_charge_mwh)
 
 
-def constrain_after_intervals(
-    optimizer: Optimizer, vars: collections.defaultdict, configs: list[BatteryConfig]
-) -> None:
-    """Constrain battery dispatch after all interval asset models are created."""
-    constrain_initial_final_charge(optimizer, vars, configs)
-
-
 def constrain_initial_final_charge(
     optimizer: Optimizer,
     vars: collections.defaultdict,
-    battery_cfgs: list[BatteryConfig],
 ) -> None:
     """Constrain the battery state of charge at the start and end of the simulation."""
 
-    batteries = vars["batteries"]
-    first = batteries[0]
-    for battery, cfg in zip(first, battery_cfgs, strict=True):
-        optimizer.constrain(battery.initial_charge_mwh == cfg.initial_charge_mwh)
-
-    last = batteries[-1]
-    for battery, cfg in zip(last, battery_cfgs, strict=True):
-        optimizer.constrain(battery.final_charge_mwh == cfg.final_charge_mwh)
+    assets = vars["assets"][0]
+    first = [a for a in assets if isinstance(a, epl.battery.BatteryOneInterval)]
+    for battery in first:
+        optimizer.constrain(
+            battery.initial_charge_mwh == battery.cfg.initial_charge_mwh
+        )
+
+    assets = vars["assets"][-1]
+    last = [a for a in assets if isinstance(a, epl.battery.BatteryOneInterval)]
+    for battery in last:
+        optimizer.constrain(battery.final_charge_mwh == battery.cfg.final_charge_mwh)
 
 
 class Battery:
     """Battery asset - handles optimization and plotting of results over many intervals.
 
     Args:
         power_mw - the maximum power output of the battery in mega-watts, used for both charge and discharge.
         capacity_mwh - battery capacity in mega-watt hours.
         efficiency - round-trip efficiency of the battery, with a default value of 90% efficient.
         battery_name parameter represents the name of the battery, with a default value of "battery".
     """
 
     def __init__(
         self,
-        power_mw: float,
-        capacity_mwh: float,
+        power_mw: float = 2.0,
+        capacity_mwh: float = 4.0,
         efficiency: float = 0.9,
-        battery_name: str = "battery",
+        name: str = "battery",
     ):
         """Initialize a Battery asset model."""
         self.cfg = BatteryConfig(
-            name=battery_name,
+            name=name,
             power_mw=power_mw,
             capacity_mwh=capacity_mwh,
             efficiency_pct=efficiency,
         )
 
+    def __repr__(self) -> str:
+        """A string representation of self."""
+        return f"<energypylinear.Battery, power: {self.cfg.power_mw} MW, capacity: {self.cfg.capacity_mwh} MWh>"
+
+    def setup_initial_final_charge(
+        self, initial_charge_mwh: float, final_charge_mwh: float | None
+    ) -> None:
+        """Processes the options for initial and final charge."""
+        self.cfg.initial_charge_mwh = min(initial_charge_mwh, self.cfg.capacity_mwh)
+        self.cfg.final_charge_mwh = (
+            self.cfg.initial_charge_mwh
+            if final_charge_mwh is None
+            else min(final_charge_mwh, self.cfg.capacity_mwh)
+        )
+
+    def one_interval(
+        self, optimizer: Optimizer, i: int, freq: Freq, flags: Flags
+    ) -> BatteryOneInterval:
+        """Create Battery asset data for a single interval."""
+        return BatteryOneInterval(
+            cfg=self.cfg,
+            charge_mwh=optimizer.continuous(
+                f"{self.cfg.name}-charge_mwh-{i}", up=freq.mw_to_mwh(self.cfg.power_mw)
+            ),
+            discharge_mwh=optimizer.continuous(
+                f"{self.cfg.name}-discharge_mwh-{i}",
+                up=freq.mw_to_mwh(self.cfg.power_mw),
+            ),
+            charge_binary=optimizer.binary(f"{self.cfg.name}-charge_binary-{i}")
+            if flags.include_charge_discharge_binary_variables
+            else 0,
+            discharge_binary=optimizer.binary(f"{self.cfg.name}-discharge_binary-{i}")
+            if flags.include_charge_discharge_binary_variables
+            else 0,
+            losses_mwh=optimizer.continuous(f"{self.cfg.name}-losses_mwh-{i}"),
+            initial_charge_mwh=optimizer.continuous(
+                f"{self.cfg.name}-initial_charge_mwh-{i}",
+                low=0,
+                up=self.cfg.capacity_mwh,
+            ),
+            final_charge_mwh=optimizer.continuous(
+                f"{self.cfg.name}-final_charge_mwh-{i}", low=0, up=self.cfg.capacity_mwh
+            ),
+            efficiency_pct=self.cfg.efficiency_pct,
+        )
+
+    def constrain_within_interval(
+        self,
+        optimizer: Optimizer,
+        vars: collections.defaultdict,
+        interval_data: "epl.IntervalData",
+        i: int,
+        freq: Freq,
+        flags: Flags = Flags(),
+    ) -> None:
+        """Constrain Battery dispatch within a single interval"""
+        constrain_only_charge_or_discharge(optimizer, vars, flags)
+        constrain_battery_electricity_balance(optimizer, vars)
+        constrain_connection_batteries_between_intervals(optimizer, vars)
+
+    def constrain_after_intervals(
+        self,
+        optimizer: Optimizer,
+        vars: collections.defaultdict,
+        interval_data: "epl.IntervalData",
+    ) -> None:
+        """Constrain battery dispatch after all interval asset models are created."""
+        constrain_initial_final_charge(optimizer, vars)
+
     def optimize(
         self,
-        electricity_prices: np.ndarray,
-        gas_prices: typing.Union[None, np.ndarray] = None,
-        electricity_carbon_intensities: typing.Union[None, np.ndarray] = None,
-        #  should these go in here?  TODO
-        high_temperature_load_mwh: typing.Union[None, np.ndarray] = None,
-        low_temperature_load_mwh: typing.Union[None, np.ndarray] = None,
+        electricity_prices: np.ndarray | list[float],
+        gas_prices: np.ndarray | list[float] | None = None,
+        electricity_carbon_intensities: np.ndarray | list[float] | None = None,
         freq_mins: int = defaults.freq_mins,
         initial_charge_mwh: float = 0.0,
-        final_charge_mwh: typing.Union[float, None] = None,
+        final_charge_mwh: float | None = None,
         objective: str = "price",
-        allow_infeasible: bool = False,
         flags: Flags = Flags(),
-        verbose: int = 0,
+        verbose: bool = True,
     ) -> "epl.results.SimulationResult":
         """Optimize the battery's dispatch using a mixed-integer linear program.
 
         Args:
             electricity_prices: the price of electricity in each interval.
             gas_prices: the prices of natural gas, used in CHP and boilers in each interval.
             electricity_carbon_intensities: carbon intensity of electricity in each interval.
             high_temperature_load_mwh: high temperature load of the site in mega-watt hours.
             low_temperature_load_mwh: low temperature load of the site in mega-watt hours.
             freq_mins: the size of an interval in minutes.
             initial_charge_mwh: initial charge state of the battery in mega-watt hours.
             final_charge_mwh: final charge state of the battery in mega-watt hours.
             objective: the optimization objective - either "price" or "carbon".
-            allow_infeasible: whether to fail on infeasible linear programs.
             flags: boolean flags to change simulation and results behaviour.
             verbose: level of printing.
 
         Returns:
             epl.results.SimulationResult
         """
         self.optimizer = Optimizer()
         freq = Freq(freq_mins)
         interval_data = epl.interval_data.IntervalData(
             electricity_prices=electricity_prices,
             gas_prices=gas_prices,
             electricity_carbon_intensities=electricity_carbon_intensities,
-            high_temperature_load_mwh=high_temperature_load_mwh,
-            low_temperature_load_mwh=low_temperature_load_mwh,
         )
-        self.site_cfg = epl.assets.site.SiteConfig()
-        self.spill_cfg = epl.spill.SpillConfig()
-        self.valve_cfg = epl.valve.ValveConfig(name="valve")
+        self.site = epl.Site()
+        self.spill = epl.spill.Spill()
 
-        self.cfg.initial_charge_mwh = min(initial_charge_mwh, self.cfg.capacity_mwh)
-        self.cfg.final_charge_mwh = (
-            self.cfg.initial_charge_mwh
-            if final_charge_mwh is None
-            else min(final_charge_mwh, self.cfg.capacity_mwh)
-        )
+        self.setup_initial_final_charge(initial_charge_mwh, final_charge_mwh)
 
-        #  TODO - difficult to type the list of list thing
-        #  maybe sign something should be reworked with this `vars` dict
         vars: collections.defaultdict[str, typing.Any] = collections.defaultdict(list)
         for i in interval_data.idx:
-
             vars["sites"].append(
-                site.site_one_interval(self.optimizer, self.site_cfg, i, freq)
+                self.site.one_interval(self.optimizer, self.site.cfg, i, freq)
             )
-            vars["spills"].append(
-                epl.spill.spill_one_interval(self.optimizer, self.spill_cfg, i, freq)
+            vars["assets"].append(
+                [
+                    self.one_interval(self.optimizer, i, freq, flags),
+                    self.spill.one_interval(self.optimizer, i, freq),
+                ]
             )
-            vars["valves"].append(
-                epl.valve.valve_one_interval(self.optimizer, self.valve_cfg, i, freq)
+
+            self.site.constrain_within_interval(self.optimizer, vars, interval_data, i)
+            self.constrain_within_interval(
+                self.optimizer, vars, interval_data, i, freq, flags=flags
             )
-            batteries = [battery_one_interval(self.optimizer, self.cfg, i, freq, flags)]
-            vars["batteries"].append(batteries)
-            vars["assets"].append(batteries)
-
-            site.constrain_within_interval(self.optimizer, vars, interval_data, i)
-            constrain_within_interval(self.optimizer, vars, [self.cfg], flags)
-
-        constrain_after_intervals(self.optimizer, vars, [self.cfg])
-
-        assert (
-            len(interval_data.idx)
-            == len(vars["assets"])
-            == len(vars["batteries"])
-            == len(vars["sites"])
-        )
+
+        self.constrain_after_intervals(self.optimizer, vars, interval_data)
+
+        assert len(interval_data.idx) == len(vars["assets"]) == len(vars["sites"])
 
         objective_fn = epl.objectives[objective]
         self.optimizer.objective(objective_fn(self.optimizer, vars, interval_data))
-        _, feasible = self.optimizer.solve(verbose=verbose)
+        status = self.optimizer.solve(verbose=verbose)
+
         self.interval_data = interval_data
-        return epl.results.extract_results(interval_data, vars, feasible=feasible)
+        return epl.results.extract_results(
+            interval_data, vars, feasible=status.feasible, verbose=verbose
+        )
 
     def plot(
         self,
         results: "epl.results.SimulationResult",
         path: typing.Union[pathlib.Path, str],
     ) -> None:
         """Plot simulation results."""
```

### Comparing `energypylinear-0.1.1/energypylinear/assets/chp.py` & `energypylinear-0.1.2/energypylinear/assets/chp.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,23 +11,14 @@
 from energypylinear.assets.asset import AssetOneInterval
 from energypylinear.defaults import defaults
 from energypylinear.flags import Flags
 from energypylinear.freq import Freq
 from energypylinear.optimizer import Optimizer
 
 
-class BoilerConfig(AssetOneInterval):
-    """Gas boiler configuration."""
-
-    name: str
-    high_temperature_generation_max_mw: float = 0
-    high_temperature_generation_min_mw: float = 0
-    high_temperature_efficiency_pct: float = 0
-
-
 class GeneratorConfig(pydantic.BaseModel):
     """CHP generator configuration."""
 
     name: str
     electric_power_max_mw: float = 0
     electric_power_min_mw: float = 0
 
@@ -39,132 +30,25 @@
     @pydantic.validator("name")
     def check_name(cls, name: str) -> str:
         """Ensure we can identify this asset correctly."""
         assert "generator" in name
         return name
 
 
-class BoilerOneInterval(AssetOneInterval):
-    """Boiler data for a single interval."""
-
-    cfg: BoilerConfig
-    high_temperature_generation_mwh: pulp.LpVariable
-    gas_consumption_mwh: pulp.LpVariable
-    binary: pulp.LpVariable
-
-
 class GeneratorOneInterval(AssetOneInterval):
     """CHP generator data for a single interval."""
 
     electric_generation_mwh: pulp.LpVariable
     gas_consumption_mwh: pulp.LpVariable
     high_temperature_generation_mwh: pulp.LpVariable
     low_temperature_generation_mwh: pulp.LpVariable
     binary: pulp.LpVariable
     cfg: GeneratorConfig
 
 
-def boiler_one_interval(
-    optimizer: Optimizer, cfg: BoilerConfig, i: int, freq: Freq
-) -> BoilerOneInterval:
-    """Create Boiler asset data for a single interval."""
-    return BoilerOneInterval(
-        high_temperature_generation_mwh=optimizer.continuous(
-            f"{cfg.name}-high_temperature_generation_mwh-{i}",
-            low=freq.mw_to_mwh(cfg.high_temperature_generation_min_mw),
-            up=freq.mw_to_mwh(cfg.high_temperature_generation_max_mw),
-        ),
-        binary=optimizer.binary(
-            f"{cfg.name}-binary_mwh-{i}",
-        ),
-        gas_consumption_mwh=optimizer.continuous(f"{cfg.name}-gas_consumption_mwh-{i}"),
-        cfg=cfg,
-    )
-
-
-def generator_one_interval(
-    optimizer: Optimizer, cfg: GeneratorConfig, i: int, freq: Freq
-) -> GeneratorOneInterval:
-    """Create a Generator asset model for one interval."""
-    return GeneratorOneInterval(
-        electric_generation_mwh=optimizer.continuous(
-            f"{cfg.name}-electric_generation_mwh-{i}",
-            low=0,
-            up=freq.mw_to_mwh(cfg.electric_power_max_mw),
-        ),
-        binary=optimizer.binary(
-            f"{cfg.name}-binary_mwh-{i}",
-        ),
-        gas_consumption_mwh=optimizer.continuous(f"{cfg.name}-gas_consumption_mwh-{i}"),
-        high_temperature_generation_mwh=optimizer.continuous(
-            f"{cfg.name}-high_temperature_generation_mwh-{i}",
-            low=0,
-        ),
-        low_temperature_generation_mwh=optimizer.continuous(
-            f"{cfg.name}-low_temperature_generation_mwh-{i}",
-            low=0,
-        ),
-        cfg=cfg,
-    )
-
-
-def constrain_within_interval_boilers(
-    optimizer: Optimizer, vars: dict, freq: Freq
-) -> None:
-    """Constrain boiler upper and lower bounds for generating high & low temperature heat."""
-    for asset in vars["boilers"][-1]:
-        optimizer.constrain(
-            asset.gas_consumption_mwh
-            == asset.high_temperature_generation_mwh
-            * (1 / asset.cfg.high_temperature_efficiency_pct)
-        )
-
-        optimizer.constrain_max(
-            asset.high_temperature_generation_mwh,
-            asset.binary,
-            freq.mw_to_mwh(asset.cfg.high_temperature_generation_max_mw),
-        )
-        optimizer.constrain_min(
-            asset.high_temperature_generation_mwh,
-            asset.binary,
-            freq.mw_to_mwh(asset.cfg.high_temperature_generation_min_mw),
-        )
-
-
-def constrain_within_interval_generators(
-    optimizer: Optimizer, vars: dict, freq: Freq
-) -> None:
-    """Constrain generator upper and lower bounds for generating electricity, high & low temperature heat."""
-    for asset in vars["generators"][-1]:
-        optimizer.constrain(
-            asset.gas_consumption_mwh
-            == asset.electric_generation_mwh * (1 / asset.cfg.electric_efficiency_pct)
-        )
-        optimizer.constrain(
-            asset.high_temperature_generation_mwh
-            == asset.gas_consumption_mwh * asset.cfg.high_temperature_efficiency_pct
-        )
-        optimizer.constrain(
-            asset.low_temperature_generation_mwh
-            == asset.gas_consumption_mwh * asset.cfg.low_temperature_efficiency_pct
-        )
-        #  add cooling constraint here TODO
-
-        optimizer.constrain_max(
-            asset.electric_generation_mwh,
-            asset.binary,
-            freq.mw_to_mwh(asset.cfg.electric_power_max_mw),
-        )
-        optimizer.constrain_min(
-            asset.electric_generation_mwh,
-            asset.binary,
-            freq.mw_to_mwh(asset.cfg.electric_power_min_mw),
-        )
-
-
 class Generator:
     """CHP generator asset - handles optimization and plotting of results over many intervals.
 
     Args:
         electric_power_max_mw - maximum electric power output of the generator in mega-watts.
         electric_power_min_mw - minimum electric power output of the generator in mega-watts.
         electric_efficiency_pct - electric efficiency of the generator, measured in percentage.
@@ -177,33 +61,106 @@
     def __init__(
         self,
         electric_power_max_mw: float = 0.0,
         electric_power_min_mw: float = 0.0,
         electric_efficiency_pct: float = 0.0,
         high_temperature_efficiency_pct: float = 0.0,
         low_temperature_efficiency_pct: float = 0.0,
+        name: str = "generator",
     ):
         """Initialize a Battery asset model."""
         self.cfg = GeneratorConfig(
-            name="generator",
+            name=name,
             electric_power_min_mw=electric_power_min_mw,
             electric_power_max_mw=electric_power_max_mw,
             electric_efficiency_pct=electric_efficiency_pct,
             high_temperature_efficiency_pct=high_temperature_efficiency_pct,
             low_temperature_efficiency_pct=low_temperature_efficiency_pct,
         )
 
+    def one_interval(
+        self, optimizer: Optimizer, i: int, freq: Freq, flags: Flags = Flags()
+    ) -> GeneratorOneInterval:
+        """Create a Generator asset model for one interval."""
+        return GeneratorOneInterval(
+            electric_generation_mwh=optimizer.continuous(
+                f"{self.cfg.name}-electric_generation_mwh-{i}",
+                low=0,
+                up=freq.mw_to_mwh(self.cfg.electric_power_max_mw),
+            ),
+            binary=optimizer.binary(
+                f"{self.cfg.name}-binary_mwh-{i}",
+            ),
+            gas_consumption_mwh=optimizer.continuous(
+                f"{self.cfg.name}-gas_consumption_mwh-{i}"
+            ),
+            high_temperature_generation_mwh=optimizer.continuous(
+                f"{self.cfg.name}-high_temperature_generation_mwh-{i}",
+                low=0,
+            ),
+            low_temperature_generation_mwh=optimizer.continuous(
+                f"{self.cfg.name}-low_temperature_generation_mwh-{i}",
+                low=0,
+            ),
+            cfg=self.cfg,
+        )
+
+    def constrain_within_interval(
+        self,
+        optimizer: Optimizer,
+        vars: dict,
+        interval_data: "epl.IntervalData",
+        i: int,
+        freq: Freq,
+        flags: Flags = Flags(),
+    ) -> None:
+        """Constrain generator upper and lower bounds for generating electricity, high & low temperature heat."""
+        assets = vars["assets"][-1]
+        generators = [a for a in assets if isinstance(a, epl.chp.GeneratorOneInterval)]
+        for asset in generators:
+            if asset.cfg.electric_efficiency_pct > 0:
+                optimizer.constrain(
+                    asset.gas_consumption_mwh
+                    == asset.electric_generation_mwh
+                    * (1 / asset.cfg.electric_efficiency_pct)
+                )
+
+            optimizer.constrain(
+                asset.high_temperature_generation_mwh
+                == asset.gas_consumption_mwh * asset.cfg.high_temperature_efficiency_pct
+            )
+            optimizer.constrain(
+                asset.low_temperature_generation_mwh
+                == asset.gas_consumption_mwh * asset.cfg.low_temperature_efficiency_pct
+            )
+            #  add cooling constraint here TODO
+            optimizer.constrain_max(
+                asset.electric_generation_mwh,
+                asset.binary,
+                freq.mw_to_mwh(asset.cfg.electric_power_max_mw),
+            )
+            optimizer.constrain_min(
+                asset.electric_generation_mwh,
+                asset.binary,
+                freq.mw_to_mwh(asset.cfg.electric_power_min_mw),
+            )
+
+    def constrain_after_intervals(
+        self, *args: typing.Tuple[typing.Any], **kwargs: typing.Any
+    ) -> None:
+        """Constrain asset after all interval asset models are created."""
+        return
+
     def optimize(
         self,
         electricity_prices: typing.Union[np.ndarray, list[float]],
         gas_prices: typing.Union[None, np.ndarray, float] = None,
         electricity_carbon_intensities: typing.Union[
             None, np.ndarray, list[float], float
         ] = None,
-        #  should these go in here?  TODO
         high_temperature_load_mwh: typing.Union[None, np.ndarray, list[float]] = None,
         low_temperature_load_mwh: typing.Union[None, np.ndarray, list[float]] = None,
         freq_mins: int = defaults.freq_mins,
         objective: str = "price",
         flags: Flags = Flags(),
     ) -> "epl.results.SimulationResult":
         """
@@ -224,70 +181,63 @@
         interval_data = epl.interval_data.IntervalData(
             electricity_prices=electricity_prices,
             gas_prices=gas_prices,
             electricity_carbon_intensities=electricity_carbon_intensities,
             high_temperature_load_mwh=high_temperature_load_mwh,
             low_temperature_load_mwh=low_temperature_load_mwh,
         )
-        self.site_cfg = epl.site.SiteConfig()
-        self.spill_cfg = epl.spill.SpillConfig()
-        self.valve_cfg = epl.valve.ValveConfig(name="valve")
+        self.site = epl.Site()
+        self.spill = epl.spill.Spill()
+        self.valve = epl.valve.Valve()
 
+        assert interval_data.high_temperature_load_mwh is not None
+        assert interval_data.low_temperature_load_mwh is not None
         default_boiler_size = freq.mw_to_mwh(
             max(interval_data.high_temperature_load_mwh)
             + max(interval_data.low_temperature_load_mwh)
         )
-        self.default_boiler_cfg = BoilerConfig(
-            name="boiler",
+        self.boiler = epl.Boiler(
             high_temperature_generation_max_mw=default_boiler_size,
             high_temperature_efficiency_pct=defaults.default_boiler_efficiency_pct,
         )
 
-        #  TODO - difficult to type the list of list thing
-        #  maybe sign something should be reworked
         vars: collections.defaultdict[str, typing.Any] = collections.defaultdict(list)
         for i in interval_data.idx:
             vars["sites"].append(
-                epl.site.site_one_interval(self.optimizer, self.site_cfg, i, freq)
+                self.site.one_interval(self.optimizer, self.site.cfg, i, freq)
+            )
+            vars["assets"].append(
+                [
+                    self.one_interval(self.optimizer, i, freq),
+                    self.boiler.one_interval(self.optimizer, i, freq),
+                    self.valve.one_interval(self.optimizer, i, freq),
+                    self.spill.one_interval(self.optimizer, i, freq),
+                ]
             )
-            vars["spills"].append(
-                epl.spill.spill_one_interval(self.optimizer, self.spill_cfg, i, freq)
+
+            self.site.constrain_within_interval(self.optimizer, vars, interval_data, i)
+            self.constrain_within_interval(self.optimizer, vars, interval_data, i, freq)
+            self.boiler.constrain_within_interval(
+                self.optimizer, vars, interval_data, i, freq
             )
-            vars["valves"].append(
-                epl.valve.valve_one_interval(self.optimizer, self.valve_cfg, i, freq)
+            self.valve.constrain_within_interval(
+                self.optimizer, vars, interval_data, i, freq
+            )
+            self.spill.constrain_within_interval(
+                self.optimizer, vars, interval_data, i, freq
             )
 
-            generators = [
-                generator_one_interval(self.optimizer, self.cfg, i, freq),
-            ]
-            boilers = [
-                boiler_one_interval(self.optimizer, self.default_boiler_cfg, i, freq),
-            ]
-            vars["generators"].append(generators)
-            vars["boilers"].append(boilers)
-            vars["assets"].append([*generators, *boilers])
-
-            epl.site.constrain_within_interval(self.optimizer, vars, interval_data, i)
-            constrain_within_interval_generators(self.optimizer, vars, freq)
-            constrain_within_interval_boilers(self.optimizer, vars, freq)
-            epl.valve.constrain_within_interval_valve(self.optimizer, vars)
-
-        assert (
-            len(interval_data.idx)
-            == len(vars["assets"])
-            == len(vars["generators"])
-            == len(vars["boilers"])
-        )
+        assert len(interval_data.idx) == len(vars["assets"])
 
         objective_fn = epl.objectives[objective]
         self.optimizer.objective(objective_fn(self.optimizer, vars, interval_data))
-        _, feasible = self.optimizer.solve()
+        status = self.optimizer.solve()
         self.interval_data = interval_data
         return epl.results.extract_results(
-            interval_data, vars, feasible=feasible, flags=flags
+            interval_data, vars, feasible=status.feasible, flags=flags
         )
 
     def plot(
         self,
         results: "epl.results.SimulationResult",
         path: typing.Union[pathlib.Path, str],
     ) -> None:
```

### Comparing `energypylinear-0.1.1/energypylinear/assets/evs.py` & `energypylinear-0.1.2/energypylinear/assets/evs.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,48 +4,60 @@
 import typing
 
 import numpy as np
 import pulp
 import pydantic
 
 import energypylinear as epl
-from energypylinear.assets import site
 from energypylinear.assets.asset import AssetOneInterval
 from energypylinear.defaults import defaults
+from energypylinear.flags import Flags
 from energypylinear.freq import Freq
 from energypylinear.optimizer import Optimizer
 
 
 class ChargerConfig(pydantic.BaseModel):
-    """Electric vehicle (EV) charger asset configuration."""
+    """Electric vehicle (EV) single charger asset configuration."""
 
     name: str
     power_max_mw: float
     power_min_mw: float
 
 
+class EVsConfig(pydantic.BaseModel):
+    """Electric vehicle (EV) asset configuration."""
+
+    name: str
+
+    @pydantic.validator("name")
+    def check_name(cls, name: str) -> str:
+        """Ensure we can identify this asset correctly."""
+        assert "evs" in name
+        return name
+
+
 class EVOneInterval(AssetOneInterval):
     """EV asset data for a single interval"""
 
     #  could use `electric_charge_mwh`
-    #  or event electric_load_mwh
+    #  or even electric_load_mwh
     charge_mwh: pulp.LpVariable
     charge_binary: pulp.LpVariable
 
     class Config:
         """pydantic.BaseModel configuration."""
 
         arbitrary_types_allowed = True
 
 
 class EVsArrayOneInterval(AssetOneInterval):
     """EV asset for a single interval as a 2D array.."""
 
     #  could use `electric_charge_mwh`
-    #  or event electric_load_mwh
+    #  or even electric_load_mwh
     charge_mwh: np.ndarray
     charge_binary: np.ndarray
     charger_cfgs: np.ndarray
 
     class Config:
         """pydantic.BaseModel configuration."""
 
@@ -119,27 +131,26 @@
     n_chargers = chargers.shape[0]
 
     for charge_event_idx in range(n_charge_events):
         for charger_idx, charger in enumerate(chargers):
             #  add the connection between the contiunous and binary variables
             continuous = evs.charge_mwh[0, charge_event_idx, charger_idx]
             binary = evs.charge_binary[0, charge_event_idx, charger_idx]
-
             optimizer.constrain_max(
                 continuous, binary, freq.mw_to_mwh(charger.power_max_mw)
             )
             optimizer.constrain_min(
                 continuous, binary, freq.mw_to_mwh(charger.power_min_mw)
             )
             #  only let the binary be positive when the charge_event is positive
             #  this forces the charger to only charge during a charge event
             optimizer.constrain(binary <= charge_event[i, charge_event_idx])
 
     #  required to handle the spill charger case
-    #  where we don't want to limit it
+    #  where we don't want to limit the matching of chargers and charge events
     if add_single_charger_or_event_constraints is True:
 
         #  constrain to only one charger per charging event
         #  sum across all chargers for one charge event <= 1
         for charge_event_idx in range(n_charge_events):
             optimizer.constrain(
                 optimizer.sum(evs.charge_binary[0, charge_event_idx, :].tolist()) <= 1
@@ -161,15 +172,14 @@
 ) -> None:
     """Constrain chargers after all intervals over."""
     assert interval_data.evs
 
     stacked_charge_mwh = stack_ev(vars, "charge_mwh")
 
     #  check the stack worked correctly
-    #  TODO move after interval data refactor
     stacked_charge_mwh = stack_ev(vars, "charge_mwh")
     assert stacked_charge_mwh.shape[0] == len(interval_data.idx)
     assert isinstance(interval_data.evs.charge_events, np.ndarray)
     assert stacked_charge_mwh.shape[1] == interval_data.evs.charge_events.shape[1]
     assert (
         stacked_charge_mwh.shape[2]
         == charger_cfgs.shape[0] + spill_charger_config.shape[0]
@@ -195,17 +205,24 @@
     """EV asset class - handles optimization and plotting of results over many intervals.
 
     Args:
         charger_mws - size of EV chargers in mega-watts.
         charger_turndown - minimum charger output defined by the charger_turndown as a percent of the charger size in mega-watts.
     """
 
-    def __init__(self, charger_mws: list[float], charger_turndown: float = 0.1):
+    def __init__(
+        self,
+        charger_mws: list[float],
+        charger_turndown: float = 0.1,
+        name: str = "evs",
+    ):
         """Initialize an electric vehicle asset model."""
 
+        self.cfg = EVsConfig(name=name)
+
         self.charger_cfgs = np.array(
             [
                 ChargerConfig(
                     name=f"charger-{name}",
                     power_max_mw=power_mw,
                     power_min_mw=power_mw * charger_turndown,
                 )
@@ -218,27 +235,91 @@
                     name="charger-spill",
                     power_max_mw=defaults.spill_charge_max_mw,
                     power_min_mw=0,
                 )
             ]
         )
 
+    def one_interval(
+        self, optimizer: Optimizer, i: int, freq: Freq, flags: Flags = Flags()
+    ) -> tuple:
+        """Create EV asset data for a single interval."""
+        assert self.interval_data.evs is not None
+        assert self.interval_data.evs.charge_events is not None
+
+        evs, evs_array = evs_one_interval(
+            optimizer,
+            self.charger_cfgs,
+            np.array(self.interval_data.evs.charge_events),
+            i,
+            freq,
+        )
+        spill_evs, spill_evs_array = evs_one_interval(
+            optimizer,
+            self.spill_charger_config,
+            np.array(self.interval_data.evs.charge_events),
+            i,
+            freq,
+        )
+        return evs, evs_array, spill_evs, spill_evs_array
+
+    def constrain_within_interval(
+        self,
+        optimizer: Optimizer,
+        vars: collections.defaultdict,
+        interval_data: "epl.IntervalData",
+        i: int,
+        freq: Freq,
+        flags: Flags = Flags(),
+    ) -> None:
+        """Constrain EVs dispatch within a single interval"""
+        evs_array = vars["evs-array"][i]
+        assert self.interval_data.evs is not None
+        constrain_within_interval(
+            optimizer,
+            evs_array,
+            self.interval_data.evs.charge_events,
+            freq,
+            self.charger_cfgs,
+            i,
+        )
+        spill_evs_array = vars["spill-evs-array"][i]
+        constrain_within_interval(
+            optimizer,
+            spill_evs_array,
+            self.interval_data.evs.charge_events,
+            freq,
+            self.spill_charger_config,
+            i,
+            add_single_charger_or_event_constraints=False,
+        )
+
+    def constrain_after_intervals(
+        self,
+        optimizer: Optimizer,
+        vars: collections.defaultdict,
+        interval_data: "epl.IntervalData",
+    ) -> None:
+        """Constrain EVs after all interval asset models are created."""
+        constrain_after_intervals(
+            optimizer, vars, interval_data, self.charger_cfgs, self.spill_charger_config
+        )
+
     def optimize(
         self,
         charge_events: typing.Union[list[list[int]], np.ndarray],
         charge_event_mwh: typing.Union[list[int], np.ndarray],
         electricity_prices: typing.Union[np.ndarray, list[float]],
         gas_prices: typing.Union[None, np.ndarray, float] = None,
         electricity_carbon_intensities: typing.Union[
             None, np.ndarray, list[float], float
         ] = None,
-        high_temperature_load_mwh: typing.Union[None, np.ndarray, list[float]] = None,
-        low_temperature_load_mwh: typing.Union[None, np.ndarray, list[float]] = None,
         freq_mins: int = defaults.freq_mins,
         objective: str = "price",
+        verbose: int = 0,
     ) -> "epl.results.SimulationResult":
         """Optimize the EVs's dispatch using a mixed-integer linear program.
 
         Args:
             charge_events: 2D matrix representing when a charge event is active.
                 Shape is (n_charge_events, n_timesteps).
                 A charge events matrix for 4 charge events over 5 intervals.
@@ -258,15 +339,15 @@
                 ```
 
             electricity_prices - the price of electricity in each interval.
             gas_prices - the prices of natural gas, used in CHP and boilers in each interval.
             electricity_carbon_intensities - carbon intensity of electricity in each interval.
             freq_mins - the size of an interval in minutes.
             objective - the optimization objective - either "price" or "carbon".
-            allow_infeasible: whether to fail on infeasible linear programs.
+            verbose: level of printing.
 
         Returns:
             epl.results.SimulationResult
         """
         self.optimizer = Optimizer()
         freq = Freq(freq_mins)
 
@@ -282,88 +363,69 @@
             electricity_carbon_intensities=electricity_carbon_intensities,
             evs=epl.interval_data.EVIntervalData(
                 charge_events=charge_events,
                 charge_event_mwh=charge_event_mwh,
             ),
         )
         assert interval_data.evs
-        self.site_cfg = epl.assets.site.SiteConfig()
-        self.spill_cfg = epl.spill.SpillConfig()
-        self.valve_cfg = epl.valve.ValveConfig(name="valve")
+        self.site = epl.Site()
+        self.spill = epl.spill.Spill()
+
+        #  needed in self.one_interval
+        self.interval_data = interval_data
 
-        #  TODO - difficult to type the list of list thing
-        #  maybe sign something should be reworked
         vars: collections.defaultdict[str, typing.Any] = collections.defaultdict(list)
         for i in interval_data.idx:
             vars["sites"].append(
-                site.site_one_interval(self.optimizer, self.site_cfg, i, freq)
-            )
-            vars["spills"].append(
-                epl.spill.spill_one_interval(self.optimizer, self.spill_cfg, i, freq)
+                self.site.one_interval(self.optimizer, self.site.cfg, i, freq)
             )
-            vars["valves"].append(
-                epl.valve.valve_one_interval(self.optimizer, self.valve_cfg, i, freq)
-            )
-
             assert isinstance(interval_data.evs.charge_events, np.ndarray)
-            evs, evs_array = evs_one_interval(
+            evs, evs_array, spill_evs, spill_evs_array = self.one_interval(
                 self.optimizer,
-                self.charger_cfgs,
-                interval_data.evs.charge_events,
                 i,
                 freq,
             )
-            spill_evs, spill_evs_array = evs_one_interval(
-                self.optimizer,
-                self.spill_charger_config,
-                interval_data.evs.charge_events,
-                i,
-                freq,
-            )
-            vars["evs"].append(evs)
+
+            #  should get rid of all these and just use `assets`
+            #  reason to use the separate keys is that we don't want
+            #  both evs_array and evs in assets for epl.Site
             vars["evs-array"].append(evs_array)
-            vars["spill-evs"].append(spill_evs)
             vars["spill-evs-array"].append(spill_evs_array)
-            vars["assets"].append([*evs, *spill_evs])
-
-            site.constrain_within_interval(self.optimizer, vars, interval_data, i)
-            constrain_within_interval(
-                self.optimizer,
-                evs_array,
-                interval_data.evs.charge_events,
-                freq,
-                self.charger_cfgs,
-                i,
+            vars["assets"].append(
+                [
+                    *evs,
+                    *spill_evs,
+                    self.spill.one_interval(self.optimizer, i, freq),
+                ]
             )
-            constrain_within_interval(
-                self.optimizer,
-                spill_evs_array,
-                interval_data.evs.charge_events,
-                freq,
-                self.spill_charger_config,
-                i,
-                add_single_charger_or_event_constraints=False,
+
+            self.site.constrain_within_interval(self.optimizer, vars, interval_data, i)
+
+            self.constrain_within_interval(
+                self.optimizer, vars, interval_data, i, freq=freq
             )
 
         assert isinstance(interval_data.evs.charge_events, np.ndarray)
         assert isinstance(self.charger_cfgs, np.ndarray)
         assert isinstance(self.spill_charger_config, np.ndarray)
-        constrain_after_intervals(
+        self.constrain_after_intervals(
             self.optimizer,
             vars,
             interval_data,
-            self.charger_cfgs,
-            self.spill_charger_config,
+            # self.charger_cfgs,
+            # self.spill_charger_config,
         )
 
         objective_fn = epl.objectives[objective]
         self.optimizer.objective(objective_fn(self.optimizer, vars, interval_data))
-        _, feasible = self.optimizer.solve()
+        status = self.optimizer.solve(verbose=verbose)
         self.interval_data = interval_data
-        return epl.results.extract_results(interval_data, vars, feasible=feasible)
+        return epl.results.extract_results(
+            interval_data, vars, feasible=status.feasible
+        )
 
     def plot(
         self,
         results: "epl.results.SimulationResult",
         path: typing.Union[pathlib.Path, str],
     ) -> None:
         """Plot simulation results."""
```

### Comparing `energypylinear-0.1.1/energypylinear/assets/valve.py` & `energypylinear-0.1.2/energypylinear/assets/valve.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Valve asset for allowing heat to flow from high to low temperature.
 
 This allows high temperature heat generated by either gas boilers or
 CHP generators to be used for low temperature heat consumption.
 """
+import typing
+
 import pulp
 import pydantic
 
 import energypylinear as epl
 from energypylinear.assets.asset import AssetOneInterval
 
 
@@ -26,33 +28,56 @@
     """Valve asset data for a single interval."""
 
     cfg: ValveConfig
     high_temperature_load_mwh: pulp.LpVariable
     low_temperature_generation_mwh: pulp.LpVariable
 
 
-def valve_one_interval(
-    optimizer: "epl.optimizer.Optimizer",
-    cfg: ValveConfig,
-    i: int,
-    freq: "epl.freq.Freq",
-) -> ValveOneInterval:
-    """Create Valve asset data for a single interval."""
-    return ValveOneInterval(
-        cfg=cfg,
-        high_temperature_load_mwh=optimizer.continuous(
-            f"{cfg.name}-high_temperature_load_mwh-{i}", low=0
-        ),
-        low_temperature_generation_mwh=optimizer.continuous(
-            f"{cfg.name}-low_temperature_generation_mwh-{i}", low=0
-        ),
-    )
-
-
-def constrain_within_interval_valve(
-    optimizer: "epl.optimizer.Optimizer", vars: dict
-) -> None:
-    """Constrain thermal balance across the valve."""
-    valve = vars["valves"][-1]
-    optimizer.constrain(
-        valve.high_temperature_load_mwh == valve.low_temperature_generation_mwh
-    )
+class Valve:
+    """Spill asset - allows heat to flow from high to low temperature."""
+
+    def __init__(self, name: str = "valve"):
+        """Initialize a Valve asset model."""
+        self.cfg = ValveConfig(name=name)
+
+    def __repr__(self) -> str:
+        """A string representation of self."""
+        return "<energypylinear.Valve>"
+
+    def one_interval(
+        self,
+        optimizer: "epl.optimizer.Optimizer",
+        i: int,
+        freq: "epl.freq.Freq",
+        flags: epl.flags.Flags = epl.flags.Flags(),
+    ) -> ValveOneInterval:
+        """Create Valve asset data for a single interval."""
+        return ValveOneInterval(
+            cfg=self.cfg,
+            high_temperature_load_mwh=optimizer.continuous(
+                f"{self.cfg.name}-high_temperature_load_mwh-{i}", low=0
+            ),
+            low_temperature_generation_mwh=optimizer.continuous(
+                f"{self.cfg.name}-low_temperature_generation_mwh-{i}", low=0
+            ),
+        )
+
+    def constrain_within_interval(
+        self,
+        optimizer: "epl.optimizer.Optimizer",
+        vars: dict,
+        interval_data: "epl.IntervalData",
+        i: int,
+        freq: "epl.freq.Freq",
+        flags: epl.flags.Flags = epl.flags.Flags(),
+    ) -> None:
+        """Constrain thermal balance across the valve."""
+        valve = epl.utils.filter_assets(vars, "valve")[-1]
+        optimizer.constrain(
+            valve.high_temperature_load_mwh == valve.low_temperature_generation_mwh
+        )
+
+    def constrain_after_intervals(
+        self, *args: typing.Any, **kwargs: typing.Any
+    ) -> None:
+        """Constrain asset after all interval asset models are created."""
+        return
```

### Comparing `energypylinear-0.1.1/energypylinear/data_generation.py` & `energypylinear-0.1.2/energypylinear/data_generation.py`

 * *Files identical despite different names*

### Comparing `energypylinear-0.1.1/energypylinear/defaults.py` & `energypylinear-0.1.2/energypylinear/defaults.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,21 +8,25 @@
     electricity_prices: float = 100.0
     electricity_carbon_intensities: float = 0.1
     gas_prices: float = 20
     freq_mins: int = 60
 
     high_temperature_load_mwh: float = 0
     low_temperature_load_mwh: float = 0
+    electricity_load_mwh: float = 0
 
     #   setting this too high will break the evs... was as 1e10
     spill_objective_penalty: float = 1e11
 
     default_boiler_efficiency_pct: float = 0.8
 
     gas_carbon_intensity: float = 0.185
 
     spill_charge_max_mw: float = 1e4
 
     decimal_tolerance: int = 4
 
+    #  used for < 0 stuff
+    epsilon: float = -1e-8
+
 
 defaults = Defaults()
```

### Comparing `energypylinear-0.1.1/energypylinear/freq.py` & `energypylinear-0.1.2/energypylinear/freq.py`

 * *Files identical despite different names*

### Comparing `energypylinear-0.1.1/energypylinear/interval_data.py` & `energypylinear-0.1.2/energypylinear/interval_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         charge_event_mwh: total energy consumption in each time step
 
     Methods:
         setup_idx: sets up the index of the time steps based on the shape of `charge_events`
         validate_all_things: validates the input data
     """
 
-    charge_events: typing.Union[list[list[int]], np.ndarray]
+    charge_events: np.ndarray
     idx: typing.Any = []
     charge_event_mwh: typing.Union[list[int], np.ndarray]
 
     class Config:
         """pydantic.BaseModel configuration."""
 
         arbitrary_types_allowed = True
@@ -101,34 +101,41 @@
     Methods:
         validate_evs: validates the EVIntervalData instance,
         validate_all_things: validates the input data,
         setup_idx: sets up the index of the time steps based on the length of `electricity_prices`.
     """
 
     electricity_prices: np.ndarray
-    electricity_carbon_intensities: typing.Union[np.ndarray, None]
-    gas_prices: np.ndarray
-    high_temperature_load_mwh: np.ndarray
-    low_temperature_load_mwh: np.ndarray
+    electricity_carbon_intensities: typing.Optional[np.ndarray] = None
+    gas_prices: typing.Optional[np.ndarray] = None
+    high_temperature_load_mwh: typing.Optional[np.ndarray] = None
+    low_temperature_load_mwh: typing.Optional[np.ndarray] = None
+    electricity_load_mwh: typing.Optional[np.ndarray] = None
     idx: list[int] = []
 
     evs: typing.Union[EVIntervalData, None] = None
 
     class Config:
         """pydantic.BaseModel configuration."""
 
         arbitrary_types_allowed = True
 
+    def __str__(self) -> str:
+        """A string representation of self."""
+        return f"<epl.IntervalData n: {self.electricity_prices.shape[0]} electricity_prices: {self.electricity_prices.mean():2.1f}>"
+
     @pydantic.validator("evs")
     def validate_evs(
         cls, evs: "epl.interval_data.EVIntervalData", values: dict
-    ) -> "epl.interval_data.EVIntervalData":
+    ) -> typing.Optional["epl.interval_data.EVIntervalData"]:
         """Validate our indexes are the same with our parent index."""
-        assert all(evs.idx == values["idx"])
-        return evs
+        if evs:
+            assert all(evs.idx == values["idx"])
+            return evs
+        return None
 
     @pydantic.root_validator(pre=True)
     def validate_all_things(cls, values: dict) -> dict:
         """Validate all input data in a single step."""
         base_field = "electricity_prices"
         prices = values[base_field]
 
@@ -139,14 +146,15 @@
             values[base_field] = np.array(prices)
 
         fields = [
             "gas_prices",
             "electricity_carbon_intensities",
             "high_temperature_load_mwh",
             "low_temperature_load_mwh",
+            "electricity_load_mwh",
         ]
         for field in fields:
             value = values.get(field)
             if isinstance(value, (float, int)):
                 values[field] = np.array([value] * len(values[base_field]))
 
             elif value is None:
@@ -161,23 +169,21 @@
             assert values[field] is not None
             assert isinstance(values[field], np.ndarray)
             assert np.isnan(values[field]).sum() == 0
 
         return values
 
     @pydantic.validator("idx", always=True)
-    def setup_idx(cls, value: list, values: dict) -> list:
+    def setup_idx(cls, _: list, values: dict) -> list:
         """Create an integer index."""
         return list(range(len(values["electricity_prices"])))
 
     def to_dataframe(self) -> pd.DataFrame:
         """Save all interval data to a pandas DataFrame."""
         data = self.dict()
-
         expected_len = len(data["idx"])
-
         df = {}
         for name, data in data.items():
             if data is not None:
                 if len(data) == expected_len:
                     df[name] = data
         return pd.DataFrame(df)
```

### Comparing `energypylinear-0.1.1/energypylinear/objectives.py` & `energypylinear-0.1.2/energypylinear/objectives.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,37 +23,36 @@
         interval_data: interaval data used in the simulation.
 
     Returns:
         A linear programming objective as an instance of `pulp.LpAffineExpression` class.
     """
 
     sites = vars["sites"]
-    spills = vars["spills"]
+    spills = epl.utils.filter_all_assets(vars, "spill")
     spill_evs = vars["spill-evs"]
-    generators = vars.get("generators", [])
-    boilers = vars.get("boilers", [])
+    boilers = epl.utils.filter_all_assets(vars, "boiler")
+    generators = epl.utils.filter_all_assets(vars, "generator")
 
-    if len(generators) == 0:
-        generators = [[epl.assets.asset.AssetOneInterval()] for i in interval_data.idx]
-    if len(boilers) == 0:
-        boilers = [[epl.assets.asset.AssetOneInterval()] for i in interval_data.idx]
     if len(spill_evs) == 0:
         spill_evs = [[epl.assets.asset.AssetOneInterval()] for i in interval_data.idx]
 
     assert isinstance(interval_data.gas_prices, np.ndarray)
     assert isinstance(interval_data.electricity_prices, np.ndarray)
 
     obj = [
         sites[i].import_power_mwh * interval_data.electricity_prices[i]
         - sites[i].export_power_mwh * interval_data.electricity_prices[i]
-        + spills[i].electric_generation_mwh * defaults.spill_objective_penalty
-        + spills[i].high_temperature_generation_mwh * defaults.spill_objective_penalty
-        + spills[i].electric_load_mwh * defaults.spill_objective_penalty
-        #  dumping heat has no penalty
-        + spills[i].high_temperature_load_mwh
+        + [
+            spill.electric_generation_mwh * defaults.spill_objective_penalty
+            + spill.high_temperature_generation_mwh * defaults.spill_objective_penalty
+            + spill.electric_load_mwh * defaults.spill_objective_penalty
+            #  don't think I need this - this is dumping of HT heat - was in here - TODO test
+            # + spill.high_temperature_load_mwh
+            for spill in spills[i]
+        ]
         + [
             spill_ev.charge_mwh * defaults.spill_objective_penalty
             for spill_ev in spill_evs[i]
         ]
         + [
             generator.gas_consumption_mwh * interval_data.gas_prices[i]
             for generator in generators[i]
@@ -84,28 +83,31 @@
         interval_data: interaval data used in the simulation.
 
     Returns:
         A linear programming objective as an instance of `pulp.LpAffineExpression` class.
     """
 
     sites = vars["sites"]
-    spills = vars["spills"]
-    generators = vars.get("generators", [])
-    boilers = vars.get("boilers", [])
+    spills = epl.utils.filter_all_assets(vars, "spill")
+    boilers = epl.utils.filter_all_assets(vars, "boiler")
+    generators = epl.utils.filter_all_assets(vars, "generator")
 
     assert isinstance(interval_data.electricity_carbon_intensities, np.ndarray)
     obj = [
         sites[i].import_power_mwh * interval_data.electricity_carbon_intensities[i]
         - sites[i].export_power_mwh * interval_data.electricity_carbon_intensities[i]
-        #  could turn this off TODO
-        + spills[i].electric_generation_mwh * defaults.spill_objective_penalty
-        + spills[i].high_temperature_generation_mwh * defaults.spill_objective_penalty
-        + spills[i].electric_load_mwh * defaults.spill_objective_penalty
-        #  dumping heat has no penalty
-        + spills[i].high_temperature_load_mwh
+        + [
+            spill.electric_generation_mwh * defaults.spill_objective_penalty
+            + spill.high_temperature_generation_mwh * defaults.spill_objective_penalty
+            + spill.electric_load_mwh * defaults.spill_objective_penalty
+            #  dumping heat has no penalty
+            #  so high_temperature_load_mwh and low_temperature_load_mwh
+            #  are not included here
+            for spill in spills[i]
+        ]
         for i in interval_data.idx
     ]
     if generators:
         obj += [
             generator.gas_consumption_mwh * defaults.gas_carbon_intensity
             for i in interval_data.idx
             for generator in generators[i]
```

### Comparing `energypylinear-0.1.1/energypylinear/optimizer.py` & `energypylinear-0.1.2/energypylinear/optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 """
 Interface to the `pulp` optimization library to solve linear programming problems.
 
 The `Optimizer` allows creating linear constraints, variables, and objectives, along with a linear program solver.
 """
+import dataclasses
 import typing
 
 import pulp
 
 
+@dataclasses.dataclass
+class OptimizationStatus:
+    """Result of a linear program optimization."""
+
+    status: str
+    feasible: bool
+
+
 class Optimizer:
     """
     Solver for linear programs. Interfaces with `pulp`.
 
     Attributes:
         prob: problem to be optimized.
         solver: solver to use for solving the optimization problem.
     """
 
     def __init__(self) -> None:
         """Initialize an Optimizer."""
         self.prob = pulp.LpProblem("prob", pulp.LpMinimize)
         self.solver = pulp.PULP_CBC_CMD(msg=0)
 
+    def __repr__(self) -> str:
+        """A string representation of self."""
+        return f"<energypylinear.Optimizer variables: {len(self.variables())} constraints: {len(self.constraints())}>"
+
     def continuous(
-        self, name: str, low: float = 0, up: typing.Optional[float] = None
+        self, name: str, low: float = 0, up: float | None = None
     ) -> pulp.LpVariable:
         """Creates a new continuous linear programming variable.
 
         Args:
             name: The name of the variable.
             low: The lower bound of the variable.
             up: The upper bound of the variable.
@@ -47,15 +60,15 @@
 
         Args:
             vector: list of `LpAffineExpression` objects to sum.
         """
         return pulp.lpSum(vector)
 
     def constrain(
-        self, constraint: pulp.LpConstraint, name: typing.Optional[str] = None
+        self, constraint: pulp.LpConstraint, name: str | None = None
     ) -> pulp.LpConstraint:
         """Create a linear program constrain.
 
         Args:
             constraint: equality or inequality expression.
             name: optional name to give to the constraint.
         """
@@ -67,37 +80,33 @@
         Args:
             objective: cost function to optimize.
         """
         return self.prob.setObjective(objective)
 
     def solve(
         self, verbose: int = 0, allow_infeasible: bool = False
-    ) -> tuple[str, bool]:
+    ) -> OptimizationStatus:
         """Solve the optimization problem.
 
         Args:
             verbose: a flag indicating how verbose the output should be.  0 for no output.
             allow_infeasible: whether an infeasible solution should raise an error.
-
-        Returns:
-            status: optimization status like `Optimial` or `Infeasible`
-            feasible: whether optimization was feasible or not.
         """
         self.assert_no_duplicate_variables()
         self.solver.solve(self.prob)
 
         status = self.status()
         if verbose > 0:
             print(f"status is {status}")
 
         feasible = status == "Optimal"
         if not allow_infeasible:
             assert feasible
 
-        return status, feasible
+        return OptimizationStatus(status=status, feasible=feasible)
 
     def assert_no_duplicate_variables(self) -> None:
         """Check there are no duplicate variable names in the optimization problem."""
         variables = self.variables()
         names = [v.name for v in variables]
         assert len(names) == len(
             set(names)
```

### Comparing `energypylinear-0.1.1/energypylinear/plot.py` & `energypylinear-0.1.2/energypylinear/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,31 +15,38 @@
 def find_column(df: pd.DataFrame, start: str, end: str) -> str:
     """Finds a column based on the start and end of the column name."""
     cols = [c for c in df.columns if c.startswith(start) and c.endswith(end)]
     assert len(cols) == 1
     return cols[0]
 
 
-def plot_battery(results: "epl.results.SimulationResult", path: pathlib.Path) -> None:
+def plot_battery(
+    results: "epl.results.SimulationResult", path: pathlib.Path | str
+) -> None:
     """Plot battery simulation results."""
+    path = pathlib.Path(path)
+    path.parent.mkdir(exist_ok=True, parents=True)
+
     fig, axes = plt.subplots(nrows=5, sharex=True, figsize=(12, 8))
     simulation = results.simulation
 
     simulation["Index"] = np.arange(simulation.shape[0]).tolist()
 
     simulation["import-export-balance"] = (
-        simulation["import_power_mwh"] - simulation["export_power_mwh"]
+        simulation["site-import_power_mwh"] - simulation["site-export_power_mwh"]
     )
     simulation.plot(
         ax=axes[0],
         x="Index",
         y="import-export-balance",
     )
+    axes[0].set_ylim()
     axes[0].set_title("Power Balance MWh (Import Positive)")
     axes[0].set_ylabel("MWh")
+
     #  TODO will need some work in a multi-battery world
     simulation["net-battery-charge"] = (
         simulation[find_column(simulation, "battery-", "-charge_mwh")]
         - simulation[find_column(simulation, "battery-", "-discharge_mwh")]
     )
     simulation.plot(
         ax=axes[1],
@@ -160,15 +167,15 @@
 def plot_chp(results: "epl.results.SimulationResult", path: pathlib.Path) -> None:
     """Plot CHP generator simulation results."""
     simulation = results.simulation
     fig, axes = plt.subplots(nrows=5, sharex=True, figsize=(12, 8))
     simulation["Index"] = np.arange(simulation.shape[0]).tolist()
 
     simulation["import-export-balance"] = (
-        simulation["import_power_mwh"] - simulation["export_power_mwh"]
+        simulation["site-import_power_mwh"] - simulation["site-export_power_mwh"]
     )
     simulation.plot(
         ax=axes[0],
         x="Index",
         y="import-export-balance",
     )
     axes[0].set_ylabel("MWh")
@@ -179,15 +186,15 @@
         y="boiler-high_temperature_generation_mwh",
     )
     axes[1].set_ylabel("MWh")
     axes[1].set_title("Boiler Heat Generation MWh")
     simulation.plot(
         ax=axes[2],
         x="Index",
-        y="spill-default-low_temperature_load_mwh",
+        y="spill-low_temperature_load_mwh",
     )
     axes[2].set_ylabel("MWh")
     axes[2].set_title("Low Temperature Heat Dump MWh")
     simulation.plot(
         "Index",
         "electricity_prices",
         ax=axes[3],
```

### Comparing `energypylinear-0.1.1/pyproject.toml` & `energypylinear-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 [tool.poetry]
 name = "energypylinear"
-version = "0.1.1"
+version = "0.1.2"
 description = "Optimizing energy assets with mixed-integer linear programming."
 authors = ["Adam Green <adam.green@adgefficiency.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.12"
 PuLP = "^2.7.0"
 numpy = "^1.23.4"
 pydantic = "^1.10.2"
 pandas = "^1.5.2"
 matplotlib = "^3.6.2"
 rich = "^12.0.0"
 seaborn = "^0.12.2"
-
+pandera = "^0.14.5"
+markdown-include = "^0.8.1"
 
 [tool.poetry.group.check.dependencies]
 black = "^22.10.0"
 isort = "^5.10.1"
 flake8-docstring-checker = "^1.1"
-
+ruff = "^0.0.275"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
 coverage = "^6.5.0"
 hypothesis = "^6.61.0"
 phmdoctest = "^1.4.0"
 nbmake = "^1.3.5"
 pytest-testmon = "^1.4.5"
 pytest-sugar = "^0.9.6"
 coverage-badge = "^1.1.0"
 
-
 [tool.poetry.group.develop.dependencies]
 ipython = "^8.7.0"
 
-
 [tool.poetry.group.static.dependencies]
 mypy = "^0.991"
 
+
+[tool.poetry.group.dev.dependencies]
+mike = "^1.1.2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

