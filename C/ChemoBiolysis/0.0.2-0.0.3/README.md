# Comparing `tmp/ChemoBiolysis-0.0.2.tar.gz` & `tmp/ChemoBiolysis-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChemoBiolysis-0.0.2.tar", last modified: Mon Apr  1 13:32:53 2024, max compression
+gzip compressed data, was "ChemoBiolysis-0.0.3.tar", last modified: Thu Apr 25 00:36:17 2024, max compression
```

## Comparing `ChemoBiolysis-0.0.2.tar` & `ChemoBiolysis-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 13:32:53.433894 ChemoBiolysis-0.0.2/
--rw-rw-rw-   0        0        0       84 2023-12-14 04:42:20.000000 ChemoBiolysis-0.0.2/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2024-04-01 13:32:53.390847 ChemoBiolysis-0.0.2/ChemoBiolysis/
--rw-rw-rw-   0        0        0    88834 2024-04-01 03:38:57.000000 ChemoBiolysis-0.0.2/ChemoBiolysis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:32:53.429907 ChemoBiolysis-0.0.2/ChemoBiolysis.egg-info/
--rw-rw-rw-   0        0        0     2758 2024-04-01 13:32:53.000000 ChemoBiolysis-0.0.2/ChemoBiolysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-01 13:32:53.000000 ChemoBiolysis-0.0.2/ChemoBiolysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 13:32:53.000000 ChemoBiolysis-0.0.2/ChemoBiolysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      240 2024-04-01 13:32:53.000000 ChemoBiolysis-0.0.2/ChemoBiolysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-01 13:32:53.000000 ChemoBiolysis-0.0.2/ChemoBiolysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1053 2023-12-09 17:25:26.000000 ChemoBiolysis-0.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0       26 2023-12-09 17:19:48.000000 ChemoBiolysis-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2758 2024-04-01 13:32:53.431928 ChemoBiolysis-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2053 2023-12-15 19:14:47.000000 ChemoBiolysis-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-01 13:32:53.433894 ChemoBiolysis-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1426 2024-04-01 13:31:58.000000 ChemoBiolysis-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 00:36:17.438649 ChemoBiolysis-0.0.3/
+-rw-rw-rw-   0        0        0       84 2023-12-14 04:42:20.000000 ChemoBiolysis-0.0.3/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 00:36:17.381843 ChemoBiolysis-0.0.3/ChemoBiolysis/
+-rw-rw-rw-   0        0        0   102226 2024-04-22 04:55:24.000000 ChemoBiolysis-0.0.3/ChemoBiolysis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 00:36:17.426305 ChemoBiolysis-0.0.3/ChemoBiolysis.egg-info/
+-rw-rw-rw-   0        0        0     2758 2024-04-25 00:36:16.000000 ChemoBiolysis-0.0.3/ChemoBiolysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-25 00:36:16.000000 ChemoBiolysis-0.0.3/ChemoBiolysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 00:36:16.000000 ChemoBiolysis-0.0.3/ChemoBiolysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      240 2024-04-25 00:36:16.000000 ChemoBiolysis-0.0.3/ChemoBiolysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-25 00:36:16.000000 ChemoBiolysis-0.0.3/ChemoBiolysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1053 2023-12-09 17:25:26.000000 ChemoBiolysis-0.0.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       26 2023-12-09 17:19:48.000000 ChemoBiolysis-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2758 2024-04-25 00:36:17.431337 ChemoBiolysis-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2053 2023-12-15 19:14:47.000000 ChemoBiolysis-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-25 00:36:17.441180 ChemoBiolysis-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1426 2024-04-25 00:34:22.000000 ChemoBiolysis-0.0.3/setup.py
```

### Comparing `ChemoBiolysis-0.0.2/ChemoBiolysis/__init__.py` & `ChemoBiolysis-0.0.3/ChemoBiolysis/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2320,7 +2320,388 @@
     print(f"Processed data with Morgan fingerprints saved to {output_csv}")
 
 
 # Example usage:
 #input_csv = "AID_1860_datatable_inactive.csv"
 #smiles_column = "SMILES"
 #process_csv_and_compute_morgan_fp(input_csv, smiles_column)
