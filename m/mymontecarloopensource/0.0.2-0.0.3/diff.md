# Comparing `tmp/mymontecarloopensource-0.0.2-py3-none-any.whl.zip` & `tmp/mymontecarloopensource-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5032 bytes, number of entries: 9
+Zip file size: 5911 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx     1648 b- defN 23-Jun-13 08:39 Autocallable/AutocallableSingleUnderlyingPricer.py
--rw-rw-r--  2.0 unx     2863 b- defN 23-Jun-13 08:39 Autocallable/AutocallableTwoUnderlyingsPricer.py
+-rw-rw-r--  2.0 unx     2863 b- defN 23-Jul-03 16:50 Autocallable/AutocallableTwoUnderlyingsPricer.py
 -rw-rw-r--  2.0 unx       97 b- defN 23-Jun-13 08:39 Autocallable/__init__.py
--rw-rw-r--  2.0 unx     7048 b- defN 23-Jun-13 09:00 StableGreeksInvestigationToolbox/StableGreeksInvestigationToolbox.py
+-rw-rw-r--  2.0 unx    15586 b- defN 23-Jul-03 16:50 StableGreeksInvestigationToolbox/StableGreeksInvestigationToolbox.py
 -rw-rw-r--  2.0 unx       47 b- defN 23-Jun-13 09:00 StableGreeksInvestigationToolbox/__init__.py
--rw-rw-r--  2.0 unx      135 b- defN 23-Jun-13 09:01 mymontecarloopensource-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-13 09:01 mymontecarloopensource-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       46 b- defN 23-Jun-13 09:01 mymontecarloopensource-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      872 b- defN 23-Jun-13 09:01 mymontecarloopensource-0.0.2.dist-info/RECORD
-9 files, 12848 bytes uncompressed, 3482 bytes compressed:  72.9%
+-rw-rw-r--  2.0 unx      135 b- defN 23-Jul-03 16:53 mymontecarloopensource-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-03 16:53 mymontecarloopensource-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       46 b- defN 23-Jul-03 16:53 mymontecarloopensource-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      873 b- defN 23-Jul-03 16:53 mymontecarloopensource-0.0.3.dist-info/RECORD
+9 files, 21387 bytes uncompressed, 4361 bytes compressed:  79.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: StableGreeksInvestigationToolbox/StableGreeksInvestigationToolbox.py
 Comment: 
 
 Filename: StableGreeksInvestigationToolbox/__init__.py
 Comment: 
 
-Filename: mymontecarloopensource-0.0.2.dist-info/METADATA
+Filename: mymontecarloopensource-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: mymontecarloopensource-0.0.2.dist-info/WHEEL
+Filename: mymontecarloopensource-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: mymontecarloopensource-0.0.2.dist-info/top_level.txt
+Filename: mymontecarloopensource-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: mymontecarloopensource-0.0.2.dist-info/RECORD
+Filename: mymontecarloopensource-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## StableGreeksInvestigationToolbox/StableGreeksInvestigationToolbox.py

