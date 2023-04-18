# Comparing `tmp/molbeam_fp-0.1.tar.gz` & `tmp/molbeam_fp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molbeam_fp-0.1.tar", last modified: Tue Apr 18 18:47:56 2023, max compression
+gzip compressed data, was "molbeam_fp-0.1.1.tar", last modified: Tue Apr 18 20:17:40 2023, max compression
```

## Comparing `molbeam_fp-0.1.tar` & `molbeam_fp-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 tgraham    (501) staff       (20)        0 2023-04-18 18:47:56.411706 molbeam_fp-0.1/
--rw-r--r--   0 tgraham    (501) staff       (20)      395 2023-04-18 18:47:56.411525 molbeam_fp-0.1/PKG-INFO
--rw-r--r--   0 tgraham    (501) staff       (20)        0 2023-04-18 18:39:40.000000 molbeam_fp-0.1/README.md
-drwxr-xr-x   0 tgraham    (501) staff       (20)        0 2023-04-18 18:47:56.410871 molbeam_fp-0.1/molbeam_fp/
--rw-r--r--   0 tgraham    (501) staff       (20)        0 2023-04-18 18:29:23.000000 molbeam_fp-0.1/molbeam_fp/__init__.py
--rwxrwxrwx   0 tgraham    (501) staff       (20)     3581 2023-04-18 16:34:52.000000 molbeam_fp-0.1/molbeam_fp/app.py
--rwxrwxrwx   0 tgraham    (501) staff       (20)     2872 2023-04-18 16:37:51.000000 molbeam_fp-0.1/molbeam_fp/large_csv_to_parquet_chunks.py
--rwxrwxrwx   0 tgraham    (501) staff       (20)      376 2022-03-30 13:40:08.000000 molbeam_fp-0.1/molbeam_fp/molbeam.py
--rwxrwxrwx   0 tgraham    (501) staff       (20)      611 2023-04-18 16:25:26.000000 molbeam_fp-0.1/molbeam_fp/mole.py
--rwxrwxrwx   0 tgraham    (501) staff       (20)     4097 2023-04-17 18:45:18.000000 molbeam_fp-0.1/molbeam_fp/process_smiles_to_fp_pq.py
--rwxrwxrwx   0 tgraham    (501) staff       (20)     2678 2023-04-18 16:26:25.000000 molbeam_fp-0.1/molbeam_fp/similarity.py
-drwxr-xr-x   0 tgraham    (501) staff       (20)        0 2023-04-18 18:47:56.411382 molbeam_fp-0.1/molbeam_fp.egg-info/
--rw-r--r--   0 tgraham    (501) staff       (20)      395 2023-04-18 18:47:56.000000 molbeam_fp-0.1/molbeam_fp.egg-info/PKG-INFO
--rw-r--r--   0 tgraham    (501) staff       (20)      374 2023-04-18 18:47:56.000000 molbeam_fp-0.1/molbeam_fp.egg-info/SOURCES.txt
--rw-r--r--   0 tgraham    (501) staff       (20)        1 2023-04-18 18:47:56.000000 molbeam_fp-0.1/molbeam_fp.egg-info/dependency_links.txt
--rw-r--r--   0 tgraham    (501) staff       (20)       36 2023-04-18 18:47:56.000000 molbeam_fp-0.1/molbeam_fp.egg-info/requires.txt
--rw-r--r--   0 tgraham    (501) staff       (20)       11 2023-04-18 18:47:56.000000 molbeam_fp-0.1/molbeam_fp.egg-info/top_level.txt
--rw-r--r--   0 tgraham    (501) staff       (20)       38 2023-04-18 18:47:56.411740 molbeam_fp-0.1/setup.cfg
--rw-r--r--   0 tgraham    (501) staff       (20)      606 2023-04-18 18:39:06.000000 molbeam_fp-0.1/setup.py
+drwxr-xr-x   0 tgraham    (501) staff       (20)        0 2023-04-18 20:17:40.075703 molbeam_fp-0.1.1/
+-rw-r--r--   0 tgraham    (501) staff       (20)     1070 2023-04-18 19:03:17.000000 molbeam_fp-0.1.1/LICENSE
+-rw-r--r--   0 tgraham    (501) staff       (20)      419 2023-04-18 20:17:40.075550 molbeam_fp-0.1.1/PKG-INFO
+-rw-r--r--   0 tgraham    (501) staff       (20)        0 2023-04-18 18:39:40.000000 molbeam_fp-0.1.1/README.md
+drwxr-xr-x   0 tgraham    (501) staff       (20)        0 2023-04-18 20:17:40.074722 molbeam_fp-0.1.1/molbeam_fp/
+-rw-r--r--   0 tgraham    (501) staff       (20)        0 2023-04-18 18:29:23.000000 molbeam_fp-0.1.1/molbeam_fp/__init__.py
+-rwxrwxrwx   0 tgraham    (501) staff       (20)     3581 2023-04-18 16:34:52.000000 molbeam_fp-0.1.1/molbeam_fp/app.py
+-rwxrwxrwx   0 tgraham    (501) staff       (20)     3037 2023-04-18 19:44:57.000000 molbeam_fp-0.1.1/molbeam_fp/large_csv_to_parquet_chunks.py
+-rwxrwxrwx   0 tgraham    (501) staff       (20)      376 2022-03-30 13:40:08.000000 molbeam_fp-0.1.1/molbeam_fp/molbeam.py
+-rwxrwxrwx   0 tgraham    (501) staff       (20)      611 2023-04-18 16:25:26.000000 molbeam_fp-0.1.1/molbeam_fp/mole.py
+-rwxrwxrwx   0 tgraham    (501) staff       (20)     4217 2023-04-18 19:23:06.000000 molbeam_fp-0.1.1/molbeam_fp/process_smiles_to_fp_pq.py
+-rwxrwxrwx   0 tgraham    (501) staff       (20)     2678 2023-04-18 16:26:25.000000 molbeam_fp-0.1.1/molbeam_fp/similarity.py
+drwxr-xr-x   0 tgraham    (501) staff       (20)        0 2023-04-18 20:17:40.075340 molbeam_fp-0.1.1/molbeam_fp.egg-info/
+-rw-r--r--   0 tgraham    (501) staff       (20)      419 2023-04-18 20:17:40.000000 molbeam_fp-0.1.1/molbeam_fp.egg-info/PKG-INFO
+-rw-r--r--   0 tgraham    (501) staff       (20)      419 2023-04-18 20:17:40.000000 molbeam_fp-0.1.1/molbeam_fp.egg-info/SOURCES.txt
+-rw-r--r--   0 tgraham    (501) staff       (20)        1 2023-04-18 20:17:40.000000 molbeam_fp-0.1.1/molbeam_fp.egg-info/dependency_links.txt
+-rw-r--r--   0 tgraham    (501) staff       (20)      193 2023-04-18 20:17:40.000000 molbeam_fp-0.1.1/molbeam_fp.egg-info/entry_points.txt
+-rw-r--r--   0 tgraham    (501) staff       (20)       36 2023-04-18 20:17:40.000000 molbeam_fp-0.1.1/molbeam_fp.egg-info/requires.txt
+-rw-r--r--   0 tgraham    (501) staff       (20)       11 2023-04-18 20:17:40.000000 molbeam_fp-0.1.1/molbeam_fp.egg-info/top_level.txt
+-rw-r--r--   0 tgraham    (501) staff       (20)       38 2023-04-18 20:17:40.075747 molbeam_fp-0.1.1/setup.cfg
+-rw-r--r--   0 tgraham    (501) staff       (20)      887 2023-04-18 20:17:20.000000 molbeam_fp-0.1.1/setup.py
```

### Comparing `molbeam_fp-0.1/molbeam_fp/app.py` & `molbeam_fp-0.1.1/molbeam_fp/app.py`

 * *Files identical despite different names*

### Comparing `molbeam_fp-0.1/molbeam_fp/large_csv_to_parquet_chunks.py` & `molbeam_fp-0.1.1/molbeam_fp/large_csv_to_parquet_chunks.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,16 +31,17 @@
         duration = timedelta(seconds=te - ts)
         print(f"{method.__name__}: {duration}")
         return result
     return timed
 
 
 class InputStreamReader:
