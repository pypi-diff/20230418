# Comparing `tmp/vdk-meta-jobs-0.1.836044868.tar.gz` & `tmp/vdk-meta-jobs-0.1.840981730.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-meta-jobs-0.1.836044868.tar", last modified: Thu Apr 13 09:30:52 2023, max compression
+gzip compressed data, was "vdk-meta-jobs-0.1.840981730.tar", last modified: Tue Apr 18 14:42:56 2023, max compression
```

## Comparing `vdk-meta-jobs-0.1.836044868.tar` & `vdk-meta-jobs-0.1.840981730.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:30:52.977267 vdk-meta-jobs-0.1.836044868/
--rw-r--r--   0 root         (0) root         (0)     6645 2023-04-13 09:30:52.977267 vdk-meta-jobs-0.1.836044868/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6072 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 09:30:52.977267 vdk-meta-jobs-0.1.836044868/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1456 2023-04-13 09:30:42.000000 vdk-meta-jobs-0.1.836044868/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:30:52.973267 vdk-meta-jobs-0.1.836044868/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:30:52.973267 vdk-meta-jobs-0.1.836044868/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:30:52.973267 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:30:52.977267 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:30:52.977267 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/api/
--rw-rw-rw-   0 root         (0) root         (0)     1402 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/api/meta_job.py
--rw-rw-rw-   0 root         (0) root         (0)     9347 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/cached_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     7949 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/dag_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/dags_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2269 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     6713 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/meta_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     6148 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/meta_dag.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/meta_job_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     9344 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/remote_data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1743 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/remote_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     2579 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/time_based_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:30:52.977267 vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6645 2023-04-13 09:30:52.000000 vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      858 2023-04-13 09:30:52.000000 vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 09:30:52.000000 vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-13 09:30:52.000000 vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-13 09:30:52.000000 vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-13 09:30:52.000000 vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:30:52.977267 vdk-meta-jobs-0.1.836044868/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2624 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/tests/test_meta_dag.py
--rw-rw-rw-   0 root         (0) root         (0)    15096 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/tests/test_meta_job.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/tests/test_time_based_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2303 2023-04-13 09:30:38.000000 vdk-meta-jobs-0.1.836044868/tests/test_tracking_job_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:42:56.147864 vdk-meta-jobs-0.1.840981730/
+-rw-r--r--   0 root         (0) root         (0)     8391 2023-04-18 14:42:56.147864 vdk-meta-jobs-0.1.840981730/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7818 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 14:42:56.147864 vdk-meta-jobs-0.1.840981730/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2023-04-18 14:42:46.000000 vdk-meta-jobs-0.1.840981730/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:42:56.143864 vdk-meta-jobs-0.1.840981730/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:42:56.143864 vdk-meta-jobs-0.1.840981730/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:42:56.143864 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:42:56.143864 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:42:56.143864 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1402 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/api/meta_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     9347 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/cached_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7949 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/dag_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/dags_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2269 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     6713 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/meta_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     6148 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/meta_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/meta_job_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     9344 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/remote_data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1743 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/remote_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2579 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/time_based_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:42:56.143864 vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8391 2023-04-18 14:42:56.000000 vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      858 2023-04-18 14:42:56.000000 vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 14:42:56.000000 vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-18 14:42:56.000000 vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-18 14:42:56.000000 vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-18 14:42:56.000000 vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:42:56.147864 vdk-meta-jobs-0.1.840981730/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/tests/test_meta_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)    15096 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/tests/test_meta_job.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/tests/test_time_based_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2303 2023-04-18 14:42:43.000000 vdk-meta-jobs-0.1.840981730/tests/test_tracking_job_executor.py
```

### Comparing `vdk-meta-jobs-0.1.836044868/PKG-INFO` & `vdk-meta-jobs-0.1.840981730/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-meta-jobs
-Version: 0.1.836044868
+Version: 0.1.840981730
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,23 +21,25 @@
 A meta job is a regular Data Job that invokes other Data Jobs using Control Service Execution API.
 In this way, there's nothing different from other data jobs except for its purpose. See [Data Job types](https://github.com/vmware/versatile-data-kit/wiki/User-Guide#data-job-types) for more info.
 
 It's meant to be a much more lightweight alternative to complex and comprehensive workflows solution (like Airflow)
 as it doesn't require to provision any new infrastructure or to need to learn new tool.
 You install a new python library (this plugin itself) and you are ready to go.
 