```diff
@@ -3,99 +3,199 @@
 from enum import Enum
 
 
         
 class StableGreeksInvestigationToolbox:
     @staticmethod
     def runInvestigation(fixed_func, x, investigationSettings):
-        if investigationSettings.DetectInstabilities:
-            StableGreeksInvestigationToolbox.instabilityDetectionDelta(fixed_func, x, investigationSettings)
-            StableGreeksInvestigationToolbox.instabilityDetectionGamma(fixed_func, x, investigationSettings)
-            
-        PlotSurfaceTool.runInvestigation(fixed_func, x, investigationSettings)
+        if x.ndim == 1: 
+            if investigationSettings.DetectInstabilities:
+                StableGreeksInvestigationToolbox.instabilityDetectionDelta(fixed_func, x, investigationSettings)
+                StableGreeksInvestigationToolbox.instabilityDetectionGamma(fixed_func, x, investigationSettings)
+                
+            PlotSurfaceTool.runInvestigation(fixed_func, x, investigationSettings)
+        elif x.ndim == 2:
+            PlotSurfaceTool.runInvestigation(fixed_func, x, investigationSettings)
+        else:
+            # Handle the error or default case
+            raise ValueError("Invalid input shape. Expected 1 or 2 dimensions.")
+
         
     @staticmethod
     def instabilityDetectionDelta(fixed_func, x, investigationSettings):
-        
         print("Instability detection for Delta started:")
-        
         delta1 = FunctionEvaluation.compute_delta(fixed_func, x, investigationSettings,0.1)
         delta2 = FunctionEvaluation.compute_delta(fixed_func, x, investigationSettings,0.001)
         delta3 = FunctionEvaluation.compute_delta(fixed_func, x, investigationSettings,0.00001)
-        
         instabilityDetected = False
-        
         for i in range(0, len(x)):
             if (delta1[i] != 0 and delta2[i] != 0 and delta3[i] != 0):
                 ratio1 = np.abs(np.divide(delta2[i] , delta1[i]))
                 ratio2 = np.abs(np.divide(delta3[i] , delta2[i]))
                                 
                 if (ratio1 > ratio2 * 2 ):
                     print("Delta jump detected for x = " + str(x[i]))
                     instabilityDetected = True
                     print("Stopping investigation for Delta (stopping on first hit)")
                     break
         if (not instabilityDetected):        
             print("Instability detection for Delta done: No instabilities detected")
                 
-                
     @staticmethod
     def instabilityDetectionGamma(fixed_func, x, investigationSettings):
-        
         print("Instability detection for Gamma started:")
-        
         gamma1 = FunctionEvaluation.compute_gamma(fixed_func, x, investigationSettings,0.1)
         gamma2 = FunctionEvaluation.compute_gamma(fixed_func, x, investigationSettings,0.01)
         gamma3 = FunctionEvaluation.compute_gamma(fixed_func, x, investigationSettings,0.001)
-        
         instabilityDetected = False
-        
         for i in range(0, len(x)):
             if (gamma1[i] != 0 and gamma2[i] != 0 and gamma3[i] != 0):
                 ratio1 = np.abs(np.divide(gamma2[i] , gamma1[i]))
                 ratio2 = np.abs(np.divide(gamma3[i] , gamma2[i]))
                 if (ratio1 > ratio2 * 2 ):
                     print("Gamma jump detected for x = " + str(x[i]))
                     instabilityDetected = True
                     print("Stopping investigation for Gamma (stopping on first hit)")
                     break
         if (not instabilityDetected): 
             print("Instability detection for Gamma done: No instabilities detected")
         
         
+        
+        
 class FunctionEvaluation:
     
     @staticmethod
     def evaluate_function(fixed_func, x):
-        y = np.zeros(len(x))  # Create an array to store the y-values
-        for i in range(0, len(x)):
-            y[i] = fixed_func(x[i])
-        return y
-    
+        if x.ndim == 1:
+            y = np.zeros(len(x))  # Create an array to store the y-values
+            for i in range(0, len(x)):
+                y[i] = fixed_func(x[i])
+            return y
+        elif x.ndim == 2:
+            s_0, s_1 = x
+            # Generate meshgrid from s_0 and s_1
+            S0, S1 = np.meshgrid(s_0, s_1)
+
+            # Evaluate fixed_func for each combination of S0 and S1
+            y = np.zeros_like(S0)
+            for i in range(S0.shape[0]):
+                for j in range(S0.shape[1]):
+                    y[i, j] = fixed_func(S0[i, j], S1[i, j])
+            return y
+        else:
+            # Handle the error or default case
+            raise ValueError("Invalid input shape. Expected 1 or 2 dimensions.")
+
+        
     @staticmethod
     def compute_delta(fixed_func, x, hFinDiff, hardCodedh = None):
         if hardCodedh is None:
             h = hFinDiff
         else:
             h = hardCodedh   
-        delta = np.zeros(len(x))
-        for i in range(0, len(x)):
-            delta[i] = np.divide(fixed_func(x[i] + h) - fixed_func(x[i]), h)
+        if x.ndim == 1:
+            delta = np.zeros(len(x))
+            for i in range(len(x)):
+                delta[i] = np.divide(fixed_func(x[i] + h) - fixed_func(x[i]), h)
+            return delta
+        elif x.ndim == 2:
+            s_0, s_1 = x
+            # Generate meshgrid from s_0 and s_1
+            S0, S1 = np.meshgrid(s_0, s_1)
+
+            # Evaluate fixed_func for each combination of S0 and S1
+            delta1 = np.zeros([S0.shape[0],S0.shape[1]])
+            for i in range(S0.shape[0]):
+                for j in range(S0.shape[1]):
+                    a = np.divide(fixed_func(S0[i, j] + h, S1[i, j]) - fixed_func(S0[i, j], S1[i, j]),h)
+                    delta1[i, j] = a
+            delta = delta1
+            return delta
+        else:
+            raise ValueError("Invalid input shape. Expected 1 or 2 dimensions.")
+        
+    # Additional method for computing delta w.r.t. s2 (second dimension)    
+    @staticmethod
+    def compute_delta_s2(fixed_func, x, hFinDiff, hardCodedh = None):
+        if hardCodedh is None:
+            h = hFinDiff
+        else:
+            h = hardCodedh   
+        s_0, s_1 = x
+        # Generate meshgrid from s_0 and s_1
+        S0, S1 = np.meshgrid(s_0, s_1)
+
+        # Evaluate fixed_func for each combination of S0 and S1
+        delta1 = np.zeros([S0.shape[0],S0.shape[1]])
+        for i in range(S0.shape[0]):
+            for j in range(S0.shape[1]):
+                a = np.divide(fixed_func(S0[i, j], S1[i, j]+h) - fixed_func(S0[i, j], S1[i, j]),h)
+                delta1[i, j] = a
+        delta = delta1
         return delta
     
     @staticmethod
     def compute_gamma(fixed_func, x, hFinDiff, hardCodedh = None):
         if hardCodedh is None:
             h = hFinDiff
         else:
             h = hardCodedh   
-        gamma = np.zeros(len(x))
-        for i in range(0, len(x)):
-            gamma[i] = np.divide(fixed_func(x[i] + h)  - 2*  fixed_func(x[i])  + fixed_func(x[i] - h) , h * h)
-        return gamma
+        if x.ndim == 1:
+            gamma = np.zeros(len(x))
+            for i in range(len(x)):
+                gamma[i] = np.divide(fixed_func(x[i] + h) - 2 * fixed_func(x[i]) + fixed_func(x[i] - h), h * h)
+            return gamma
+        elif x.ndim == 2:
+            s_0, s_1 = x
+            # Generate meshgrid from s_0 and s_1
+            S0, S1 = np.meshgrid(s_0, s_1)
+
+            # Evaluate fixed_func for each combination of S0 and S1
+            gamma_s1 = np.zeros([S0.shape[0],S0.shape[1]])
+            for i in range(S0.shape[0]):
+                for j in range(S0.shape[1]):
+                    gamma_s1[i, j] = np.divide(fixed_func(S0[i, j]+h, S1[i, j])-2*fixed_func(S0[i, j], S1[i, j])+fixed_func(S0[i, j]-h, S1[i, j]),h*h)
+            return gamma_s1
+        else:
+            raise ValueError("Invalid input shape. Expected 1 or 2 dimensions.")
+    
+    @staticmethod
+    def compute_gamma_s2(fixed_func, x, hFinDiff, hardCodedh = None):
+        if hardCodedh is None:
+            h = hFinDiff
+        else:
+            h = hardCodedh   
+        s_0, s_1 = x
+        # Generate meshgrid from s_0 and s_1
+        S0, S1 = np.meshgrid(s_0, s_1)
+
+        # Evaluate fixed_func for each combination of S0 and S1
+        gamma_s2 = np.zeros([S0.shape[0],S0.shape[1]])
+        for i in range(S0.shape[0]):
+            for j in range(S0.shape[1]):
+                gamma_s2[i, j] = np.divide(fixed_func(S0[i, j], S1[i, j]+h)-2*fixed_func(S0[i, j], S1[i, j])+fixed_func(S0[i, j], S1[i, j]-h),h*h)
+        return gamma_s2
+
+    @staticmethod
+    def compute_gamma_mixed(fixed_func, x, hFinDiff, hardCodedh = None):
+        if hardCodedh is None:
+            h = hFinDiff
+        else:
+            h = hardCodedh   
+        s_0, s_1 = x
+        # Generate meshgrid from s_0 and s_1
+        S0, S1 = np.meshgrid(s_0, s_1)
+
+        # Evaluate fixed_func for each combination of S0 and S1
+        gamma_mixed = np.zeros([S0.shape[0],S0.shape[1]])
+        for i in range(S0.shape[0]):
+            for j in range(S0.shape[1]):
+                gamma_mixed[i, j] = np.divide(fixed_func(S0[i, j]+h, S1[i, j]+h)-fixed_func(S0[i, j]+h, S1[i, j])-fixed_func(S0[i, j], S1[i, j]+h)+2*fixed_func(S0[i, j], S1[i, j])-fixed_func(S0[i, j]-h, S1[i, j])-fixed_func(S0[i, j], S1[i, j]-h)+fixed_func(S0[i, j]-h, S1[i, j]-h),h*h)
+        return gamma_mixed
         
     
 class InvestigationSettings:
     def __init__(self):
         self._plot_setting = None
         self._h_finite_differences = None
         self._detect_instabilities = False
@@ -116,78 +216,142 @@
         
     @property
     def DetectInstabilities(self):
         return self._detect_instabilities
 
     def set_DetectInstabilities(self, value):
         self._detect_instabilities = bool(value)
-        
 
 
 class PlotSettings(Enum):
     PresentValue = 1
     Delta = 2
     Gamma = 3
+    DeltaExtended = 4
+    GammaExtended = 5
     
 class PlotSurfaceTool:
     @staticmethod
     def runInvestigation(fixed_func, x, investigationSettings):
         if investigationSettings.PlotSetting == PlotSettings.PresentValue:
             print(investigationSettings.PlotSetting)
-            y = FunctionEvaluation.evaluate_function(fixed_func, x)
-            PlotSurfaceTool.plot_valuation_1d(x, y, 'Present value')
+            pv = FunctionEvaluation.evaluate_function(fixed_func, x)
+            if x.ndim == 1:
+                PlotSurfaceTool.plot_valuation_1d(x, pv, 'Present value')
+            elif x.ndim == 2:
+                #Meshgrid
+                x, y = x
+                X, Y = np.meshgrid(x, y)
+                fig, axs = plt.subplots(1, 1, figsize=(15, 4))
+                axs.axis('off')
+                # Plots
+                PlotSurfaceTool.plot_valuation_2d(X, Y, pv, 'Present Value', fig, 111)
         elif investigationSettings.PlotSetting== PlotSettings.Delta:
-            y = FunctionEvaluation.evaluate_function(fixed_func, x)
+            pv = FunctionEvaluation.evaluate_function(fixed_func, x)
             delta = FunctionEvaluation.compute_delta(fixed_func, x, investigationSettings.FiniteDifferencesStepWidth)
-
-            fig, axs = plt.subplots(1, 2, figsize=(10, 3))
-
-            axs[0].plot(x, y)
-            axs[0].set_xlabel('x')
-            axs[0].set_ylabel('Value')
-            axs[0].set_title('Present value')
-
-            axs[1].plot(x, delta)
-            axs[1].set_xlabel('x')
-            axs[1].set_ylabel('Delta')
-            axs[1].set_title('Delta')
-
-            plt.tight_layout()
+            if x.ndim == 1:
+                fig, axs = plt.subplots(1, 2, figsize=(12, 4))
+                PlotSurfaceTool.plot_valuation_1d(x, pv, 'Present value', fig, 121)
+                PlotSurfaceTool.plot_valuation_1d(x, delta, 'Delta', fig, 122)
+                plt.show()
+            elif x.ndim == 2:
+                #Meshgrid
+                x, y = x
+                X, Y = np.meshgrid(x, y)
+                fig, axs = plt.subplots(1, 2, figsize=(15, 4))
+                for ax in axs:
+                    ax.axis('off')
+                # Plots
+                PlotSurfaceTool.plot_valuation_2d(X, Y, pv, 'Present Value', fig, 121)
+                PlotSurfaceTool.plot_valuation_2d(X, Y, delta, 'Delta', fig, 122)
+                plt.show()
+        elif investigationSettings.PlotSetting== PlotSettings.DeltaExtended:
+            if x.ndim == 1:
+                raise ValueError("Extended only for 2 dimensional functions")
+            pv = FunctionEvaluation.evaluate_function(fixed_func, x)
+            delta = FunctionEvaluation.compute_delta(fixed_func, x, investigationSettings.FiniteDifferencesStepWidth)
+            delta_s2 = FunctionEvaluation.compute_delta_s2(fixed_func, x, investigationSettings.FiniteDifferencesStepWidth)
+            #Meshgrid
+            x, y = x
+            X, Y = np.meshgrid(x, y)
+            fig, axs = plt.subplots(1, 3, figsize=(15, 4))
+            for ax in axs:
+                ax.axis('off')
+            # Plots
+            PlotSurfaceTool.plot_valuation_2d(X, Y, pv, 'Present Value', fig, 131)
+            PlotSurfaceTool.plot_valuation_2d(X, Y, delta, 'Delta S1', fig, 132)
+            PlotSurfaceTool.plot_valuation_2d(X, Y, delta_s2, 'Delta S2', fig, 133)
             plt.show()
+            
         elif investigationSettings.PlotSetting == PlotSettings.Gamma:
-            y = FunctionEvaluation.evaluate_function(fixed_func, x)
+            pv = FunctionEvaluation.evaluate_function(fixed_func, x)
             delta = FunctionEvaluation.compute_delta(fixed_func, x, investigationSettings.FiniteDifferencesStepWidth)
             gamma = FunctionEvaluation.compute_gamma(fixed_func, x, investigationSettings.FiniteDifferencesStepWidth)
+            if x.ndim == 1:
+                fig, axs = plt.subplots(1, 2, figsize=(12, 4))
+                PlotSurfaceTool.plot_valuation_1d(x, pv, 'Present value', fig, 131)
+                PlotSurfaceTool.plot_valuation_1d(x, delta, 'Delta', fig, 132)
+                PlotSurfaceTool.plot_valuation_1d(x, gamma, 'Gamma', fig, 133)
+                plt.show()
+            elif x.ndim == 2:
+                #Meshgrid
+                x, y = x
+                X, Y = np.meshgrid(x, y)
+                fig, axs = plt.subplots(1, 3, figsize=(15, 4))
+                for ax in axs:
+                    ax.axis('off')
+                # Plots
+                PlotSurfaceTool.plot_valuation_2d(X, Y, pv, 'Present Value', fig, 131)
+                PlotSurfaceTool.plot_valuation_2d(X, Y, delta, 'Delta', fig, 132)
+                PlotSurfaceTool.plot_valuation_2d(X, Y, gamma, 'Gamma', fig, 133)
+                plt.show()
+        elif investigationSettings.PlotSetting == PlotSettings.GammaExtended:
+            if x.ndim == 1:
+                raise ValueError("Extended only for 2 dimensional functions")
+            pv = FunctionEvaluation.evaluate_function(fixed_func, x)
+            delta = FunctionEvaluation.compute_delta(fixed_func, x, investigationSettings.FiniteDifferencesStepWidth)
+            delta_s2 = FunctionEvaluation.compute_delta_s2(fixed_func, x, investigationSettings.FiniteDifferencesStepWidth)
+            gamma = FunctionEvaluation.compute_gamma(fixed_func, x, investigationSettings.FiniteDifferencesStepWidth)
+            gamma_s2 = FunctionEvaluation.compute_gamma_s2(fixed_func, x, investigationSettings.FiniteDifferencesStepWidth)
+            gamma_mixed = FunctionEvaluation.compute_gamma_mixed(fixed_func, x, investigationSettings.FiniteDifferencesStepWidth)
 
-            fig, axs = plt.subplots(1, 3, figsize=(10, 3))
-
-            axs[0].plot(x, y)
-            axs[0].set_xlabel('x')
-            axs[0].set_ylabel('Value')
-            axs[0].set_title('Present value')
-
-            axs[1].plot(x, delta)
-            axs[1].set_xlabel('x')
-            axs[1].set_ylabel('Delta')
-            axs[1].set_title('Delta')
-
-            axs[2].plot(x, gamma)
-            axs[2].set_xlabel('x')
-            axs[2].set_ylabel('Gamma')
-            axs[2].set_title('Gamma')
-
-            plt.tight_layout()
+            #Meshgrid
+            x, y = x
+            X, Y = np.meshgrid(x, y)
+            fig, axs = plt.subplots(1, 6, figsize=(15, 4))
+            for ax in axs:
+                ax.axis('off')
+            # Plots
+            PlotSurfaceTool.plot_valuation_2d(X, Y, pv, 'Present Value', fig, 161)
+            PlotSurfaceTool.plot_valuation_2d(X, Y, delta, 'Delta S1', fig, 162)
+            PlotSurfaceTool.plot_valuation_2d(X, Y, delta_s2, 'Delta S2', fig, 163)
+            PlotSurfaceTool.plot_valuation_2d(X, Y, gamma, 'Gamma S1', fig, 164)
+            PlotSurfaceTool.plot_valuation_2d(X, Y, gamma_s2, 'Gamma S2', fig, 165)
+            PlotSurfaceTool.plot_valuation_2d(X, Y, gamma_mixed, 'Gamma mixed', fig, 166)
+            plt.subplots_adjust(wspace=0.4)
             plt.show()
+            
     
     @staticmethod
-    def plot_valuation_1d(x, y, title):
-        plt.plot(x, y)
-        plt.xlabel('x')
-        plt.ylabel('y')
-        plt.title(title)
-        plt.show()
+    def plot_valuation_1d(x, y, title, fig, subplotIndex):
+        ax = fig.add_subplot(subplotIndex)
+        ax.plot(x, y)
+        ax.set_xlabel('S')
+        ax.set_ylabel('Value')
+        ax.set_title(title)
         
     @staticmethod
+    def plot_valuation_2d(x, y, z, title, fig, subplotIndex):
+        ax = fig.add_subplot(subplotIndex, projection='3d')
+        ax.plot_surface(x, y, z, cmap='viridis')
+        ax.set_title(title)
+        ax.set_xlabel('S0')
+        ax.set_ylabel('S1')
+        ax.set_zlabel('Value')
+    
+    @staticmethod
     def do_something(a, b, c):
         # Perform some computations
         result = a + b * c
-        return result
+        return result
+        
+
```

