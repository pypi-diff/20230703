# Comparing `tmp/easyFermi-1.1.2.tar.gz` & `tmp/easyFermi-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyFermi-1.1.2.tar", last modified: Wed Jun 14 14:31:34 2023, max compression
+gzip compressed data, was "easyFermi-1.1.3.tar", last modified: Mon Jul  3 12:51:44 2023, max compression
```

## Comparing `easyFermi-1.1.2.tar` & `easyFermi-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-06-14 14:31:34.253104 easyFermi-1.1.2/
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1522 2022-01-31 12:02:33.000000 easyFermi-1.1.2/LICENSE.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)     1702 2023-06-14 14:31:34.253104 easyFermi-1.1.2/PKG-INFO
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1172 2022-08-22 09:22:30.000000 easyFermi-1.1.2/README.md
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-06-14 14:31:34.253104 easyFermi-1.1.2/easyFermi/
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)       63 2022-02-01 13:52:31.000000 easyFermi-1.1.2/easyFermi/__init__.py
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)    92547 2023-06-14 14:28:57.000000 easyFermi-1.1.2/easyFermi/easyFermi.py
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-06-14 14:31:34.253104 easyFermi-1.1.2/easyFermi/images/
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)    40332 2022-01-15 16:04:30.000000 easyFermi-1.1.2/easyFermi/images/easyFermiIcon.png
--rw-rw-r--   0 raniere   (1000) raniere   (1000)   120905 2023-03-08 11:57:13.000000 easyFermi-1.1.2/easyFermi/images/easyFermiWindow.png
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)   121691 2021-11-23 14:18:26.000000 easyFermi-1.1.2/easyFermi/images/fermi.png
-drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-06-14 14:31:34.253104 easyFermi-1.1.2/easyFermi.egg-info/
--rw-rw-r--   0 raniere   (1000) raniere   (1000)     1702 2023-06-14 14:31:34.000000 easyFermi-1.1.2/easyFermi.egg-info/PKG-INFO
--rw-rw-r--   0 raniere   (1000) raniere   (1000)      338 2023-06-14 14:31:34.000000 easyFermi-1.1.2/easyFermi.egg-info/SOURCES.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)        1 2023-06-14 14:31:34.000000 easyFermi-1.1.2/easyFermi.egg-info/dependency_links.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)       14 2023-06-14 14:31:34.000000 easyFermi-1.1.2/easyFermi.egg-info/requires.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)       10 2023-06-14 14:31:34.000000 easyFermi-1.1.2/easyFermi.egg-info/top_level.txt
--rw-rw-r--   0 raniere   (1000) raniere   (1000)       38 2023-06-14 14:31:34.253104 easyFermi-1.1.2/setup.cfg
--rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1181 2023-06-14 14:30:04.000000 easyFermi-1.1.2/setup.py
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-07-03 12:51:44.200266 easyFermi-1.1.3/
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1522 2022-01-31 12:02:33.000000 easyFermi-1.1.3/LICENSE.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)     1702 2023-07-03 12:51:44.200266 easyFermi-1.1.3/PKG-INFO
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1172 2022-08-22 09:22:30.000000 easyFermi-1.1.3/README.md
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-07-03 12:51:44.196267 easyFermi-1.1.3/easyFermi/
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)       63 2022-02-01 13:52:31.000000 easyFermi-1.1.3/easyFermi/__init__.py
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)    93185 2023-07-03 12:42:36.000000 easyFermi-1.1.3/easyFermi/easyFermi.py
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-07-03 12:51:44.200266 easyFermi-1.1.3/easyFermi/images/
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)    40332 2022-01-15 16:04:30.000000 easyFermi-1.1.3/easyFermi/images/easyFermiIcon.png
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)   122614 2023-07-03 12:48:11.000000 easyFermi-1.1.3/easyFermi/images/easyFermiWindow.png
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)   121691 2021-11-23 14:18:26.000000 easyFermi-1.1.3/easyFermi/images/fermi.png
+drwxrwxr-x   0 raniere   (1000) raniere   (1000)        0 2023-07-03 12:51:44.196267 easyFermi-1.1.3/easyFermi.egg-info/
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)     1702 2023-07-03 12:51:44.000000 easyFermi-1.1.3/easyFermi.egg-info/PKG-INFO
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)      338 2023-07-03 12:51:44.000000 easyFermi-1.1.3/easyFermi.egg-info/SOURCES.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)        1 2023-07-03 12:51:44.000000 easyFermi-1.1.3/easyFermi.egg-info/dependency_links.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)       14 2023-07-03 12:51:44.000000 easyFermi-1.1.3/easyFermi.egg-info/requires.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)       10 2023-07-03 12:51:44.000000 easyFermi-1.1.3/easyFermi.egg-info/top_level.txt
+-rw-rw-r--   0 raniere   (1000) raniere   (1000)       38 2023-07-03 12:51:44.200266 easyFermi-1.1.3/setup.cfg
+-rwxrwxrwx   0 raniere   (1000) raniere   (1000)     1181 2023-07-03 12:50:40.000000 easyFermi-1.1.3/setup.py
```

### Comparing `easyFermi-1.1.2/LICENSE.txt` & `easyFermi-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easyFermi-1.1.2/PKG-INFO` & `easyFermi-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyFermi
-Version: 1.1.2
+Version: 1.1.3
 Summary: The easiest way to analyze Fermi-LAT data
 Author: Raniere de Menezes
 Author-email: <easyfermi@gmail.com>
 Keywords: python,fermi,GUI,graphical interface,easyFermi,gamma-rays
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyFermi-1.1.2/README.md` & `easyFermi-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `easyFermi-1.1.2/easyFermi/easyFermi.py` & `easyFermi-1.1.3/easyFermi/easyFermi.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         self.checkBox_6.setObjectName("checkBox_6")
         self.doubleSpinBox_2 = QtWidgets.QDoubleSpinBox(self.groupBox_2)
         self.doubleSpinBox_2.setGeometry(QtCore.QRect(40, 280, 69, 26))
         self.doubleSpinBox_2.setMinimum(0.5)
         self.doubleSpinBox_2.setProperty("value", 2.0)
         self.doubleSpinBox_2.setObjectName("doubleSpinBox_2")
         self.checkBox_5 = QtWidgets.QCheckBox(self.groupBox_2)
-        self.checkBox_5.setGeometry(QtCore.QRect(10, 260, 131, 23))
+        self.checkBox_5.setGeometry(QtCore.QRect(10, 260, 151, 23))
         self.checkBox_5.setChecked(True)
         self.checkBox_5.setObjectName("checkBox_5")
         self.checkBox_4 = QtWidgets.QCheckBox(self.groupBox_2)
         self.checkBox_4.setGeometry(QtCore.QRect(10, 240, 131, 23))
         self.checkBox_4.setObjectName("checkBox_4")
         self.label_11 = QtWidgets.QLabel(self.groupBox_2)
         self.label_11.setGeometry(QtCore.QRect(120, 280, 101, 21))
@@ -628,16 +628,16 @@
         self.comboBox_2.setToolTip("Select a spectral model for your target")
         self.comboBox_3.setToolTip("Select the output format for the main plots (i.e. SED, light curve etc)")
         self.checkBox_13.setToolTip("Check if you wish that only the normalizations can vary")
         self.checkBox_14.setToolTip("Freeze the Galactic diffuse model")
         self.checkBox_15.setToolTip("Freeze the isotropic diffuse model")
         self.checkBox_16.setToolTip("If checked, you will freeze the spectral shape of the target")
         self.checkBox_8.setToolTip("Check to look for extra sources in the ROI, i.e. sources not listed in the adopted catalog")
-        self.checkBox_6.setToolTip("If checked, the target will be removed from the model. If unchecked, easyFermi computes the residuals TS map")
-        self.label_11.setToolTip("The photon index of the test source")
+        self.checkBox_6.setToolTip("If checked, easyFermi will also compute the residuals TS map")
+        self.label_11.setToolTip("The photon index of the test source adopted in the TS and excess maps")
         self.spinBox_2.setToolTip("Multiprocessing is available only for Linux OS")
         self.checkBox_4.setToolTip("Check this to find the optimal R.A. and Dec. of the target's gamma-ray emission")
         self.lineEdit_12.setToolTip("Only the sources within this radius will have free parameters during the fit")
 
     def retranslateUi(self, mainWindow):
         _translate = QtCore.QCoreApplication.translate
         mainWindow.setWindowIcon(QtGui.QIcon(libpath+'easyFermiIcon.png'))
@@ -650,16 +650,16 @@
         self.checkBox_3.setText(_translate("mainWindow", "Extension:"))
         self.label_9.setText(_translate("mainWindow", "N⁰ of cores"))
         self.label_10.setText(_translate("mainWindow", "N⁰ of energy bins"))
         self.checkBox.setText(_translate("mainWindow", "Light curve:"))
         self.label_5.setText(_translate("mainWindow", "Max. size"))
         self.checkBox_2.setText(_translate("mainWindow", "SED:"))
         self.radioButton_2.setText(_translate("mainWindow", "2D-Gauss"))
-        self.checkBox_6.setText(_translate("mainWindow", "Remove target"))
-        self.checkBox_5.setText(_translate("mainWindow", "TS map:"))
+        self.checkBox_6.setText(_translate("mainWindow", "Residuals TS map"))
+        self.checkBox_5.setText(_translate("mainWindow", "TS and excess maps:"))
         self.checkBox_4.setText(_translate("mainWindow", "Relocalize"))
         self.label_11.setText(_translate("mainWindow", "Photon index"))
         self.groupBox_3.setTitle(_translate("mainWindow", "Advanced configurations:"))
         self.label_15.setText(_translate("mainWindow", "Target name/tag:"))
         self.checkBox_11.setText(_translate("mainWindow", "Delete sources:"))
         self.comboBox_2.setAccessibleName(_translate("mainWindow", "4FGL"))
         self.comboBox_2.setAccessibleDescription(_translate("mainWindow", "4FGL"))
@@ -772,15 +772,15 @@
                         
             if self.freeradiusalert != 'ok':
                 self.plainTextEdit.setPlainText(self.plainTextEdit.toPlainText()+self.freeradiusalert+"\n")
                     
             if self.checkBox_4.isChecked():
                 self.plainTextEdit.setPlainText(self.plainTextEdit.toPlainText()+"- Relocalizing target...\n")
             if self.checkBox_5.isChecked():
-                self.plainTextEdit.setPlainText(self.plainTextEdit.toPlainText()+"- Computing TS map.\n")
+                self.plainTextEdit.setPlainText(self.plainTextEdit.toPlainText()+"- Computing TS and excess maps.\n")
             if self.checkBox_2.isChecked():
                 self.plainTextEdit.setPlainText(self.plainTextEdit.toPlainText()+"- Computing SED.\n")
             if self.checkBox_3.isChecked():
                 self.plainTextEdit.setPlainText(self.plainTextEdit.toPlainText()+"- Computing extension.\n")
             if self.checkBox.isChecked():
                 self.plainTextEdit.setPlainText(self.plainTextEdit.toPlainText()+"- Computing light curve.\n")
                 
@@ -1642,14 +1642,15 @@
             self.fitquality = '- Fit quality: 1. Poor fit. Diagonal approximation only, not accurate.'
         else:
             self.fitquality = '- Fit quality: 0. Bad fit. Error matrix not calculated.'
         
         #Do plots:
         if self.checkBox_10.isChecked():
             self.gta.write_roi(self.OutputDir+'Results',make_plots=True)
+            
         else:
             self.gta.write_roi(self.OutputDir+'Results',make_plots=False)
         
         #Saving results
         f = open(self.OutputDir+'Target_results.txt','w')
         f.write(str(self.gta.roi[self.sourcename]))
         f.write('\nEnergy flux upper limit (MeV cm-2 s-1): '+str(self.gta.roi.sources[0]['eflux_ul95']))
@@ -1674,23 +1675,32 @@
             #print("New position. RA = ",self.locRA,", Dec = ",self.locDec,", r_68 = ",self.locr68,", r_95 = ",self.locr95)
             #self.plainTextEdit.setPlainText(self.plainTextEdit.toPlainText()+"Localization results saved in the file "+self.sourcename+"_loc.fits\n")
         
         #TSmap:    
         if self.checkBox_5.isChecked():
             model = {'Index' : self.doubleSpinBox_2.value(), 'SpatialModel' : 'PointSource'}
             if self.checkBox_6.isChecked():
-                TSmap = self.gta.tsmap(self.OutputDir+'Source_TS_map_', model=model, exclude=self.sourcename)
-            else:
-                TSmap = self.gta.tsmap(self.OutputDir+'Residuals_TS_map_', model=model)
+                TSmap_res = self.gta.tsmap(self.OutputDir+'Residuals_TS_map_', model=model)
+                fig = plt.figure(figsize=(8,8))
+                ROIPlotter(TSmap_res['sqrt_ts'],roi=self.gta.roi).plot(vmin=0,vmax=5,levels=[3,5,7,9],subplot=111,cmap='magma')
+                plt.gca().set_title('sqrt(TS)')
+                plt.savefig(self.OutputDir+'TSmap_residuals.'+output_format,bbox_inches='tight')
+                          
 
+            TSmap = self.gta.tsmap(self.OutputDir+'Source_TS_map_', model=model, exclude=self.sourcename)
             fig = plt.figure(figsize=(8,8))
             ROIPlotter(TSmap['sqrt_ts'],roi=self.gta.roi).plot(vmin=0,vmax=5,levels=[3,5,7,9],subplot=111,cmap='magma')
             plt.gca().set_title('sqrt(TS)')
-            plt.savefig(self.OutputDir+'TSmap.'+output_format,bbox_inches='tight')
-        
+            plt.savefig(self.OutputDir+'TSmap_target_highlighted.'+output_format,bbox_inches='tight')
+            
+            #Below we compute the excess, significance, model, and data maps:
+            resid = self.gta.residmap(self.OutputDir+'Excess_'+self.sourcename,model=model,make_plots=True, write_fits=True, write_npy=False)
+            
+            
+            
         #SED:    
         if self.checkBox_2.isChecked():
             c = np.load(self.OutputDir+'Results.npy',allow_pickle=True).flat[0]
             E = np.array(c['sources'][self.sourcename]['model_flux']['energies'])
             dnde = np.array(c['sources'][self.sourcename]['model_flux']['dnde'])
             dnde_hi = np.array(c['sources'][self.sourcename]['model_flux']['dnde_hi'])
             dnde_lo = np.array(c['sources'][self.sourcename]['model_flux']['dnde_lo'])
```

### Comparing `easyFermi-1.1.2/easyFermi/images/easyFermiIcon.png` & `easyFermi-1.1.3/easyFermi/images/easyFermiIcon.png`

 * *Files identical despite different names*

### Comparing `easyFermi-1.1.2/easyFermi/images/fermi.png` & `easyFermi-1.1.3/easyFermi/images/fermi.png`

 * *Files identical despite different names*

### Comparing `easyFermi-1.1.2/easyFermi.egg-info/PKG-INFO` & `easyFermi-1.1.3/easyFermi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyFermi
-Version: 1.1.2
+Version: 1.1.3
 Summary: The easiest way to analyze Fermi-LAT data
 Author: Raniere de Menezes
 Author-email: <easyfermi@gmail.com>
 Keywords: python,fermi,GUI,graphical interface,easyFermi,gamma-rays
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easyFermi-1.1.2/setup.py` & `easyFermi-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.2'
+VERSION = '1.1.3'
 DESCRIPTION = 'The easiest way to analyze Fermi-LAT data'
 LONG_DESCRIPTION = 'A GUI that allows to do measure the flux, create light curves, SEDs, and TS maps for Fermi-LAT data.'
 
 # Setting up
 setup(
     name="easyFermi",
     version=VERSION,
```

