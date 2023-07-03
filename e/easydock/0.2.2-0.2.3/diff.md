# Comparing `tmp/easydock-0.2.2.tar.gz` & `tmp/easydock-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easydock-0.2.2.tar", last modified: Wed Jun 28 10:20:05 2023, max compression
+gzip compressed data, was "dist/easydock-0.2.3.tar", last modified: Mon Jul  3 14:31:45 2023, max compression
```

## Comparing `easydock-0.2.2.tar` & `easydock-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-28 10:20:05.000000 easydock-0.2.2/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1516 2019-11-25 13:17:56.000000 easydock-0.2.2/LICENSE.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     9135 2023-06-28 10:20:05.000000 easydock-0.2.2/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       79 2023-06-28 10:20:05.000000 easydock-0.2.2/setup.cfg
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-28 10:20:05.000000 easydock-0.2.2/easydock/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    22000 2023-06-28 09:30:15.000000 easydock-0.2.2/easydock/preparation_for_docking.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    13918 2023-06-28 10:08:30.000000 easydock-0.2.2/easydock/run_dock.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3382 2023-05-16 09:01:52.000000 easydock-0.2.2/easydock/vina_dock_cli.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7491 2023-05-16 09:01:52.000000 easydock-0.2.2/easydock/read_input.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       22 2023-06-28 10:18:21.000000 easydock-0.2.2/easydock/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5965 2023-05-30 12:11:29.000000 easydock-0.2.2/easydock/get_sdf_from_dock_db.py
--rwxrwxr-x   0 pavel     (1000) pavel     (1000)     5288 2023-05-16 09:01:52.000000 easydock-0.2.2/easydock/vina_dock.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2713 2023-05-16 09:01:52.000000 easydock-0.2.2/easydock/gnina_dock.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7048 2023-06-28 10:18:21.000000 easydock-0.2.2/README.md
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-06-28 10:20:05.000000 easydock-0.2.2/easydock.egg-info/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     9135 2023-06-28 10:20:04.000000 easydock-0.2.2/easydock.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      439 2023-06-28 10:20:05.000000 easydock-0.2.2/easydock.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      111 2023-06-28 10:20:04.000000 easydock-0.2.2/easydock.egg-info/entry_points.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        9 2023-06-28 10:20:04.000000 easydock-0.2.2/easydock.egg-info/top_level.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       24 2023-06-28 10:20:04.000000 easydock-0.2.2/easydock.egg-info/requires.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-06-28 10:20:04.000000 easydock-0.2.2/easydock.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1155 2023-05-16 09:01:52.000000 easydock-0.2.2/setup.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-07-03 14:31:45.000000 easydock-0.2.3/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1516 2019-11-25 13:17:56.000000 easydock-0.2.3/LICENSE.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10179 2023-07-03 14:31:45.000000 easydock-0.2.3/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       79 2023-07-03 14:31:45.000000 easydock-0.2.3/setup.cfg
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-07-03 14:31:45.000000 easydock-0.2.3/easydock/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7814 2023-06-30 15:44:58.000000 easydock-0.2.3/easydock/preparation_for_docking.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    13959 2023-06-30 15:44:57.000000 easydock-0.2.3/easydock/run_dock.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    17149 2023-07-03 06:43:04.000000 easydock-0.2.3/easydock/database.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3382 2023-05-16 09:01:52.000000 easydock-0.2.3/easydock/vina_dock_cli.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7491 2023-05-16 09:01:52.000000 easydock-0.2.3/easydock/read_input.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       22 2023-07-03 14:22:44.000000 easydock-0.2.3/easydock/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5965 2023-05-30 12:11:29.000000 easydock-0.2.3/easydock/get_sdf_from_dock_db.py
+-rwxrwxr-x   0 pavel     (1000) pavel     (1000)     5288 2023-05-16 09:01:52.000000 easydock-0.2.3/easydock/vina_dock.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2713 2023-05-16 09:01:52.000000 easydock-0.2.3/easydock/gnina_dock.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       91 2023-06-30 16:25:46.000000 easydock-0.2.3/easydock/auxiliary.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7988 2023-07-03 14:29:59.000000 easydock-0.2.3/README.md
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-07-03 14:31:45.000000 easydock-0.2.3/easydock.egg-info/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10179 2023-07-03 14:31:45.000000 easydock-0.2.3/easydock.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      482 2023-07-03 14:31:45.000000 easydock-0.2.3/easydock.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      111 2023-07-03 14:31:45.000000 easydock-0.2.3/easydock.egg-info/entry_points.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        9 2023-07-03 14:31:45.000000 easydock-0.2.3/easydock.egg-info/top_level.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       24 2023-07-03 14:31:45.000000 easydock-0.2.3/easydock.egg-info/requires.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-07-03 14:31:45.000000 easydock-0.2.3/easydock.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1155 2023-05-16 09:01:52.000000 easydock-0.2.3/setup.py
```

### Comparing `easydock-0.2.2/LICENSE.txt` & `easydock-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easydock-0.2.2/PKG-INFO` & `easydock-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easydock
-Version: 0.2.2
+Version: 0.2.3
 Summary: EasyDock Python module to facilitate molecular docking
 Home-page: https://github.com/ci-lab-cz/easydock
 Author: Pavel Polishchuk, Guzel Minibaeva, Aleksandra Ivanova
 Author-email: pavel_polishchuk@ukr.net
 License: UNKNOWN
 Description: # EasyDock - Python module to automate molecular docking
         