-Using this plugin you can specify dependencies between data jobs as a direct acyclic graph (DAG). See usage for more information.
+Using this plugin, you can specify dependencies between data jobs as a direct acyclic graph (DAG).
+See [Usage](#usage) for more information.
 
 ## Usage
 
 ```
 pip install vdk-meta-jobs
 ```
 
-Then one would create a single step and define the jobs we want to orchestrate
+Then one would create a single [step](https://github.com/vmware/versatile-data-kit/wiki/dictionary#data-job-step) and
+define the jobs we want to orchestrate:
 
 ```python
 def run(job_input):
     jobs = [
         {
         "job_name": "name-of-job",
         "team_name": "team-of-job",
@@ -47,29 +49,29 @@
         },
         ...
     ]
     MetaJobInput().run_meta_job(jobs)
 ```
 
 When defining a job to be run following attributes are supported:
-* **job_name**: required, the name of the data job
-* **team_name:**: optional, the team of the data job. If omitted , it will use the meta job's team
+* **job_name**: required, the name of the data job.
+* **team_name:**: optional, the team of the data job. If omitted , it will use the meta job's team.
 * **fail_meta_job_on_error**: optional, default is true. If true, the meta job will abort and fail if the orchestrated job fails, if false, meta job won't fail and continue.
 * **arguments**: optional, the arguments that are passed to the underlying orchestrated data job.
 * **depends_on**: required (can be empty), list of other jobs that the orchestrated job depends on. The job will not be started until depends_on job have finished.
 
 
 ### Example
 
 The following example dependency graph can be implemented with below code.
 
 
 ![img_2.png](img_2.png)
 
-In this example what happens is
+In this example what happens is:
 * Job 1 will execute.
 * After Job 1 is completed, jobs 2,3,4 will start executing in parallel.
 * Jobs 5 and 6 will start executing after job 3 completes, but will not wait for the completion of jobs 2 and 4.
 
 
 ```python
 
@@ -124,14 +126,41 @@
 ]
 
 
 def run(job_input: IJobInput) - > None:
     MetaJobInput().run_meta_job(JOBS_RUN_ORDER)
 ```
 
+
+### Runtime sequencing
+
+The depends_on key stores the dependencies of each job - the jobs that have to finish before it starts.
+The DAG execution starts from the jobs with empty dependency lists - they start together in parallel.
+But what happens if they are too many? It could cause server overload. In order to avoid such unfortunate situations,
+a limit in the number of concurrent running jobs is set. This limit is
+a [configuration variable](https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-meta-jobs/src/vdk/plugin/meta_jobs/meta_configuration.py#L87)
+that you are able to set according to your needs. When the limit is exceeded, the execution of the rest of the jobs
+is not cancelled but delayed until a spot is freed by one of the running jobs. What's important here is that
+although there are delayed jobs due to the limitation, the overall sequence is not broken.
+
+
+### Data Job start comparison
+
+There are 3 types of jobs right now in terms of how are they started.
+
+* Started by Schedule
+   * When the time comes for a scheduled execution of a Data Job, if the one is currently running, it will be waited
+     to finish by retrying a few times. If it is still running then, this scheduled execution will be skipped.
+* Started by the user using UI or CLI
+   * If a user tries to start a job that is already running, one would get an appropriate error immediately and a
+     recommendation to try again later.
+* **Started by a DAG Job**
+   * If a DAG job tries to start a job and there is already running such job, the approach of the DAG job would be
+     similar to the schedule - retry later but more times.
+
 ### FAQ
 
 
 **Q: Will the metajob retry on Platform Error?**<br>
 A: Yes, as any other job, up to N (configurable by the Control Service) attempts for each job it is orchestrating.
    See Control Service documentation for more information
```

### Comparing `vdk-meta-jobs-0.1.836044868/README.md` & `vdk-meta-jobs-0.1.840981730/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 A meta job is a regular Data Job that invokes other Data Jobs using Control Service Execution API.
 In this way, there's nothing different from other data jobs except for its purpose. See [Data Job types](https://github.com/vmware/versatile-data-kit/wiki/User-Guide#data-job-types) for more info.
 
 It's meant to be a much more lightweight alternative to complex and comprehensive workflows solution (like Airflow)
 as it doesn't require to provision any new infrastructure or to need to learn new tool.
 You install a new python library (this plugin itself) and you are ready to go.
 
-Using this plugin you can specify dependencies between data jobs as a direct acyclic graph (DAG). See usage for more information.
+Using this plugin, you can specify dependencies between data jobs as a direct acyclic graph (DAG).
+See [Usage](#usage) for more information.
 
 ## Usage
 
 ```
 pip install vdk-meta-jobs
 ```
 
-Then one would create a single step and define the jobs we want to orchestrate
+Then one would create a single [step](https://github.com/vmware/versatile-data-kit/wiki/dictionary#data-job-step) and
+define the jobs we want to orchestrate:
 
 ```python
 def run(job_input):
     jobs = [
         {
         "job_name": "name-of-job",
         "team_name": "team-of-job",
@@ -33,29 +35,29 @@
         },
         ...
     ]
     MetaJobInput().run_meta_job(jobs)
 ```
 
 When defining a job to be run following attributes are supported:
-* **job_name**: required, the name of the data job
-* **team_name:**: optional, the team of the data job. If omitted , it will use the meta job's team
+* **job_name**: required, the name of the data job.
+* **team_name:**: optional, the team of the data job. If omitted , it will use the meta job's team.
 * **fail_meta_job_on_error**: optional, default is true. If true, the meta job will abort and fail if the orchestrated job fails, if false, meta job won't fail and continue.
 * **arguments**: optional, the arguments that are passed to the underlying orchestrated data job.
 * **depends_on**: required (can be empty), list of other jobs that the orchestrated job depends on. The job will not be started until depends_on job have finished.
 
 
 ### Example
 
 The following example dependency graph can be implemented with below code.
 
 
 ![img_2.png](img_2.png)
 
-In this example what happens is
+In this example what happens is:
 * Job 1 will execute.
 * After Job 1 is completed, jobs 2,3,4 will start executing in parallel.
 * Jobs 5 and 6 will start executing after job 3 completes, but will not wait for the completion of jobs 2 and 4.
 
 
 ```python
 
@@ -110,14 +112,41 @@
 ]
 
 
 def run(job_input: IJobInput) - > None:
     MetaJobInput().run_meta_job(JOBS_RUN_ORDER)
 ```
 
+
+### Runtime sequencing
+
+The depends_on key stores the dependencies of each job - the jobs that have to finish before it starts.
+The DAG execution starts from the jobs with empty dependency lists - they start together in parallel.
+But what happens if they are too many? It could cause server overload. In order to avoid such unfortunate situations,
+a limit in the number of concurrent running jobs is set. This limit is
+a [configuration variable](https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-meta-jobs/src/vdk/plugin/meta_jobs/meta_configuration.py#L87)
+that you are able to set according to your needs. When the limit is exceeded, the execution of the rest of the jobs
+is not cancelled but delayed until a spot is freed by one of the running jobs. What's important here is that
+although there are delayed jobs due to the limitation, the overall sequence is not broken.
+
+
+### Data Job start comparison
+
+There are 3 types of jobs right now in terms of how are they started.
+
+* Started by Schedule
+   * When the time comes for a scheduled execution of a Data Job, if the one is currently running, it will be waited
+     to finish by retrying a few times. If it is still running then, this scheduled execution will be skipped.
+* Started by the user using UI or CLI
+   * If a user tries to start a job that is already running, one would get an appropriate error immediately and a
+     recommendation to try again later.
+* **Started by a DAG Job**
+   * If a DAG job tries to start a job and there is already running such job, the approach of the DAG job would be
+     similar to the schedule - retry later but more times.
+
 ### FAQ
 
 
 **Q: Will the metajob retry on Platform Error?**<br>
 A: Yes, as any other job, up to N (configurable by the Control Service) attempts for each job it is orchestrating.
    See Control Service documentation for more information
```

### Comparing `vdk-meta-jobs-0.1.836044868/setup.py` & `vdk-meta-jobs-0.1.840981730/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.836044868"
+__version__ = "0.1.840981730"
 
 setuptools.setup(
     name="vdk-meta-jobs",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Express dependecies between data jobs.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/api/meta_job.py` & `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/api/meta_job.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/cached_data_job_executor.py` & `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/cached_data_job_executor.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/dag_validator.py` & `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/dag_validator.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/dags_plugin.py` & `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/dags_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/meta.py` & `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/meta.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/meta_configuration.py` & `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/meta_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/meta_dag.py` & `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/meta_dag.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/meta_job_runner.py` & `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/meta_job_runner.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/remote_data_job.py` & `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/remote_data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/remote_data_job_executor.py` & `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/remote_data_job_executor.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.836044868/src/vdk/plugin/meta_jobs/time_based_queue.py` & `vdk-meta-jobs-0.1.840981730/src/vdk/plugin/meta_jobs/time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/PKG-INFO` & `vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-meta-jobs
-Version: 0.1.836044868
+Version: 0.1.840981730
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,23 +21,25 @@
 A meta job is a regular Data Job that invokes other Data Jobs using Control Service Execution API.
 In this way, there's nothing different from other data jobs except for its purpose. See [Data Job types](https://github.com/vmware/versatile-data-kit/wiki/User-Guide#data-job-types) for more info.
 
 It's meant to be a much more lightweight alternative to complex and comprehensive workflows solution (like Airflow)
 as it doesn't require to provision any new infrastructure or to need to learn new tool.
 You install a new python library (this plugin itself) and you are ready to go.
 
-Using this plugin you can specify dependencies between data jobs as a direct acyclic graph (DAG). See usage for more information.
+Using this plugin, you can specify dependencies between data jobs as a direct acyclic graph (DAG).
+See [Usage](#usage) for more information.
 
 ## Usage
 
 ```
 pip install vdk-meta-jobs
 ```
 
-Then one would create a single step and define the jobs we want to orchestrate
+Then one would create a single [step](https://github.com/vmware/versatile-data-kit/wiki/dictionary#data-job-step) and
+define the jobs we want to orchestrate:
 
 ```python
 def run(job_input):
     jobs = [
         {
         "job_name": "name-of-job",
         "team_name": "team-of-job",
@@ -47,29 +49,29 @@
         },
         ...
     ]
     MetaJobInput().run_meta_job(jobs)
 ```
 
 When defining a job to be run following attributes are supported:
-* **job_name**: required, the name of the data job
-* **team_name:**: optional, the team of the data job. If omitted , it will use the meta job's team
+* **job_name**: required, the name of the data job.
+* **team_name:**: optional, the team of the data job. If omitted , it will use the meta job's team.
 * **fail_meta_job_on_error**: optional, default is true. If true, the meta job will abort and fail if the orchestrated job fails, if false, meta job won't fail and continue.
 * **arguments**: optional, the arguments that are passed to the underlying orchestrated data job.
 * **depends_on**: required (can be empty), list of other jobs that the orchestrated job depends on. The job will not be started until depends_on job have finished.
 
 
 ### Example
 
 The following example dependency graph can be implemented with below code.
 
 
 ![img_2.png](img_2.png)
 
-In this example what happens is
+In this example what happens is:
 * Job 1 will execute.
 * After Job 1 is completed, jobs 2,3,4 will start executing in parallel.
 * Jobs 5 and 6 will start executing after job 3 completes, but will not wait for the completion of jobs 2 and 4.
 
 
 ```python
 
@@ -124,14 +126,41 @@
 ]
 
 
 def run(job_input: IJobInput) - > None:
     MetaJobInput().run_meta_job(JOBS_RUN_ORDER)
 ```
 
+
+### Runtime sequencing
+
+The depends_on key stores the dependencies of each job - the jobs that have to finish before it starts.
+The DAG execution starts from the jobs with empty dependency lists - they start together in parallel.
+But what happens if they are too many? It could cause server overload. In order to avoid such unfortunate situations,
+a limit in the number of concurrent running jobs is set. This limit is
+a [configuration variable](https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-plugins/vdk-meta-jobs/src/vdk/plugin/meta_jobs/meta_configuration.py#L87)
+that you are able to set according to your needs. When the limit is exceeded, the execution of the rest of the jobs
+is not cancelled but delayed until a spot is freed by one of the running jobs. What's important here is that
+although there are delayed jobs due to the limitation, the overall sequence is not broken.
+
+
+### Data Job start comparison
+
+There are 3 types of jobs right now in terms of how are they started.
+
+* Started by Schedule
+   * When the time comes for a scheduled execution of a Data Job, if the one is currently running, it will be waited
+     to finish by retrying a few times. If it is still running then, this scheduled execution will be skipped.
+* Started by the user using UI or CLI
+   * If a user tries to start a job that is already running, one would get an appropriate error immediately and a
+     recommendation to try again later.
+* **Started by a DAG Job**
+   * If a DAG job tries to start a job and there is already running such job, the approach of the DAG job would be
+     similar to the schedule - retry later but more times.
+
 ### FAQ
 
 
 **Q: Will the metajob retry on Platform Error?**<br>
 A: Yes, as any other job, up to N (configurable by the Control Service) attempts for each job it is orchestrating.
    See Control Service documentation for more information
```

### Comparing `vdk-meta-jobs-0.1.836044868/src/vdk_meta_jobs.egg-info/SOURCES.txt` & `vdk-meta-jobs-0.1.840981730/src/vdk_meta_jobs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.836044868/tests/test_meta_dag.py` & `vdk-meta-jobs-0.1.840981730/tests/test_meta_dag.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.836044868/tests/test_meta_job.py` & `vdk-meta-jobs-0.1.840981730/tests/test_meta_job.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.836044868/tests/test_time_based_queue.py` & `vdk-meta-jobs-0.1.840981730/tests/test_time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-meta-jobs-0.1.836044868/tests/test_tracking_job_executor.py` & `vdk-meta-jobs-0.1.840981730/tests/test_tracking_job_executor.py`

 * *Files identical despite different names*