-    def __init__(self, file_stream):
+    def __init__(self, file_stream, include_columns):
         self.file_stream = file_stream
+        self.include_columns = include_columns
         self._stream = None
 
     def batches(self):
         i = tries = 0
         while True:
             try:
                 batch = self.__next_batch()
@@ -54,15 +55,15 @@
 
 
     @property
     def stream(self):
         if not self._stream:
             read_options = pa.csv.ReadOptions(block_size=2097152)
             parse_options = pa.csv.ParseOptions(delimiter='\t')
-            convert_options = pa.csv.ConvertOptions(include_columns=include_columns)
+            convert_options = pa.csv.ConvertOptions(include_columns=self.include_columns)
             self._stream = pa.csv.open_csv(
                 self.file_stream, read_options=read_options,
                 parse_options=parse_options,
                 convert_options=convert_options
             
         )
         return self._stream
@@ -73,15 +74,15 @@
                  input_file_to_stream, \
                  output_file_stream_directory, \
                  output_file_prefix, \
                  smiles_column_title):
     
     print('Initiating stream.')
     
-    input_stream_reader = InputStreamReader(input_file_to_stream)
+    input_stream_reader = InputStreamReader(input_file_to_stream, include_columns)
     
     outfiles_list = []
     
     for i, batch in input_stream_reader.batches():
         print(f'Ingesting batch number {i}')
         df = batch.to_pandas()
         table = pa.Table.from_pandas(df)