@@ -54,32 +54,34 @@
         - docking with `vina`/`gnina`
         - output poses are converted in MOL format and stored into output DB along with docking scores
         
         ### Example
         
         ##### Docking from command line
         
-        Docking using `vina` takes input SMILES and a config file. Ligands will not be protonated with Chemaxon, so their supplied charged states will be used. 4 CPU cores will be used. When docking will finish an SDF file will be created with top docking poses for each ligand. 
+        Docking using `vina` takes input SMILES and a config file. Ligands will not be protonated with Chemaxon, so their supplied charged states will be used. 4 CPU cores will be used (4 molecules will be dock in parallel). When docking will finish an SDF file will be created with top docking poses for each ligand. 
         ```
-        run_dock -i input.smi -o output.db --program vina -c config.yml --no_protonation -c 4 --sdf
+        run_dock -i input.smi -o output.db --program vina --config config.yml --no_protonation -c 4 --sdf
         ``` 
         
         Example of config.yml for `vina` docking  
         ```
         protein: /path/to/protein.pdbqt
         protein_setup: /path/to/grid.txt
         exhaustiveness: 8
         seed: 0
         n_poses: 5
         ncpu: 5
         ```
         
+        NOTE: ncpu argument in `run_dock` and `config.yml` has different meaning. In `run_dock` it means the number of molecules docked in parallel. In `config.yml` it means the number of CPUs used for docking of a single molecule. The product of these two values should be equal or a little bit more than the number of CPUs on a computer.
+        
         The same but using `gnina`
         ```
-        run_dock -i input.smi -o output.db --program gnina -c config.yml --no_protonation -c 4 --sdf
+        run_dock -i input.smi -o output.db --program gnina --config config.yml --no_protonation -c 4 --sdf
         ``` 
         
         Example of config.yml for `gnina` docking  
         ```
         script_file: /path/to/gnina_executable
         protein: /path/to/protein.pdbqt
         protein_setup: /path/to/grid.txt
@@ -114,14 +116,18 @@
         
         ```bash
         dask ssh --hostfile $PBS_NODEFILE --nworkers 15 --nthreads 1 &
         sleep 10
         run_dock -i input.smi -o output.db --program vina -c config.yml --no_protonation -c 4 --sdf --hostfile $PBS_NODEFILE --dask_report
         ```
         `$PBS_NODEFILE` is a file containing list of IP addresses of servers. The first one from the list will be used by a dask scheduler, but it will also participate in computations.
+        
+        `--nworkers` is the number of workers per host. This is the number of molecules which are docked in parallel on a single host.
+        
+        `--nthreads` can be any value. The number of CPUs used for docking of a single molecule will be taken from `config.yml`.
           
         `--dask_report` argument will create at the end of calculations an html-file with performance report (may be useful to tweak docking parameters).
           
         **Important setup issue** - the limit of open files on every server should be increased to the level at least twice the total number of requested workers (file streams are used for inter-node communication by dask).
         
         ##### Data retrieval from the output database
         
@@ -164,14 +170,21 @@
         
         ##### Customization
         
         To implement support of a custom docking program one should implement a function like `mol_dock` which will take as input an RDKit mol object (named molecule) and an yml-file with all docking parameters. The function should run a command line script/utility and return back a tuple of a molecule name and a dictionary of parameters and their values which should be stored in DB (parameter names should be exactly the same as corresponding field names in DB). For examples, please look at `mol_dock` functions in `vina_dock` or `gnina_dock`.
         
         ### Changelog
         
+        **0.2.3**
+        - improve descriptions of examples on README
+        - catch all exceptions in conversion of PDBQT to Mol
+        - move DB related functions to a new database.py module
+        - use SMILES temporary file to protonate molecules with cxcalc
+        - add functions to get molecules from DB in Python (get_mols, select_from_db)
+        
         **0.2.2**
         - fix bug with continuation of calculations after db was transferred to other machine
         - restrict precedence of command line arguments over arguments restored from DB only to specific ones (output, hostfile, dask_report, ncpu, verbose)
         
         **0.2.1**
         - fix treatment of molecule ids in get_sdf_from_dock_db
         - change installation instructions, vina must be installed from sources
```

### Comparing `easydock-0.2.2/easydock/preparation_for_docking.py` & `easydock-0.2.3/easydock/database.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,307 +1,21 @@
 import os
-import re
 import sqlite3
 import subprocess
 import sys
 import tempfile
-import traceback
-import yaml
-from multiprocessing import cpu_count
 from copy import deepcopy
+from functools import partial
 
-from meeko import MoleculePreparation
+import yaml
+from easydock import read_input
+from easydock.preparation_for_docking import mol_is_3d
+from easydock.auxiliary import take
 from rdkit import Chem
 from rdkit.Chem import AllChem