+import pandas as pd
+
+
+def find_unique_values(csv_file, column_name):
+    """
+    Read a CSV file and find unique values in a specified column.
+
+    Parameters:
+        csv_file (str): Path to the CSV file.
+        column_name (str): Name of the column to find unique values from.
+
+    Returns:
+        list: A list of unique values found in the specified column.
+    """
+    try:
+        # Read the CSV file
+        df = pd.read_csv(csv_file)
+
+        # Find unique values in the specified column
+        unique_values = df[column_name].unique().tolist()
+
+        return unique_values
+    except Exception as e:
+        print(f"An error occurred: {e}")
+        return []
+
+
+# Example usage:
+#csv_file = "pubchem_taxid_287_bioactivity.csv"  # Replace "example.csv" with the path to your CSV file
+#column_name = "aid"  # Replace "AID" with the name of the column you want to find unique values from
+#unique_values = find_unique_values(csv_file, column_name)
+#print(unique_values)
+import pandas as pd
+
+
+def substance_sid_to_cid_1(*substance_sids):
+    """Retrieve all AID URLs for given substance SIDs."""
+    # Assuming substance_sid_conversion and get_text_from_url are defined elsewhere
+    url = substance_sid_conversion(str(substance_sids[0]), record_type='cids/txt')
+    cid = get_text_from_url(url[0])
+    return cid
+
+
+def compound_cid_to_CanonicalSMILES(compound_cids):
+    print
+    """Retrieve CanonicalSMILES for given compound CIDs."""
+    # Assuming compound_cid_conversion is defined elsewhere
+    url = compound_cid_conversion(*compound_cids, record_type="property/CanonicalSMILES/txt")
+    smiles = get_text_from_url(url[0])
+
+    return smiles
+
+
+import pandas as pd
+
+
+def substance_sid_to_cid_1(*substance_sids):
+    """Retrieve all AID URLs for given substance SIDs."""
+    # Assuming substance_sid_conversion and get_text_from_url are defined elsewhere
+    url = substance_sid_conversion(str(substance_sids[0]), record_type='cids/txt')
+    cid = get_text_from_url(url[0])
+    return cid
+
+
+def compound_cid_to_CanonicalSMILES(compound_cids):
+    print
+    """Retrieve CanonicalSMILES for given compound CIDs."""
+    # Assuming compound_cid_conversion is defined elsewhere
+    url = compound_cid_conversion(*compound_cids, record_type="property/CanonicalSMILES/txt")
+    smiles = get_text_from_url(url[0])
+
+    return smiles
+
+
+def sid_to_smiles_csv(input_file, output_file):
+    # Read the CSV file
+    df = pd.read_csv(input_file)
+
+    # Loop over 'sid' column and retrieve corresponding 'cid'
+    cids = []
+    for sid in df['SID']:
+        cid = substance_sid_to_cid_1(sid)
+        cids.append(cid)
+
+    # Add 'cid' column to DataFrame
+    df['cid'] = cids
+
+    # Loop over 'cid' column and find corresponding 'CanonicalSMILES'
+    smiles = []
+    for cid in df['cid']:
+        smile = compound_cid_to_CanonicalSMILES(cid)
+        smiles.append(smile)
+
+    # Add 'CanonicalSMILES' column to DataFrame
+    df['CanonicalSMILES'] = smiles
+
+    # Save DataFrame to CSV with new columns
+    df.to_csv(output_file, index=False)
+
+    # Display the DataFrame
+    display(df)
+    return
+
+
+import pandas as pd
+import pubchempy as pcp
+
+
+def add_smiles_from_cid(csv_file, cid_column):
+    def cid_to_smiles(cid):
+        try:
+            compound = pcp.Compound.from_cid(cid)
+            smiles = compound.canonical_smiles
+            return smiles
+        except pcp.PubChemHTTPError:
+            print(f"Could not retrieve SMILES for CID {cid}")
+            return None
+
+    # Load CSV file
+    df = pd.read_csv(csv_file)
+
+    # Loop over CID column and find corresponding SMILES
+    smiles_list = []
+    for cid in df[cid_column]:
+        cid = str(int(cid))
+        smiles = cid_to_smiles(cid)
+        smiles_list.append(smiles)
+
+    # Add the SMILES column to the DataFrame
+    df['SMILES'] = smiles_list
+
+    # Save the updated DataFrame to a new CSV file
+    output_file = csv_file.split('.')[0] + '_with_SMILES.csv'
+    df.to_csv(output_file, index=False)
+    return df
+
+
+# Example usage:
+#add_smiles_from_cid('1.xlsx', 'cid')
+
+import pandas as pd
+import matplotlib.pyplot as plt
+from rdkit import Chem
+from rdkit.Chem import Draw
+from rdkit.Chem import rdFMCS
+from rdkit import DataStructs
+from rdkit.Chem import AllChem
+from sklearn.cluster import AgglomerativeClustering
+import numpy as np
+
+def highlight_substructure(mol, substructure_atoms):
+    highlighted = Chem.Mol(mol)
+    for atom in highlighted.GetAtoms():
+        if atom.GetIdx() in substructure_atoms:
+            atom.SetAtomMapNum(1)  # Mark atoms in substructure
+        else:
+            atom.SetAtomMapNum(0)
+    return highlighted
+
+def chemical_cluster_analysis(csv_file_path, smiles_column, similarity_threshold=0.8):
+    # Read the CSV file
+    df = pd.read_csv(csv_file_path)
+
+    # Extract SMILES from the DataFrame
+    smiles = df[smiles_column]
+
+    # Convert SMILES to molecular objects
+    mols = [Chem.MolFromSmiles(smi) for smi in smiles]
+
+    # Generate Morgan fingerprints
+    fps = [AllChem.GetMorganFingerprintAsBitVect(mol, 2, nBits=1024) for mol in mols]
+
+    # Calculate similarity matrix
+    similarity_matrix = np.zeros((len(mols), len(mols)))
+    for i in range(len(mols)):
+        for j in range(i, len(mols)):
+            similarity_matrix[i][j] = similarity_matrix[j][i] = DataStructs.TanimotoSimilarity(fps[i], fps[j])
+
+    # Perform hierarchical clustering with dynamic threshold
+    clustering = AgglomerativeClustering(n_clusters=None, affinity='precomputed', linkage='average', distance_threshold=1-similarity_threshold)
+    labels = clustering.fit_predict(similarity_matrix)
+
+    # Get the number of clusters
+    num_clusters = len(set(labels))
+
+    # Visualize the chemicals in each cluster and find common substructure
+    for label in range(num_clusters):  # Iterate over unique labels assigned by the clustering algorithm
+        print(f"Cluster {label + 1}:")
+        cluster_indices = [idx for idx, l in enumerate(labels) if l == label]
+        mols_in_cluster = [mols[idx] for idx in cluster_indices]
+
+        num_images = len(mols_in_cluster)
+        num_cols = min(num_images, 5)  # Set maximum of 5 images per line
+        num_rows = num_images // num_cols + (1 if num_images % num_cols != 0 else 0)
+
+        fig, axes = plt.subplots(num_rows, num_cols, figsize=(num_cols * 5, num_rows * 5))
+        axes = axes.flatten() if isinstance(axes, np.ndarray) else [axes]  # Ensure axes is a list
+
+        for ax, mol, idx in zip(axes, mols_in_cluster, cluster_indices):
+            if mol is not None:
+                ax.imshow(Draw.MolToImage(mol, size=(200, 200)))
+                ax.set_title(smiles[idx], fontsize=10)
+                ax.axis('off')
+
+                # Find common substructure for this cluster
+                if len(mols_in_cluster) > 1:
+                    mcs_result = rdFMCS.FindMCS(mols_in_cluster, threshold=0.5)
+                    common_substructure = Chem.MolFromSmarts(mcs_result.smartsString)
+                    if common_substructure is not None:
+                        atom_indices = [atom.GetIdx() for atom in common_substructure.GetAtoms()]
+                        highlighted_mol = highlight_substructure(mol, atom_indices)
+                        ax.imshow(Draw.MolToImage(highlighted_mol, size=(200, 200)))
+
+        # Find and display the common substructure for this cluster
+        print("Common substructure for this cluster:")
+        all_mols_in_cluster = [mol for mol in mols_in_cluster if mol is not None]
+        if len(all_mols_in_cluster) > 1:
+            mcs_result = rdFMCS.FindMCS(all_mols_in_cluster, threshold=0.7)
+            common_substructure = Chem.MolFromSmarts(mcs_result.smartsString)
+            if common_substructure is not None:
+                print(Chem.MolToSmiles(common_substructure))
+                display(common_substructure)
+        else:
+            print("There is only one chemical in this cluster, so there is no common substructure.")
+
+        plt.tight_layout()
+        plt.show()
+
+# Example usage:
+#chemical_cluster_analysis('smile pa.csv', smiles_column='SMILES', similarity_threshold=0.95)
+
+
+import pandas as pd
+import matplotlib.pyplot as plt
+from rdkit import Chem
+from rdkit.Chem import Draw
+from rdkit.Chem import rdFMCS
+from rdkit import DataStructs
+from rdkit.Chem import AllChem
+from sklearn.cluster import AgglomerativeClustering
+import numpy as np
+
+def highlight_substructure(mol, substructure_atoms):
+    highlighted = Chem.Mol(mol)
+    for atom in highlighted.GetAtoms():
+        if atom.GetIdx() in substructure_atoms:
+            atom.SetAtomMapNum(1)  # Mark atoms in substructure
+        else:
+            atom.SetAtomMapNum(0)
+    return highlighted
+
+def find_common_substructure(mols):
+    # Find common substructure for the given list of molecules
+    if len(mols) > 1:
+        mcs_result = rdFMCS.FindMCS(mols, threshold=0.7)
+        common_substructure = Chem.MolFromSmarts(mcs_result.smartsString)
+        return common_substructure
+    else:
+        return None
+
+def cluster_analysis_with_size(csv_file_path, smiles_column, cluster_size=10):
+    # Read the CSV file
+    df = pd.read_csv(csv_file_path)
+
+    # Extract SMILES from the DataFrame
+    smiles = df[smiles_column]
+
+    # Convert SMILES to molecular objects
+    mols = [Chem.MolFromSmiles(smi) for smi in smiles if Chem.MolFromSmiles(smi) is not None]
+
+    # Generate Morgan fingerprints
+    fps = [AllChem.GetMorganFingerprintAsBitVect(mol, 2, nBits=1024) for mol in mols]
+
+    # Calculate pairwise Tanimoto similarities
+    similarity_matrix = np.zeros((len(mols), len(mols)))
+    for i in range(len(mols)):
+        for j in range(i, len(mols)):
+            similarity_matrix[i][j] = similarity_matrix[j][i] = DataStructs.TanimotoSimilarity(fps[i], fps[j])
+
+    # Perform hierarchical clustering
+    clustering = AgglomerativeClustering(n_clusters=None, affinity='precomputed', linkage='average', distance_threshold=1.0e9)
+    labels = clustering.fit_predict(similarity_matrix)
+
+    # Initialize clusters
+    num_clusters = len(set(labels))
+    clusters = [[] for _ in range(num_clusters)]
+
+    # Assign molecules to clusters based on their similarity
+    for idx, mol in enumerate(mols):
+        label = labels[idx]
+        clusters[label].append(mol)
+
+    # Divide clusters into subclusters with specified size
+    subclusters = []
+    for cluster in clusters:
+        if len(cluster) <= cluster_size:
+            subclusters.append([cluster])
+        else:
+            num_subclusters = len(cluster) // cluster_size
+            for i in range(num_subclusters):
+                subcluster = cluster[i * cluster_size: (i + 1) * cluster_size]
+                subclusters.append(subcluster)
+            if len(cluster) % cluster_size != 0:
+                subclusters.append(cluster[num_subclusters * cluster_size:])
+
+    # Visualize clusters and find common substructures
+    for idx, subcluster in enumerate(subclusters):
+        print(f"Cluster {idx + 1}:")
+        if len(subcluster) == 0:
+            print("This cluster is empty.")
+            continue
+        # Visualize the chemicals in this cluster
+        num_images = len(subcluster)
+        num_cols = min(num_images, 5)  # Set maximum of 5 images per line
+        num_rows = num_images // num_cols + (1 if num_images % num_cols != 0 else 0)
+
+        fig, axes = plt.subplots(num_rows, num_cols, figsize=(num_cols * 5, num_rows * 5))
+        axes = axes.flatten() if isinstance(axes, np.ndarray) else [axes]  # Ensure axes is a list
+
+        for ax, mol in zip(axes, subcluster):
+            if mol is not None:
+                ax.imshow(Draw.MolToImage(mol, size=(200, 200)))
+                ax.axis('off')
+
+        plt.tight_layout()
+        plt.show()
+
+        # Find and display the common substructure for this cluster
+        print("Common substructure for this cluster:")
+        common_substructure = find_common_substructure(subcluster)
+        if common_substructure is not None:
+            print(Chem.MolToSmiles(common_substructure))
+            display(common_substructure)
+        else:
+            print("There is no common substructure in this cluster.")
+
+# Example usage:
+#cluster_analysis_with_size('smile pa25.csv', smiles_column='SMILES', cluster_size=10)
+
+
+import pandas as pd
+import pubchempy as pcp
+
+
+def cid_to_smiles(cid):
+    try:
+        compound = pcp.Compound.from_cid(cid)
+        smiles = compound.canonical_smiles
+        return smiles
+    except pcp.PubChemHTTPError:
+        print(f"Could not retrieve SMILES for CID {cid}")
+        return None
+
+
+def add_smiles_column(csv_file, cid_column):
+    # Load CSV file
+    df = pd.read_csv(csv_file)
+
+    # Loop over CID column and find corresponding SMILES
+    smiles_list = []
+    for cid in df[cid_column]:
+        if pd.notna(cid):  # Check if CID is not empty
+            cid_str = str(int(cid))  # Convert CID to string
+            smiles = cid_to_smiles(cid_str)  # Get SMILES for CID
+        else:
+            smiles = None  # If CID is empty, set SMILES to None
+        smiles_list.append(smiles)
+
+    # Add the SMILES column to the DataFrame
+    df['SMILES'] = smiles_list
+
+    # Save the updated DataFrame to a new CSV file
+    output_file = csv_file.split('.')[0] + '_with_SMILES.csv'
+    df.to_csv(output_file, index=False)
+    display(df)
+
+    print("SMILES column added and saved successfully!")
+
+
+# Example usage:
+#add_smiles_column('11.csv', 'cid')
```

### Comparing `ChemoBiolysis-0.0.2/ChemoBiolysis.egg-info/PKG-INFO` & `ChemoBiolysis-0.0.3/ChemoBiolysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChemoBiolysis
-Version: 0.0.2
+Version: 0.0.3
 Summary: ChemoBiolysis: A Comprehensive Python Package for Chemical and Biological Analysis
 Home-page: https://github.com/ahmed1212212/ChemoBiolysis.git
 Author: Ahmed Alhilal
 Author-email: aalhilal@udel.edu
 License: MIT
 Keywords: Cheminformatics
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ChemoBiolysis-0.0.2/LICENCE.txt` & `ChemoBiolysis-0.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `ChemoBiolysis-0.0.2/PKG-INFO` & `ChemoBiolysis-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChemoBiolysis
-Version: 0.0.2
+Version: 0.0.3
 Summary: ChemoBiolysis: A Comprehensive Python Package for Chemical and Biological Analysis
 Home-page: https://github.com/ahmed1212212/ChemoBiolysis.git
 Author: Ahmed Alhilal
 Author-email: aalhilal@udel.edu
 License: MIT
 Keywords: Cheminformatics
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ChemoBiolysis-0.0.2/README.md` & `ChemoBiolysis-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ChemoBiolysis-0.0.2/setup.py` & `ChemoBiolysis-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='ChemoBiolysis',
-    version='0.0.2',
+    version='0.0.3',
     description='ChemoBiolysis: A Comprehensive Python Package for Chemical and Biological Analysis',
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='https://github.com/ahmed1212212/ChemoBiolysis.git',
     author='Ahmed Alhilal',
     author_email='aalhilal@udel.edu',
     license='MIT',
     classifiers=classifiers,
```