@@ -92,18 +93,22 @@
         ParquetWriter(outfile, schema).write_table(table)
         print(f'Wrote parquet to {outfile}')
         outfiles_list.append(outfile)
         
     return outfile
 
 
+def main():
 
-include_columns = [column1, column2]
+    include_columns = [column1, column2]
 
-outfiles = csv_stream_to_parquet_batch_writer(include_columns, \
-                     file, \
-                     output_dir, \
-                     output_prefix, \
-                     column1)
+    outfiles = csv_stream_to_parquet_batch_writer(include_columns, \
+                         file, \
+                         output_dir, \
+                         output_prefix, \
+                         column1)
 
-print(outfiles)
+    print(outfiles)
+
+if __name__ == '__main__':
+    main()
```

### Comparing `molbeam_fp-0.1/molbeam_fp/mole.py` & `molbeam_fp-0.1.1/molbeam_fp/mole.py`

 * *Files identical despite different names*

### Comparing `molbeam_fp-0.1/molbeam_fp/process_smiles_to_fp_pq.py` & `molbeam_fp-0.1.1/molbeam_fp/process_smiles_to_fp_pq.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,31 +81,35 @@
 dataset_dir = sys.argv[1]
 output_dir = sys.argv[2]
 out_prefix = sys.argv[3]
 smiles_column = 'smiles'
 dataset_format = 'parquet'
 n_jobs = 5
 
-dataset = ds.dataset(dataset_dir, format=dataset_format)
+def main():
+    dataset = ds.dataset(dataset_dir, format=dataset_format)
 
-# Create a list of fragments that are not memory loaded
-fragments = [file for file in dataset.get_fragments()]
+    # Create a list of fragments that are not memory loaded
+    fragments = [file for file in dataset.get_fragments()]
 
-total_frags = len(fragments)
-print(f'There are a total of {len(fragments)} fragments in the dataset: {output_dir}')
+    total_frags = len(fragments)
+    print(f'There are a total of {len(fragments)} fragments in the dataset: {output_dir}')
 
-for count,element in tenumerate(fragments, start=0, total=None):
-    
+    for count,element in tenumerate(fragments, start=0, total=None):
+        
 
-    console.print(f'Starting fragment dataset: {count} in {dataset_dir}', style="blue bold")
-    #cast the fragment as a pandas df
-    df = element.to_table().to_pandas()
-    df2 = prep_parquet_db(df, n_jobs, smiles_column)
+        console.print(f'Starting fragment dataset: {count} in {dataset_dir}', style="blue bold")
+        #cast the fragment as a pandas df
+        df = element.to_table().to_pandas()
+        df2 = prep_parquet_db(df, n_jobs, smiles_column)
 
-    console.print(f'There are a total of {len(df2)} valid smiles strings with fingerprints', style="green bold")
+        console.print(f'There are a total of {len(df2)} valid smiles strings with fingerprints', style="green bold")
 
-    table = pa.Table.from_pandas(df2, preserve_index=False)
+        table = pa.Table.from_pandas(df2, preserve_index=False)
 
-    
-    #write the molchunk to disk
-    pq.write_table(table, f'{output_dir}/{out_prefix}_{count}.parquet')
-    console.print(f'Wrote parquet to {output_dir}/{out_prefix}_{count}.parquet', style="purple bold")
+        
+        #write the molchunk to disk
+        pq.write_table(table, f'{output_dir}/{out_prefix}_{count}.parquet')
+        console.print(f'Wrote parquet to {output_dir}/{out_prefix}_{count}.parquet', style="purple bold")
+
+if __name__ == '__main__':
+    main()
```

### Comparing `molbeam_fp-0.1/molbeam_fp/similarity.py` & `molbeam_fp-0.1.1/molbeam_fp/similarity.py`

 * *Files identical despite different names*