-from easydock import read_input
-
-
-def cpu_type(x):
-    return max(1, min(int(x), cpu_count()))
-
-
-def filepath_type(x):
-    if x:
-        return os.path.abspath(x)
-    else:
-        return x
-
-
-def mol_is_3d(mol):
-    if mol.GetConformers() and list(mol.GetConformers())[0].Is3D():
-        return True
-    return False
-
-
-def mol_from_smi_or_molblock(ligand_string):
-    mol = Chem.MolFromMolBlock(ligand_string)
-    if mol is None:
-        mol = Chem.MolFromSmiles(ligand_string)
-    return mol
-
-
-def add_protonation(db_fname, tautomerize=True, table_name='mols', add_sql=''):
-    '''
-    Protonate SMILES by Chemaxon cxcalc utility to get molecule ionization states at pH 7.4.
-    Parse console output and update db.
-    :param db_fname:
-    :param tautomerize: get a major tautomer at protonation
-    :param table_name: table name with molecules to protonate
-    :param add_sql: additional SQL query to be appended to the SQL query to retrieve molecules for protonation,
-                    e.g. "AND id IN ('MOL1', 'MOL2')" or "AND iteration=(SELECT MAX(iteration) FROM mols)".
-    :return:
-    '''
-    conn = sqlite3.connect(db_fname)
-
-    try:
-        cur = conn.cursor()
-
-        sql = f"""SELECT smi, source_mol_block, id 
-                  FROM {table_name} 
-                  WHERE docking_score is NULL AND smi_protonated is NULL """
-        sql += add_sql
-
-        data_list = list(cur.execute(sql))
-        if not data_list:
-            sys.stderr.write(f'no molecules to protonate\n')
-            return
-
-        smi_ids = []
-        mol_ids = []
-        for i, (smi, mol_block, mol_name) in enumerate(data_list):
-            if mol_block is None:
-                smi_ids.append(mol_name)
-                # add missing mol blocks
-                m = Chem.MolFromSmiles(data_list[i][0])
-                m.SetProp('_Name', mol_name)
-                m_block = Chem.MolToMolBlock(m)
-                data_list[i] = (smi, m_block, mol_name)
-            else:
-                mol_ids.append(mol_name)
-        smi_ids = set(smi_ids)
-        mol_ids = set(mol_ids)
-
-        output_data_smi = []
-        output_data_mol = []
-        with tempfile.NamedTemporaryFile(suffix='.sdf', mode='w', encoding='utf-8') as tmp:
-            fd, output = tempfile.mkstemp()  # use output file to avoid overflow of stdout in extreme cases
-            try:
-                for _, mol_block, _ in data_list:
-                    tmp.write(mol_block)
-                    tmp.write('\n$$$$\n')
-                tmp.flush()
-                cmd_run = f"cxcalc -S --ignore-error majormicrospecies -H 7.4 " \
-                          f"{'-M' if tautomerize else ''} -K '{tmp.name}' > '{output}'"
-                subprocess.call(cmd_run, shell=True)
-                sdf_protonated = Chem.SDMolSupplier(output)
-                for mol in sdf_protonated:
-                    mol_name = mol.GetProp('_Name')
-                    smi = mol.GetPropsAsDict().get('MAJORMS', None)
-                    if smi is not None:
-                        try:
-                            cansmi = Chem.CanonSmiles(smi)
-                        except:
-                            sys.stderr.write(f'EASYDOCK ERROR: {mol_name}, smiles {smi} obtained after protonation '
-                                             f'could not be read by RDKit. The molecule was skipped.\n')
-                            continue
-                        if mol_name in smi_ids:
-                            output_data_smi.append((cansmi, mol_name))
-                        elif mol_name in mol_ids:
-                            try:
-                                # mol block in chemaxon sdf is an input molecule
-                                # so, we make all bonds single, remove Hs and assign bond orders from SMILES
-                                # this should work even if a generated tautomer differs from the input molecule
-                                mol = Chem.RemoveHs(Chem.RWMol(mol))
-                                for b in mol.GetBonds():
-                                    b.SetBondType(Chem.BondType.SINGLE)
-                                ref_mol = Chem.RemoveHs(Chem.MolFromSmiles(smi))
-                                mol = AllChem.AssignBondOrdersFromTemplate(ref_mol, mol)
-                                output_data_mol.append((cansmi, Chem.MolToMolBlock(mol), mol_name))
-                            except ValueError:
-                                continue
-            finally:
-                os.remove(output)
-
-        cur.executemany(f"""UPDATE {table_name}
-                       SET 
-                           smi_protonated = ?
-                       WHERE
-                           id = ?
-                    """, output_data_smi)
-        cur.executemany(f"""UPDATE {table_name}
-                       SET 
-                           smi_protonated = ?, 
-                           source_mol_block_protonated = ?
-                       WHERE
-                           id = ?
-                    """, output_data_mol)
-        conn.commit()
-
-    finally:
-        conn.close()
-
-
-def mk_prepare_ligand(mol, verbose=False):
-    preparator = MoleculePreparation(keep_nonpolar_hydrogens=False, hydrate=False, flexible_amides=False,
-                                     rigid_macrocycles=True, min_ring_size=7, max_ring_size=33)
-    try:
-        preparator.prepare(mol)
-        pdbqt_string = preparator.write_pdbqt_string()
-        if verbose:
-            preparator.show_setup()
-    except Exception:
-        sys.stderr.write('Warning. Incorrect mol object to convert to pdbqt. Continue. \n')
-        traceback.print_exc()
-        pdbqt_string = None
-
-    return pdbqt_string
-
-
-def mol_embedding_3d(mol, seed=43):
-
-    def gen_conf(mole, useRandomCoords, randomSeed):
-        params = AllChem.ETKDGv3()
-        params.useRandomCoords = useRandomCoords
-        params.randomSeed = randomSeed
-        conf_stat = AllChem.EmbedMolecule(mole, params)
-        return mole, conf_stat
-
-    if not isinstance(mol, Chem.Mol):
-        return None
-    mol = Chem.AddHs(mol, addCoords=True)
-    if not mol_is_3d(mol):  # only for non 3D input structures
-        mol, conf_stat = gen_conf(mol, useRandomCoords=False, randomSeed=seed)
-        if conf_stat == -1:
-            # if molecule is big enough and rdkit cannot generate a conformation - use params.useRandomCoords = True
-            mol, conf_stat = gen_conf(mol, useRandomCoords=True, randomSeed=seed)
-            if conf_stat == -1:
-                return None
-        AllChem.UFFOptimizeMolecule(mol, maxIters=100)
-    return mol
-
-
-def ligand_preparation(mol, boron_replacement=False, seed=43):
-    """
-    If input ligand is not a 3D structure a conformer will be generated by RDKit, otherwise the provided 3D structure
-    will be used. Boron atoms are replaced with carbon to enable docking using Vina and gnina
-    :param mol:
-    :param boron_replacement: indicate to whether replace boron with carbon atoms or not
-    :param seed: fixed to 43 to generate consistent random stereoisomers for compounds with undefined stereocenters
-    :return: PDBQT block
-    """
-
-    try:
-        mol = mol_embedding_3d(mol, seed=seed)
-        if mol:
-            if boron_replacement:
-                idx_boron = [a.GetIdx() for a in mol.GetAtoms() if a.GetAtomicNum() == 5]
-                for id_ in idx_boron:
-                    if mol.GetAtomWithIdx(id_).GetFormalCharge() < 0:
-                        mol.GetAtomWithIdx(id_).SetFormalCharge(0)
-                    mol.GetAtomWithIdx(id_).SetAtomicNum(6)
-                    # mol.UpdatePropertyCache() # uncomment if necessary
-            mol_conf_pdbqt = mk_prepare_ligand(mol, verbose=False)
-            return mol_conf_pdbqt
-    except Exception:
-        traceback.print_exc()
-        return None
-
-
-def fix_pdbqt(pdbqt_block):
-    pdbqt_fixed = []
-    for line in pdbqt_block.split('\n'):
-        if not line.startswith('HETATM') and not line.startswith('ATOM'):
-            pdbqt_fixed.append(line)
-            continue
-        atom_type = line[12:16].strip()
-        # autodock vina types
-        if 'CA' in line[77:79]: #Calcium is exception
-            atom_pdbqt_type = 'CA'
-        else:
-            atom_pdbqt_type = re.sub('D|A', '', line[77:79]).strip() # can add meeko macrocycle types (G and \d (CG0 etc) in the sub expression if will be going to use it
-
-        if re.search('\d', atom_type[0]) or len(atom_pdbqt_type) == 2: #1HG or two-letter atom names such as CL,FE starts with 13
-            atom_format_type = '{:<4s}'.format(atom_type)
-        else:  # starts with 14
-            atom_format_type = ' {:<3s}'.format(atom_type)
-        line = line[:12] + atom_format_type + line[16:]
-        pdbqt_fixed.append(line)
-
-    return '\n'.join(pdbqt_fixed)
-
-
-def assign_bonds_from_template(template_mol, mol):
-    # explicit hydrogends are removed from carbon atoms (chiral hydrogens) to match pdbqt mol,
-    # e.g. [NH3+][C@H](C)C(=O)[O-]
-    template_mol_ = Chem.Mol(template_mol)
-    template_mol_ = Chem.AddHs(template_mol_, explicitOnly=True,
-                               onlyOnAtoms=[a.GetIdx() for a in template_mol_.GetAtoms() if
-                                            a.GetAtomicNum() != 6])
-    mol = AllChem.AssignBondOrdersFromTemplate(template_mol_, mol)
-    Chem.SanitizeMol(mol)
-    Chem.AssignStereochemistry(mol, cleanIt=True, force=True, flagPossibleStereoCenters=True)
-    return mol
-
-
-def boron_reduction(mol_B, mol):
-    mol_B_ = Chem.Mol(mol_B)
-    mol_ = Chem.Mol(mol)
-
-    idx_boron = {a.GetIdx(): a.GetFormalCharge() for a in mol_B_.GetAtoms() if a.GetAtomicNum() == 5}
-    if idx_boron:
-
-        for id_, charge in idx_boron.items():
-            if charge < 0:
-                mol_B_.GetAtomWithIdx(id_).SetFormalCharge(0)
-            mol_B_.GetAtomWithIdx(id_).SetAtomicNum(6)
-
-        mol_ = assign_bonds_from_template(mol_B_, mol_)
-        idx = mol_.GetSubstructMatches(mol_B_)
-        mol_idx_boron = [tuple(sorted((ids[i], j) for i, j in idx_boron.items())) for ids in idx]
-        mol_idx_boron = list(set(mol_idx_boron))  # retrieve all ids matched possible boron atom positions
-        if len(mol_idx_boron) == 1:  # check whether this set of ids is unique
-            for id_, charge in mol_idx_boron[0]:
-                mol_.GetAtomWithIdx(id_).SetAtomicNum(5)
-                mol_.GetAtomWithIdx(id_).SetFormalCharge(charge)
-        else:  # if not - several equivalent mappings exist
-            sys.stderr.write('different mappings was detected. The structure cannot be recostructed automatically.')
-            return None
-
-    return mol_
-
-
-def pdbqt2molblock(pdbqt_block, template_mol, mol_id):
-    """
-    The function takes PDBQT block with one or more poses and converts top pose to MDL MOL format. The function tries
-    to return back boron atoms
-    :param pdbqt_block: a single string with a single PDBQT block (a single pose)
-    :param template_mol: Mol of a reference structure to assign bond orders
-    :param mol_id: name of a molecule which will be added as a title in the output MOL block
-    :param boron_replacement: indicate whether to try to return boron atoms instead af carbon ones
-    :return: a single string with a MOL block, if conversion failed returns None
-    """
-    mol_block = None
-    fixed = False
-    while mol_block is None:
-        mol = Chem.MolFromPDBBlock('\n'.join([i[:66] for i in pdbqt_block.split('\n')]), removeHs=False, sanitize=False)
-        try:
-            if 5 in [atom.GetAtomicNum() for atom in template_mol.GetAtoms()]:
-                mol = boron_reduction(template_mol, mol)
-            else:
-                mol = assign_bonds_from_template(template_mol, mol)
-            mol.SetProp('_Name', mol_id)
-            mol_block = Chem.MolToMolBlock(mol)
-        except ValueError:
-            if fixed:  # if a molecule was already fixed and the error persists - simply break and return None
-                sys.stderr.write(f'Parsing PDB was failed (fixing did not help): {mol_id}\n')
-                break
-            sys.stderr.write(f'Could not assign bond orders while parsing PDB: {mol_id}. Trying to fix.\n')
-            pdbqt_block = fix_pdbqt(pdbqt_block)
-            fixed = True
-    return mol_block
 
 
 def create_db(db_fname, args, args_to_save=(), config_args_to_save=('protein', 'protein_setup')):
     """
     Create empty database structure and the setup table, which is filled with values. To setup table two fields are
     always stored: yaml file with all input args of the docking script and yaml file with docking config
     :param db_fname: file name of output DB
@@ -450,15 +164,15 @@
     d = yaml.safe_load(db_conn.execute("SELECT yaml FROM setup").fetchone()[0])
     return not d['no_protonation']
 
 
 def update_db(db_conn, mol_id, data, table_name='mols', commit=True):
     """
 
-    :param db_fname:
+    :param db_conn:
     :param mol_id: is of a molecule to update values
     :param data: dict of column names and values to update
     :param table_name:
     :return:
     """
     if data:
         cols, values = zip(*data.items())
@@ -538,7 +252,161 @@
         if mol_block is None:
             mol = Chem.MolFromSmiles(smi)
         else:
             mol = Chem.MolFromMolBlock(mol_block, removeHs=False)
         if mol:
             mol.SetProp('_Name', mol_id)
             yield mol
+
+
+def add_protonation(db_fname, tautomerize=True, table_name='mols', add_sql=''):
+    '''
+    Protonate SMILES by Chemaxon cxcalc utility to get molecule ionization states at pH 7.4
+    :param db_fname:
+    :param tautomerize: get a major tautomer at protonation
+    :param table_name: table name with molecules to protonate
+    :param add_sql: additional SQL query to be appended to the SQL query to retrieve molecules for protonation,
+                    e.g. "AND id IN ('MOL1', 'MOL2')" or "AND iteration=(SELECT MAX(iteration) FROM mols)".
+    :return:
+    '''
+    conn = sqlite3.connect(db_fname)
+
+    try:
+        cur = conn.cursor()
+
+        sql = f"""SELECT smi, source_mol_block, id 
+                  FROM {table_name} 
+                  WHERE docking_score is NULL AND smi_protonated is NULL """
+        sql += add_sql
+
+        data_list = list(cur.execute(sql))
+        if not data_list:
+            sys.stderr.write(f'no molecules to protonate\n')
+            return
+
+        smi_ids = []
+        mol_ids = []
+        for i, (smi, mol_block, mol_name) in enumerate(data_list):
+            if mol_block is None:
+                smi_ids.append(mol_name)
+                # add missing mol blocks
+                m = Chem.MolFromSmiles(data_list[i][0])
+                m.SetProp('_Name', mol_name)
+                m_block = Chem.MolToMolBlock(m)
+                data_list[i] = (smi, m_block, mol_name)
+            else:
+                mol_ids.append(mol_name)
+        smi_ids = set(smi_ids)
+        mol_ids = set(mol_ids)
+
+        output_data_smi = []
+        output_data_mol = []
+        with tempfile.NamedTemporaryFile(suffix='.smi', mode='w', encoding='utf-8') as tmp:
+            fd, output = tempfile.mkstemp()  # use output file to avoid overflow of stdout in extreme cases
+            try:
+                for smi, _, mol_id in data_list:
+                    tmp.write(f'{smi}\t{mol_id}\n')
+                tmp.flush()
+                cmd_run = f"cxcalc -S --ignore-error majormicrospecies -H 7.4 " \
+                          f"{'-M' if tautomerize else ''} -K '{tmp.name}' > '{output}'"
+                subprocess.call(cmd_run, shell=True)
+                for mol in Chem.SDMolSupplier(output, sanitize=False):
+                    if mol:
+                        mol_name = mol.GetProp('_Name')
+                        smi = mol.GetPropsAsDict().get('MAJORMS', None)
+                        if smi is not None:
+                            try:
+                                cansmi = Chem.CanonSmiles(smi)
+                            except:
+                                sys.stderr.write(f'EASYDOCK ERROR: {mol_name}, smiles {smi} obtained after protonation '
+                                                 f'could not be read by RDKit. The molecule was skipped.\n')
+                                continue
+                            if mol_name in smi_ids:
+                                output_data_smi.append((cansmi, mol_name))
+                            elif mol_name in mol_ids:
+                                try:
+                                    # mol block in chemaxon sdf is an input molecule but with 2d structure
+                                    # because input is SMILES
+                                    # to assign proper 3D coordinates we load 3D mol from DB,  make all bonds single,
+                                    # remove Hs and assign bond orders from SMILES
+                                    # this should work even if a generated tautomer differs from the input molecule
+                                    mol3d = get_mols(conn, [mol_name], field_name='source_mol_block')
+                                    mol3d = Chem.RemoveHs(Chem.RWMol(mol3d[0]))
+                                    for b in mol3d.GetBonds():
+                                        b.SetBondType(Chem.BondType.SINGLE)
+                                    ref_mol = Chem.RemoveHs(Chem.MolFromSmiles(smi))
+                                    mol = AllChem.AssignBondOrdersFromTemplate(ref_mol, mol3d)
+                                    Chem.AssignStereochemistryFrom3D(mol)  # not sure whether it is necessary
+                                    output_data_mol.append((cansmi, Chem.MolToMolBlock(mol), mol_name))
+                                except ValueError:
+                                    continue
+            finally:
+                os.remove(output)
+                os.close(fd)
+
+        cur.executemany(f"""UPDATE {table_name}
+                       SET 
+                           smi_protonated = ?
+                       WHERE
+                           id = ?
+                    """, output_data_smi)
+        cur.executemany(f"""UPDATE {table_name}
+                       SET 
+                           smi_protonated = ?, 
+                           source_mol_block_protonated = ?
+                       WHERE
+                           id = ?
+                    """, output_data_mol)
+        conn.commit()
+
+    finally:
+        conn.close()
+
+
+def select_from_db(cur, sql, values):
+    """
+    It makes SELECTs by chunks and works if too many values should be returned from DB.
+    Workaround of the limitation of SQLite3 on the number of values in a query (https://www.sqlite.org/limits.html,
+    section 9).
+    :param cur: curson or connection to db
+    :param sql: SQL query, where a single question mark identify position where to insert multiple values, e.g.
+                "SELECT smi FROM mols WHERE id IN (?)". This question mark will be replaced with multiple ones.
+                So, only one such a symbol should be present in the query.
+    :param values: list of values which will substitute the question mark in the query
+    :return: generator over results retrieved from DB
+    """
+    if sql.count('?') > 1:
+        raise ValueError('SQL query should contain only one question mark.')
+    chunks = iter(partial(take, 32000, iter(values)), [])  # split values on chunks with up to 32000 items
+    for chunk in chunks:
+        for item in cur.execute(sql.replace('?', ','.join('?' * len(chunk))), chunk):
+            yield item
+
+
+def get_mols(conn, mol_ids, field_name='mol_block'):
+    """
+    Returns list of Mol objects from docking DB, order is arbitrary, molecules with errors will be silently skipped
+    :param conn: connection to docking DB
+    :param mol_ids: list of molecules to retrieve
+    :param field_name: name of the field from which a molecule should be retrieved
+    :return:
+    """
+    if field_name in ['mol_block', 'source_mol_block']:
+        func = partial(Chem.MolFromMolBlock, removeHs=False)
+    elif field_name in ['smi']:
+        func = Chem.MolFromSmiles
+    else:
+        raise AttributeError(f'Wrong field name was specified for a get_mols functions. '
+                             f'Allowed: mol_block, source_mol_block, smi. Supplied: {field_name}')
+
+    cur = conn.cursor()
+    # one "?" because we use the special retrieve function - select_from_db - which does it in chunks
+    sql = f'SELECT {field_name} FROM mols WHERE id IN (?) AND {field_name} IS NOT NULL'
+
+    mols = []
+    for items in select_from_db(cur, sql, mol_ids):
+        m = func(items[0])
+        if m:
+            Chem.AssignStereochemistryFrom3D(m)
+            mols.append(m)
+    cur.close()
+    return mols
```

### Comparing `easydock-0.2.2/easydock/run_dock.py` & `easydock-0.2.3/easydock/run_dock.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 import sqlite3
 import sys
 from functools import partial
 from multiprocessing import Pool
 
 from rdkit import Chem
 from rdkit.Chem.rdMolDescriptors import CalcNumRotatableBonds
-from easydock.preparation_for_docking import create_db, restore_setup_from_db, init_db, save_sdf, add_protonation, \
-    cpu_type, filepath_type, update_db, select_mols_to_dock
+from easydock.database import create_db, restore_setup_from_db, init_db, update_db, save_sdf, select_mols_to_dock, \
+    add_protonation
+from easydock.preparation_for_docking import cpu_type, filepath_type
 
 
 class RawTextArgumentDefaultsHelpFormatter(argparse.RawTextHelpFormatter, argparse.ArgumentDefaultsHelpFormatter):
     pass
 
 
 def get_supplied_args(parser):
@@ -204,15 +205,15 @@
             raise ValueError(f'Illegal program argument was supplied: {args.program}')
 
         if args.dask_report:
             dask_report_fname = os.path.splitext(args.output)[0] + '.html'
         else:
             dask_report_fname = None
 
-        with sqlite3.connect(args.output) as conn:
+        with sqlite3.connect(args.output, timeout=60) as conn:
             mols = select_mols_to_dock(conn)
             i = 0
             for i, (mol_id, res) in enumerate(docking(mols,
                                                       dock_func=mol_dock,
                                                       dock_config=args.config,
                                                       priority_func=pred_dock_time,
                                                       ncpu=args.ncpu,
```

### Comparing `easydock-0.2.2/easydock/vina_dock_cli.py` & `easydock-0.2.3/easydock/vina_dock_cli.py`

 * *Files identical despite different names*

### Comparing `easydock-0.2.2/easydock/read_input.py` & `easydock-0.2.3/easydock/read_input.py`

 * *Files identical despite different names*

### Comparing `easydock-0.2.2/easydock/get_sdf_from_dock_db.py` & `easydock-0.2.3/easydock/get_sdf_from_dock_db.py`

 * *Files identical despite different names*

### Comparing `easydock-0.2.2/easydock/vina_dock.py` & `easydock-0.2.3/easydock/vina_dock.py`

 * *Files identical despite different names*

### Comparing `easydock-0.2.2/easydock/gnina_dock.py` & `easydock-0.2.3/easydock/gnina_dock.py`

 * *Files identical despite different names*

### Comparing `easydock-0.2.2/README.md` & `easydock-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -46,32 +46,34 @@
 - docking with `vina`/`gnina`
 - output poses are converted in MOL format and stored into output DB along with docking scores
 
 ### Example
 
 ##### Docking from command line
 
-Docking using `vina` takes input SMILES and a config file. Ligands will not be protonated with Chemaxon, so their supplied charged states will be used. 4 CPU cores will be used. When docking will finish an SDF file will be created with top docking poses for each ligand. 
+Docking using `vina` takes input SMILES and a config file. Ligands will not be protonated with Chemaxon, so their supplied charged states will be used. 4 CPU cores will be used (4 molecules will be dock in parallel). When docking will finish an SDF file will be created with top docking poses for each ligand. 
 ```
-run_dock -i input.smi -o output.db --program vina -c config.yml --no_protonation -c 4 --sdf
+run_dock -i input.smi -o output.db --program vina --config config.yml --no_protonation -c 4 --sdf
 ``` 
 
 Example of config.yml for `vina` docking  
 ```
 protein: /path/to/protein.pdbqt
 protein_setup: /path/to/grid.txt
 exhaustiveness: 8
 seed: 0
 n_poses: 5
 ncpu: 5
 ```
 
+NOTE: ncpu argument in `run_dock` and `config.yml` has different meaning. In `run_dock` it means the number of molecules docked in parallel. In `config.yml` it means the number of CPUs used for docking of a single molecule. The product of these two values should be equal or a little bit more than the number of CPUs on a computer.
+
 The same but using `gnina`
 ```
-run_dock -i input.smi -o output.db --program gnina -c config.yml --no_protonation -c 4 --sdf
+run_dock -i input.smi -o output.db --program gnina --config config.yml --no_protonation -c 4 --sdf
 ``` 
 
 Example of config.yml for `gnina` docking  
 ```
 script_file: /path/to/gnina_executable
 protein: /path/to/protein.pdbqt
 protein_setup: /path/to/grid.txt
@@ -106,14 +108,18 @@
 
 ```bash
 dask ssh --hostfile $PBS_NODEFILE --nworkers 15 --nthreads 1 &
 sleep 10
 run_dock -i input.smi -o output.db --program vina -c config.yml --no_protonation -c 4 --sdf --hostfile $PBS_NODEFILE --dask_report
 ```
 `$PBS_NODEFILE` is a file containing list of IP addresses of servers. The first one from the list will be used by a dask scheduler, but it will also participate in computations.
+
+`--nworkers` is the number of workers per host. This is the number of molecules which are docked in parallel on a single host.
+
+`--nthreads` can be any value. The number of CPUs used for docking of a single molecule will be taken from `config.yml`.
   
 `--dask_report` argument will create at the end of calculations an html-file with performance report (may be useful to tweak docking parameters).
   
 **Important setup issue** - the limit of open files on every server should be increased to the level at least twice the total number of requested workers (file streams are used for inter-node communication by dask).
 
 ##### Data retrieval from the output database
 
@@ -156,14 +162,21 @@
 
 ##### Customization
 
 To implement support of a custom docking program one should implement a function like `mol_dock` which will take as input an RDKit mol object (named molecule) and an yml-file with all docking parameters. The function should run a command line script/utility and return back a tuple of a molecule name and a dictionary of parameters and their values which should be stored in DB (parameter names should be exactly the same as corresponding field names in DB). For examples, please look at `mol_dock` functions in `vina_dock` or `gnina_dock`.
 
 ### Changelog
 
+**0.2.3**
+- improve descriptions of examples on README
+- catch all exceptions in conversion of PDBQT to Mol
+- move DB related functions to a new database.py module
+- use SMILES temporary file to protonate molecules with cxcalc
+- add functions to get molecules from DB in Python (get_mols, select_from_db)
+
 **0.2.2**
 - fix bug with continuation of calculations after db was transferred to other machine
 - restrict precedence of command line arguments over arguments restored from DB only to specific ones (output, hostfile, dask_report, ncpu, verbose)
 
 **0.2.1**
 - fix treatment of molecule ids in get_sdf_from_dock_db
 - change installation instructions, vina must be installed from sources
```

### Comparing `easydock-0.2.2/easydock.egg-info/PKG-INFO` & `easydock-0.2.3/easydock.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easydock
-Version: 0.2.2
+Version: 0.2.3
 Summary: EasyDock Python module to facilitate molecular docking
 Home-page: https://github.com/ci-lab-cz/easydock
 Author: Pavel Polishchuk, Guzel Minibaeva, Aleksandra Ivanova
 Author-email: pavel_polishchuk@ukr.net
 License: UNKNOWN
 Description: # EasyDock - Python module to automate molecular docking
         
@@ -54,32 +54,34 @@
         - docking with `vina`/`gnina`
         - output poses are converted in MOL format and stored into output DB along with docking scores
         
         ### Example
         
         ##### Docking from command line
         
-        Docking using `vina` takes input SMILES and a config file. Ligands will not be protonated with Chemaxon, so their supplied charged states will be used. 4 CPU cores will be used. When docking will finish an SDF file will be created with top docking poses for each ligand. 
+        Docking using `vina` takes input SMILES and a config file. Ligands will not be protonated with Chemaxon, so their supplied charged states will be used. 4 CPU cores will be used (4 molecules will be dock in parallel). When docking will finish an SDF file will be created with top docking poses for each ligand. 
         ```
-        run_dock -i input.smi -o output.db --program vina -c config.yml --no_protonation -c 4 --sdf
+        run_dock -i input.smi -o output.db --program vina --config config.yml --no_protonation -c 4 --sdf
         ``` 
         
         Example of config.yml for `vina` docking  
         ```
         protein: /path/to/protein.pdbqt
         protein_setup: /path/to/grid.txt
         exhaustiveness: 8
         seed: 0
         n_poses: 5
         ncpu: 5
         ```
         
+        NOTE: ncpu argument in `run_dock` and `config.yml` has different meaning. In `run_dock` it means the number of molecules docked in parallel. In `config.yml` it means the number of CPUs used for docking of a single molecule. The product of these two values should be equal or a little bit more than the number of CPUs on a computer.
+        
         The same but using `gnina`
         ```
-        run_dock -i input.smi -o output.db --program gnina -c config.yml --no_protonation -c 4 --sdf
+        run_dock -i input.smi -o output.db --program gnina --config config.yml --no_protonation -c 4 --sdf
         ``` 
         
         Example of config.yml for `gnina` docking  
         ```
         script_file: /path/to/gnina_executable
         protein: /path/to/protein.pdbqt
         protein_setup: /path/to/grid.txt
@@ -114,14 +116,18 @@
         
         ```bash
         dask ssh --hostfile $PBS_NODEFILE --nworkers 15 --nthreads 1 &
         sleep 10
         run_dock -i input.smi -o output.db --program vina -c config.yml --no_protonation -c 4 --sdf --hostfile $PBS_NODEFILE --dask_report
         ```
         `$PBS_NODEFILE` is a file containing list of IP addresses of servers. The first one from the list will be used by a dask scheduler, but it will also participate in computations.
+        
+        `--nworkers` is the number of workers per host. This is the number of molecules which are docked in parallel on a single host.
+        
+        `--nthreads` can be any value. The number of CPUs used for docking of a single molecule will be taken from `config.yml`.
           
         `--dask_report` argument will create at the end of calculations an html-file with performance report (may be useful to tweak docking parameters).
           
         **Important setup issue** - the limit of open files on every server should be increased to the level at least twice the total number of requested workers (file streams are used for inter-node communication by dask).
         
         ##### Data retrieval from the output database
         
@@ -164,14 +170,21 @@
         
         ##### Customization
         
         To implement support of a custom docking program one should implement a function like `mol_dock` which will take as input an RDKit mol object (named molecule) and an yml-file with all docking parameters. The function should run a command line script/utility and return back a tuple of a molecule name and a dictionary of parameters and their values which should be stored in DB (parameter names should be exactly the same as corresponding field names in DB). For examples, please look at `mol_dock` functions in `vina_dock` or `gnina_dock`.
         
         ### Changelog
         
+        **0.2.3**
+        - improve descriptions of examples on README
+        - catch all exceptions in conversion of PDBQT to Mol
+        - move DB related functions to a new database.py module
+        - use SMILES temporary file to protonate molecules with cxcalc
+        - add functions to get molecules from DB in Python (get_mols, select_from_db)
+        
         **0.2.2**
         - fix bug with continuation of calculations after db was transferred to other machine
         - restrict precedence of command line arguments over arguments restored from DB only to specific ones (output, hostfile, dask_report, ncpu, verbose)
         
         **0.2.1**
         - fix treatment of molecule ids in get_sdf_from_dock_db
         - change installation instructions, vina must be installed from sources
```

### Comparing `easydock-0.2.2/setup.py` & `easydock-0.2.3/setup.py`

 * *Files identical despite different names*

