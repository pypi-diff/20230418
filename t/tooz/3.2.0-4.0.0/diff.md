# Comparing `tmp/tooz-3.2.0.tar.gz` & `tmp/tooz-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooz-3.2.0.tar", last modified: Thu Oct 20 11:06:52 2022, max compression
+gzip compressed data, was "tooz-4.0.0.tar", last modified: Tue Apr 18 12:32:26 2023, max compression
```

## Comparing `tooz-3.2.0.tar` & `tooz-4.0.0.tar`

### file list

```diff
@@ -1,138 +1,139 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.572362 tooz-3.2.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2022-10-20 11:06:28.000000 tooz-3.2.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2022-10-20 11:06:28.000000 tooz-3.2.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2022-10-20 11:06:28.000000 tooz-3.2.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4918 2022-10-20 11:06:28.000000 tooz-3.2.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3611 2022-10-20 11:06:52.000000 tooz-3.2.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      656 2022-10-20 11:06:28.000000 tooz-3.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24642 2022-10-20 11:06:52.000000 tooz-3.2.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-10-20 11:06:28.000000 tooz-3.2.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2174 2022-10-20 11:06:52.572362 tooz-3.2.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2022-10-20 11:06:28.000000 tooz-3.2.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2022-10-20 11:06:28.000000 tooz-3.2.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.548362 tooz-3.2.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      641 2022-10-20 11:06:28.000000 tooz-3.2.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.548362 tooz-3.2.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2996 2022-10-20 11:06:28.000000 tooz-3.2.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2022-10-20 11:06:28.000000 tooz-3.2.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.548362 tooz-3.2.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      875 2022-10-20 11:06:28.000000 tooz-3.2.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.548362 tooz-3.2.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1499 2022-10-20 11:06:28.000000 tooz-3.2.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.552362 tooz-3.2.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3450 2022-10-20 11:06:28.000000 tooz-3.2.0/doc/source/user/compatibility.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7249 2022-10-20 11:06:28.000000 tooz-3.2.0/doc/source/user/drivers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2022-10-20 11:06:28.000000 tooz-3.2.0/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2022-10-20 11:06:28.000000 tooz-3.2.0/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.552362 tooz-3.2.0/doc/source/user/tutorial/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1592 2022-10-20 11:06:28.000000 tooz-3.2.0/doc/source/user/tutorial/coordinator.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1569 2022-10-20 11:06:28.000000 tooz-3.2.0/doc/source/user/tutorial/group_membership.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2022-10-20 11:06:28.000000 tooz-3.2.0/doc/source/user/tutorial/hashring.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2022-10-20 11:06:28.000000 tooz-3.2.0/doc/source/user/tutorial/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2022-10-20 11:06:28.000000 tooz-3.2.0/doc/source/user/tutorial/leader_election.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2022-10-20 11:06:28.000000 tooz-3.2.0/doc/source/user/tutorial/lock.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2022-10-20 11:06:28.000000 tooz-3.2.0/doc/source/user/tutorial/partitioner.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.552362 tooz-3.2.0/examples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2022-10-20 11:06:28.000000 tooz-3.2.0/examples/coordinator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2022-10-20 11:06:28.000000 tooz-3.2.0/examples/coordinator_heartbeat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2022-10-20 11:06:28.000000 tooz-3.2.0/examples/group_membership.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2022-10-20 11:06:28.000000 tooz-3.2.0/examples/group_membership_watch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1106 2022-10-20 11:06:28.000000 tooz-3.2.0/examples/hashring.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2022-10-20 11:06:28.000000 tooz-3.2.0/examples/leader_election.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2022-10-20 11:06:28.000000 tooz-3.2.0/examples/lock.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2022-10-20 11:06:28.000000 tooz-3.2.0/examples/partitioner.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.552362 tooz-3.2.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2022-10-20 11:06:28.000000 tooz-3.2.0/playbooks/stop-redis.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.544361 tooz-3.2.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.556362 tooz-3.2.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/add-consul-acl-support-2f0869681129f7e7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/add-reno-996dd44974d53238.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/consul-heartbeat-support-3ec69e2ace537dc1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/deprecate-etcd3-driver-551608037d79222b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/etcd3-etcd3gw-tls-support-618ab207706e67af.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/etcd3-group-support-b039cf19f4a268a3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/etcd3gw-group-support-598832a8764a8aa6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/etcd3gw_create_new_lease_if_expired_during_refresh-1d631d36c21ea28c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/hashring-0470f9119ef63d49.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/hashring-algo-8a279397b8ff8a6a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/join_group_create-5095ec02e20c7242.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/memcached-fix-lock-release-I6fc33b8e0a88510.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/mysql-0.10.0-7660f75a1c57a920.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/mysql-tls-support-88941e2ebaf938b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/partitioner-4005767d287dc7c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/notes/redis-connect-retries-c9adfc81eb06a4ab.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.560362 tooz-3.2.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.560362 tooz-3.2.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.560362 tooz-3.2.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8854 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-10-20 11:06:28.000000 tooz-3.2.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2022-10-20 11:06:28.000000 tooz-3.2.0/requirements.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      194 2022-10-20 11:06:28.000000 tooz-3.2.0/run-examples.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      502 2022-10-20 11:06:28.000000 tooz-3.2.0/run-tests.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1167 2022-10-20 11:06:28.000000 tooz-3.2.0/setup-consul-env.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      724 2022-10-20 11:06:28.000000 tooz-3.2.0/setup-etcd-env.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1987 2022-10-20 11:06:52.576362 tooz-3.2.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1028 2022-10-20 11:06:28.000000 tooz-3.2.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2022-10-20 11:06:28.000000 tooz-3.2.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.560362 tooz-3.2.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3430 2022-10-20 11:06:28.000000 tooz-3.2.0/tools/compat-matrix.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.564362 tooz-3.2.0/tooz/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/_retry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31905 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/coordination.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.568362 tooz-3.2.0/tooz/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20604 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/drivers/consul.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9392 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/drivers/etcd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12833 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/drivers/etcd3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15726 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/drivers/etcd3gw.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20558 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/drivers/file.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8482 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/drivers/ipc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20294 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/drivers/memcached.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8135 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/drivers/mysql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8085 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/drivers/pgsql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30379 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/drivers/redis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2150 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/drivers/zake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24030 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/drivers/zookeeper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5836 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/hashring.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3867 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/locking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3970 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/partitioner.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.572362 tooz-3.2.0/tooz/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2391 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.572362 tooz-3.2.0/tooz/tests/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/tests/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2487 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/tests/drivers/test_etcd3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2992 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/tests/drivers/test_etcd3gw.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2571 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/tests/drivers/test_file.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41543 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/tests/test_coordination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1678 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/tests/test_etcd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10285 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/tests/test_hashring.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3401 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/tests/test_memcache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2997 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/tests/test_mysql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3469 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/tests/test_partitioner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4061 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/tests/test_postgresql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4281 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/tests/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7927 2022-10-20 11:06:28.000000 tooz-3.2.0/tooz/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 11:06:52.564362 tooz-3.2.0/tooz.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2174 2022-10-20 11:06:52.000000 tooz-3.2.0/tooz.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3546 2022-10-20 11:06:52.000000 tooz-3.2.0/tooz.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-10-20 11:06:52.000000 tooz-3.2.0/tooz.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2022-10-20 11:06:52.000000 tooz-3.2.0/tooz.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-10-20 11:06:52.000000 tooz-3.2.0/tooz.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-10-20 11:06:52.000000 tooz-3.2.0/tooz.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      623 2022-10-20 11:06:52.000000 tooz-3.2.0/tooz.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2022-10-20 11:06:52.000000 tooz-3.2.0/tooz.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2331 2022-10-20 11:06:28.000000 tooz-3.2.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.040723 tooz-4.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-04-18 12:32:00.000000 tooz-4.0.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-04-18 12:32:00.000000 tooz-4.0.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2023-04-18 12:32:00.000000 tooz-4.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4972 2023-04-18 12:32:00.000000 tooz-4.0.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3781 2023-04-18 12:32:25.000000 tooz-4.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      656 2023-04-18 12:32:00.000000 tooz-4.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24922 2023-04-18 12:32:25.000000 tooz-4.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-04-18 12:32:00.000000 tooz-4.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2175 2023-04-18 12:32:26.040723 tooz-4.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2023-04-18 12:32:00.000000 tooz-4.0.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-04-18 12:32:00.000000 tooz-4.0.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.012721 tooz-4.0.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2023-04-18 12:32:00.000000 tooz-4.0.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.012721 tooz-4.0.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2996 2023-04-18 12:32:00.000000 tooz-4.0.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2023-04-18 12:32:00.000000 tooz-4.0.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.012721 tooz-4.0.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      875 2023-04-18 12:32:00.000000 tooz-4.0.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.012721 tooz-4.0.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1499 2023-04-18 12:32:00.000000 tooz-4.0.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.012721 tooz-4.0.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3451 2023-04-18 12:32:00.000000 tooz-4.0.0/doc/source/user/compatibility.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7249 2023-04-18 12:32:00.000000 tooz-4.0.0/doc/source/user/drivers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-04-18 12:32:00.000000 tooz-4.0.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-04-18 12:32:00.000000 tooz-4.0.0/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.016721 tooz-4.0.0/doc/source/user/tutorial/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1592 2023-04-18 12:32:00.000000 tooz-4.0.0/doc/source/user/tutorial/coordinator.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1569 2023-04-18 12:32:00.000000 tooz-4.0.0/doc/source/user/tutorial/group_membership.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-04-18 12:32:00.000000 tooz-4.0.0/doc/source/user/tutorial/hashring.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-04-18 12:32:00.000000 tooz-4.0.0/doc/source/user/tutorial/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2023-04-18 12:32:00.000000 tooz-4.0.0/doc/source/user/tutorial/leader_election.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-04-18 12:32:00.000000 tooz-4.0.0/doc/source/user/tutorial/lock.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-04-18 12:32:00.000000 tooz-4.0.0/doc/source/user/tutorial/partitioner.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.016721 tooz-4.0.0/examples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2023-04-18 12:32:00.000000 tooz-4.0.0/examples/coordinator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2023-04-18 12:32:00.000000 tooz-4.0.0/examples/coordinator_heartbeat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2023-04-18 12:32:00.000000 tooz-4.0.0/examples/group_membership.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2023-04-18 12:32:00.000000 tooz-4.0.0/examples/group_membership_watch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1106 2023-04-18 12:32:00.000000 tooz-4.0.0/examples/hashring.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2023-04-18 12:32:00.000000 tooz-4.0.0/examples/leader_election.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2023-04-18 12:32:00.000000 tooz-4.0.0/examples/lock.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2023-04-18 12:32:00.000000 tooz-4.0.0/examples/partitioner.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.016721 tooz-4.0.0/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2023-04-18 12:32:00.000000 tooz-4.0.0/playbooks/stop-redis.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.004721 tooz-4.0.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.024722 tooz-4.0.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/add-consul-acl-support-2f0869681129f7e7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/add-reno-996dd44974d53238.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/consul-heartbeat-support-3ec69e2ace537dc1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/deprecate-etcd3-driver-551608037d79222b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/etcd3-etcd3gw-tls-support-618ab207706e67af.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/etcd3-group-support-b039cf19f4a268a3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/etcd3gw-group-support-598832a8764a8aa6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/etcd3gw_create_new_lease_if_expired_during_refresh-1d631d36c21ea28c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/hashring-0470f9119ef63d49.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/hashring-algo-8a279397b8ff8a6a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/join_group_create-5095ec02e20c7242.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/memcached-fix-lock-release-I6fc33b8e0a88510.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/mysql-0.10.0-7660f75a1c57a920.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/mysql-tls-support-88941e2ebaf938b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/partitioner-4005767d287dc7c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/redis-connect-retries-c9adfc81eb06a4ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/notes/zookeeper_tls-808355fd2ab1acae.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.024722 tooz-4.0.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.024722 tooz-4.0.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.028722 tooz-4.0.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8854 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-18 12:32:00.000000 tooz-4.0.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2023-04-18 12:32:00.000000 tooz-4.0.0/requirements.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      194 2023-04-18 12:32:00.000000 tooz-4.0.0/run-examples.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      502 2023-04-18 12:32:00.000000 tooz-4.0.0/run-tests.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1167 2023-04-18 12:32:00.000000 tooz-4.0.0/setup-consul-env.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      724 2023-04-18 12:32:00.000000 tooz-4.0.0/setup-etcd-env.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1988 2023-04-18 12:32:26.040723 tooz-4.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1028 2023-04-18 12:32:00.000000 tooz-4.0.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2023-04-18 12:32:00.000000 tooz-4.0.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.028722 tooz-4.0.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3431 2023-04-18 12:32:00.000000 tooz-4.0.0/tools/compat-matrix.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.028722 tooz-4.0.0/tooz/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/_retry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31905 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/coordination.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.036723 tooz-4.0.0/tooz/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20604 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/drivers/consul.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9392 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/drivers/etcd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12833 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/drivers/etcd3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15726 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/drivers/etcd3gw.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20558 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/drivers/file.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8482 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/drivers/ipc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20294 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/drivers/memcached.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8318 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/drivers/mysql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8085 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/drivers/pgsql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30379 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/drivers/redis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2150 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/drivers/zake.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24742 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/drivers/zookeeper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5836 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/hashring.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3867 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/locking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3970 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/partitioner.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.036723 tooz-4.0.0/tooz/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2391 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.040723 tooz-4.0.0/tooz/tests/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/tests/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2487 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/tests/drivers/test_etcd3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2992 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/tests/drivers/test_etcd3gw.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2571 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/tests/drivers/test_file.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41543 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/tests/test_coordination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1678 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/tests/test_etcd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10285 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/tests/test_hashring.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3401 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/tests/test_memcache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3495 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/tests/test_mysql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3469 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/tests/test_partitioner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4061 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/tests/test_postgresql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4281 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/tests/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7927 2023-04-18 12:32:00.000000 tooz-4.0.0/tooz/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-18 12:32:26.032722 tooz-4.0.0/tooz.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2175 2023-04-18 12:32:25.000000 tooz-4.0.0/tooz.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3601 2023-04-18 12:32:25.000000 tooz-4.0.0/tooz.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-18 12:32:25.000000 tooz-4.0.0/tooz.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2023-04-18 12:32:25.000000 tooz-4.0.0/tooz.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-18 12:32:25.000000 tooz-4.0.0/tooz.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-04-18 12:32:25.000000 tooz-4.0.0/tooz.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      623 2023-04-18 12:32:25.000000 tooz-4.0.0/tooz.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2023-04-18 12:32:25.000000 tooz-4.0.0/tooz.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2491 2023-04-18 12:32:00.000000 tooz-4.0.0/tox.ini
```

### Comparing `tooz-3.2.0/.pre-commit-config.yaml` & `tooz-4.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/.zuul.yaml` & `tooz-4.0.0/.zuul.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -4,197 +4,197 @@
       - openstack-cover-jobs
       - openstack-python3-jobs
       - periodic-stable-jobs
       - publish-openstack-docs-pti
       - release-notes-jobs-python3
     check:
       jobs:
-        - tooz-tox-py38-etcd
         - tooz-tox-py39-etcd
-        - tooz-tox-py38-etcd3gw
+        - tooz-tox-py310-etcd
         - tooz-tox-py39-etcd3gw
-        - tooz-tox-py38-zookeeper
+        - tooz-tox-py310-etcd3gw
         - tooz-tox-py39-zookeeper
-        - tooz-tox-py38-redis
+        - tooz-tox-py310-zookeeper
         - tooz-tox-py39-redis
-        - tooz-tox-py38-sentinel
+        - tooz-tox-py310-redis
         - tooz-tox-py39-sentinel
-        - tooz-tox-py38-memcached
+        - tooz-tox-py310-sentinel
         - tooz-tox-py39-memcached
-        - tooz-tox-py38-postgresql
+        - tooz-tox-py310-memcached
         - tooz-tox-py39-postgresql
-        - tooz-tox-py38-mysql
+        - tooz-tox-py310-postgresql
         - tooz-tox-py39-mysql
-        - tooz-tox-py38-consul
+        - tooz-tox-py310-mysql
         - tooz-tox-py39-consul
+        - tooz-tox-py310-consul
     gate:
       jobs:
-        - tooz-tox-py38-etcd
         - tooz-tox-py39-etcd
-        - tooz-tox-py38-etcd3gw
+        - tooz-tox-py310-etcd
         - tooz-tox-py39-etcd3gw
-        - tooz-tox-py38-zookeeper
+        - tooz-tox-py310-etcd3gw
         - tooz-tox-py39-zookeeper
-        - tooz-tox-py38-redis
+        - tooz-tox-py310-zookeeper
         - tooz-tox-py39-redis
-        - tooz-tox-py38-sentinel
+        - tooz-tox-py310-redis
         - tooz-tox-py39-sentinel
-        - tooz-tox-py38-memcached
+        - tooz-tox-py310-sentinel
         - tooz-tox-py39-memcached
-        - tooz-tox-py38-postgresql
+        - tooz-tox-py310-memcached
         - tooz-tox-py39-postgresql
-        - tooz-tox-py38-mysql
+        - tooz-tox-py310-postgresql
         - tooz-tox-py39-mysql
-        - tooz-tox-py38-consul
+        - tooz-tox-py310-mysql
         - tooz-tox-py39-consul
+        - tooz-tox-py310-consul
 
 - job:
-    name: tooz-tox-py38-consul
-    parent: openstack-tox-py38
+    name: tooz-tox-py39-consul
+    parent: openstack-tox-py39
     description: |
-      Run tests using ``py38-consul`` environment.
+      Run tests using ``py39-consul`` environment.
     vars:
-      tox_envlist: py38-consul
+      tox_envlist: py39-consul
 
 - job:
-    name: tooz-tox-py38-etcd
-    parent: openstack-tox-py38
+    name: tooz-tox-py39-etcd
+    parent: openstack-tox-py39
     description: |
-      Run tests using ``py38-etcd`` environment.
+      Run tests using ``py39-etcd`` environment.
     vars:
-      tox_envlist: py38-etcd
+      tox_envlist: py39-etcd
 
 - job:
-    name: tooz-tox-py38-etcd3gw
-    parent: openstack-tox-py38
+    name: tooz-tox-py39-etcd3gw
+    parent: openstack-tox-py39
     description: |
-      Run tests using ``py38-etcd3gw`` environment.
+      Run tests using ``py39-etcd3gw`` environment.
     vars:
-      tox_envlist: py38-etcd3gw
+      tox_envlist: py39-etcd3gw
 
 - job:
-    name: tooz-tox-py38-memcached
-    parent: openstack-tox-py38
+    name: tooz-tox-py39-memcached
+    parent: openstack-tox-py39
     description: |
-      Run tests using ``py38-memcached`` environment.
+      Run tests using ``py39-memcached`` environment.
     vars:
-      tox_envlist: py38-memcached
+      tox_envlist: py39-memcached
 
 - job:
-    name: tooz-tox-py38-mysql
-    parent: openstack-tox-py38
+    name: tooz-tox-py39-mysql
+    parent: openstack-tox-py39
     description: |
-      Run tests using ``py38-mysql`` environment.
+      Run tests using ``py39-mysql`` environment.
     vars:
-      tox_envlist: py38-mysql
+      tox_envlist: py39-mysql
 
 - job:
-    name: tooz-tox-py38-postgresql
-    parent: openstack-tox-py38
+    name: tooz-tox-py39-postgresql
+    parent: openstack-tox-py39
     description: |
-      Run tests using ``py38-postgresql`` environment.
+      Run tests using ``py39-postgresql`` environment.
     vars:
-      tox_envlist: py38-postgresql
+      tox_envlist: py39-postgresql
 
 - job:
-    name: tooz-tox-py38-redis
-    parent: openstack-tox-py38
+    name: tooz-tox-py39-redis
+    parent: openstack-tox-py39
     description: |
-      Run tests using ``py38-redis`` environment.
+      Run tests using ``py39-redis`` environment.
     vars:
-      tox_envlist: py38-redis
+      tox_envlist: py39-redis
     pre-run:
       - playbooks/stop-redis.yaml
 
 - job:
-    name: tooz-tox-py38-sentinel
-    parent: openstack-tox-py38
+    name: tooz-tox-py39-sentinel
+    parent: openstack-tox-py39
     description: |
-      Run tests using ``py38-sentinel`` environment.
+      Run tests using ``py39-sentinel`` environment.
     vars:
-      tox_envlist: py38-sentinel
+      tox_envlist: py39-sentinel
     pre-run:
       - playbooks/stop-redis.yaml
 
 - job:
-    name: tooz-tox-py38-zookeeper
-    parent: openstack-tox-py38
+    name: tooz-tox-py39-zookeeper
+    parent: openstack-tox-py39
     description: |
-      Run tests using ``py38-zookeeper`` environment.
+      Run tests using ``py39-zookeeper`` environment.
     vars:
-      tox_envlist: py38-zookeeper
+      tox_envlist: py39-zookeeper
 
 - job:
-    name: tooz-tox-py39-consul
-    parent: openstack-tox-py39
+    name: tooz-tox-py310-consul
+    parent: openstack-tox-py310
     description: |
-      Run tests using ``py39-consul`` environment.
+      Run tests using ``py310-consul`` environment.
     vars:
-      tox_envlist: py39-consul
+      tox_envlist: py310-consul
 
 - job:
-    name: tooz-tox-py39-etcd
-    parent: openstack-tox-py39
+    name: tooz-tox-py310-etcd
+    parent: openstack-tox-py310
     description: |
-      Run tests using ``py39-etcd`` environment.
+      Run tests using ``py310-etcd`` environment.
     vars:
-      tox_envlist: py39-etcd
+      tox_envlist: py310-etcd
 
 - job:
-    name: tooz-tox-py39-etcd3gw
-    parent: openstack-tox-py39
+    name: tooz-tox-py310-etcd3gw
+    parent: openstack-tox-py310
     description: |
-      Run tests using ``py39-etcd3gw`` environment.
+      Run tests using ``py310-etcd3gw`` environment.
     vars:
-      tox_envlist: py39-etcd3gw
+      tox_envlist: py310-etcd3gw
 
 - job:
-    name: tooz-tox-py39-memcached
-    parent: openstack-tox-py39
+    name: tooz-tox-py310-memcached
+    parent: openstack-tox-py310
     description: |
-      Run tests using ``py39-memcached`` environment.
+      Run tests using ``py310-memcached`` environment.
     vars:
-      tox_envlist: py39-memcached
+      tox_envlist: py310-memcached
 
 - job:
-    name: tooz-tox-py39-mysql
-    parent: openstack-tox-py39
+    name: tooz-tox-py310-mysql
+    parent: openstack-tox-py310
     description: |
-      Run tests using ``py39-mysql`` environment.
+      Run tests using ``py310-mysql`` environment.
     vars:
-      tox_envlist: py39-mysql
+      tox_envlist: py310-mysql
 
 - job:
-    name: tooz-tox-py39-postgresql
-    parent: openstack-tox-py39
+    name: tooz-tox-py310-postgresql
+    parent: openstack-tox-py310
     description: |
-      Run tests using ``py39-postgresql`` environment.
+      Run tests using ``py310-postgresql`` environment.
     vars:
-      tox_envlist: py39-postgresql
+      tox_envlist: py310-postgresql
 
 - job:
-    name: tooz-tox-py39-redis
-    parent: openstack-tox-py39
+    name: tooz-tox-py310-redis
+    parent: openstack-tox-py310
     description: |
-      Run tests using ``py39-redis`` environment.
+      Run tests using ``py310-redis`` environment.
     vars:
-      tox_envlist: py39-redis
+      tox_envlist: py310-redis
     pre-run:
       - playbooks/stop-redis.yaml
 
 - job:
-    name: tooz-tox-py39-sentinel
-    parent: openstack-tox-py39
+    name: tooz-tox-py310-sentinel
+    parent: openstack-tox-py310
     description: |
-      Run tests using ``py39-sentinel`` environment.
+      Run tests using ``py310-sentinel`` environment.
     vars:
-      tox_envlist: py39-sentinel
+      tox_envlist: py310-sentinel
     pre-run:
       - playbooks/stop-redis.yaml
 
 - job:
-    name: tooz-tox-py39-zookeeper
-    parent: openstack-tox-py39
+    name: tooz-tox-py310-zookeeper
+    parent: openstack-tox-py310
     description: |
-      Run tests using ``py39-zookeeper`` environment.
+      Run tests using ``py310-zookeeper`` environment.
     vars:
-      tox_envlist: py39-zookeeper
+      tox_envlist: py310-zookeeper
```

### Comparing `tooz-3.2.0/AUTHORS` & `tooz-4.0.0/AUTHORS`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 Andreas Jaeger <aj@suse.com>
 Arne Wiebalck <Arne.Wiebalck@cern.ch>
 Ben Nemec <bnemec@redhat.com>
 Bob.Haddleton <bob.haddleton@nokia.com>
 Cao Xuan Hoang <hoangcx@vn.fujitsu.com>
 ChangBo Guo(gcb) <eric.guo@easystack.cn>
 Chris Dent <chdent@redhat.com>
+Christian Rohmann <christian.rohmann@inovex.de>
 Corey Bryant <corey.bryant@canonical.com>
 Daniel Bengtsson <dbengt@redhat.com>
 Davanum Srinivas <davanum@gmail.com>
 Davanum Srinivas <dims@linux.vnet.ibm.com>
 Dina Belova <dbelova@mirantis.com>
 Dirk Mueller <dirk@dmllr.de>
 Dmitriy Rabotjagov <dmitriy.r@sitevalley.com>
+Dmitriy Rabotyagov <dmitriy.rabotyagov@citynetwork.eu>
 Dmitriy Rabotyagov <noonedeadpunk@ya.ru>
 Dmitry Tantsur <dtantsur@protonmail.com>
 Doug Hellmann <doug@doughellmann.com>
 Duong Ha-Quang <duonghq@vn.fujitsu.com>
 Ekaterina Chernova <efedorova@mirantis.com>
 Elod Illes <elod.illes@est.tech>
 Eoghan Glynn <eglynn@redhat.com>
@@ -61,14 +63,15 @@
 Riccardo Pittau <elfosardo@gmail.com>
 Robert Collins <rbtcollins@hp.com>
 Ronald Bradford <ronald.bradford@gmail.com>
 Sahid Orentino Ferdjaoui <sahid.ferdjaoui@canonical.com>
 Sean McGinnis <sean.mcginnis@huawei.com>
 Sergey Lukjanov <slukjanov@mirantis.com>
 Stephen Finucane <stephenfin@redhat.com>
+Takashi Kajinami <tkajinam@redhat.com>
 Thomas Bechtold <tbechtold@suse.com>
 Thomas Herve <therve@redhat.com>
 Tobias Urdin <tobias.urdin@binero.se>
 Tony Breeds <tony@bakeyournoodle.com>
 Victor Morales <victor.morales@intel.com>
 Vilobh Meshram <vilobhmm@yahoo-inc.com>
 XiaojueGuan <guanalbertjone@gmail.com>
@@ -84,14 +87,15 @@
 lahoucine BENLAHMR <lahoucine@benlahmr.com>
 liu-sheng <liusheng@huawei.com>
 maaoyu <maaoyu@inspur.com>
 malei <malei@maleideMacBook-Pro.local>
 manchandavishal <manchandavishal143@gmail.com>
 melissaml <ma.lei@99cloud.net>
 mengalong <alongmeng@gmail.com>
+ricolin <rlin@vexxhost.com>
 ushen <yshxxsjt715@gmail.com>
 yangyawei <yangyawei@inspur.com>
 yenai <yenai@cmss.chinamobile.com>
 zhangguoqing <zhang.guoqing@99cloud.net>
 zhangsong <zhangsong@cmss.chinamobile.com>
 zhangyanxian <zhang.yanxian@zte.com.cn>
 zhen <zhen00fa@gmail.com>
```

### Comparing `tooz-3.2.0/CONTRIBUTING.rst` & `tooz-4.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/ChangeLog` & `tooz-4.0.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 CHANGES
 =======
 
+4.0.0
+-----
+
+* Fix mysql timeout
+* Moves supported python runtimes from version 3.8 to 3.10
+* tox: set allowlist\_externals
+* Allow to pass ssl-related args for zookeeper
+* Loosen protobuf version that's used for docs/renos
+* Add grouping support in etcd to compatibility matrix
+
 3.2.0
 -----
 
 
 3.1.0
 -----
```

### Comparing `tooz-3.2.0/LICENSE` & `tooz-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/PKG-INFO` & `tooz-4.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tooz
-Version: 3.2.0
+Version: 4.0.0
 Summary: Coordination library for distributed systems.
 Home-page: https://docs.openstack.org/tooz/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: Tooz
         ====
@@ -37,20 +37,20 @@
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: System :: Distributed Computing
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Provides-Extra: consul
 Provides-Extra: etcd
 Provides-Extra: etcd3
 Provides-Extra: etcd3gw
 Provides-Extra: ipc
 Provides-Extra: memcached
 Provides-Extra: mysql
```

### Comparing `tooz-3.2.0/README.rst` & `tooz-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/doc/requirements.txt` & `tooz-4.0.0/doc/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ## consul
 python-consul2>=0.0.16 # MIT License
 ## etcd
 requests>=2.10.0 # Apache-2.0
 ## etcd3
 etcd3>=0.12.0 # Apache-2.0
 grpcio>=1.18.0
-protobuf<4.0 # BSD License (3 clause)
+protobuf # BSD License (3 clause)
 ## etcd3gw
 etcd3gw!=0.2.6,>=0.1.0 # Apache-2.0
 ## zake
 zake>=0.1.6 # Apache-2.0
 ## redis
 redis>=3.1.0 # MIT
 ## postgresql
```

### Comparing `tooz-3.2.0/doc/source/conf.py` & `tooz-4.0.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/doc/source/index.rst` & `tooz-4.0.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/doc/source/install/index.rst` & `tooz-4.0.0/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/doc/source/reference/index.rst` & `tooz-4.0.0/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/doc/source/user/compatibility.rst` & `tooz-4.0.0/doc/source/user/compatibility.rst`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
    :header-rows: 1
 
    * - Driver
      - Supported
    * - :py:class:`~tooz.drivers.consul.ConsulDriver`
      - Yes
    * - :py:class:`~tooz.drivers.etcd.EtcdDriver`
-     - No
+     - Yes
    * - :py:class:`~tooz.drivers.file.FileDriver`
      - Yes
    * - :py:class:`~tooz.drivers.ipc.IPCDriver`
      - No
    * - :py:class:`~tooz.drivers.memcached.MemcachedDriver`
      - Yes
    * - :py:class:`~tooz.drivers.mysql.MySQLDriver`
```

### Comparing `tooz-3.2.0/doc/source/user/drivers.rst` & `tooz-4.0.0/doc/source/user/drivers.rst`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/doc/source/user/tutorial/coordinator.rst` & `tooz-4.0.0/doc/source/user/tutorial/coordinator.rst`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/doc/source/user/tutorial/group_membership.rst` & `tooz-4.0.0/doc/source/user/tutorial/group_membership.rst`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/doc/source/user/tutorial/leader_election.rst` & `tooz-4.0.0/doc/source/user/tutorial/leader_election.rst`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/doc/source/user/tutorial/lock.rst` & `tooz-4.0.0/doc/source/user/tutorial/lock.rst`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/examples/coordinator.py` & `tooz-4.0.0/examples/coordinator.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/examples/coordinator_heartbeat.py` & `tooz-4.0.0/examples/coordinator_heartbeat.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/examples/group_membership.py` & `tooz-4.0.0/examples/group_membership.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/examples/group_membership_watch.py` & `tooz-4.0.0/examples/group_membership_watch.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/examples/hashring.py` & `tooz-4.0.0/examples/hashring.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/examples/leader_election.py` & `tooz-4.0.0/examples/leader_election.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/examples/lock.py` & `tooz-4.0.0/examples/lock.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/examples/partitioner.py` & `tooz-4.0.0/examples/partitioner.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/releasenotes/notes/mysql-tls-support-88941e2ebaf938b4.yaml` & `tooz-4.0.0/releasenotes/notes/mysql-tls-support-88941e2ebaf938b4.yaml`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/releasenotes/source/conf.py` & `tooz-4.0.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/setup-consul-env.sh` & `tooz-4.0.0/setup-consul-env.sh`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/setup-etcd-env.sh` & `tooz-4.0.0/setup-etcd-env.sh`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/setup.cfg` & `tooz-4.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 name = tooz
 author = OpenStack
 author_email = openstack-discuss@lists.openstack.org
 summary = Coordination library for distributed systems.
 description_file = README.rst
 license = Apache-2
 home_page = https://docs.openstack.org/tooz/latest/
-python_requires = >=3.8
+python_requires = >=3.9
 classifier = 
 	Environment :: OpenStack
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: System :: Distributed Computing
 
 [files]
 packages = 
 	tooz
@@ -58,15 +58,15 @@
 redis = 
 	redis>=3.1.0 # MIT
 postgresql = 
 	psycopg2>=2.5 # LGPL/ZPL
 mysql = 
 	PyMySQL>=0.6.2 # MIT License
 zookeeper = 
-	kazoo>=2.2 # Apache-2.0
+	kazoo>=2.6 # Apache-2.0
 memcached = 
 	pymemcache!=1.3.0,>=1.2.9 # Apache 2.0 License
 ipc = 
 	sysv-ipc>=0.6.8 # BSD License
 
 [egg_info]
 tag_build =
```

### Comparing `tooz-3.2.0/setup.py` & `tooz-4.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tools/compat-matrix.py` & `tooz-4.0.0/tools/compat-matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 print_methods(grouping_methods)
 
 print_header("Driver support", delim="-")
 print("")
 grouping_table = [
     [
         "Yes",  # Consul
-        "No",  # Etcd
+        "Yes",  # Etcd
         "Yes",  # File
         "No",  # IPC
         "Yes",  # Memcached
         "No",  # MySQL
         "No",  # PostgreSQL
         "Yes",  # Redis
         "Yes",  # Zake
```

### Comparing `tooz-3.2.0/tooz/__init__.py` & `tooz-4.0.0/tooz/__init__.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/_retry.py` & `tooz-4.0.0/tooz/_retry.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/coordination.py` & `tooz-4.0.0/tooz/coordination.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/drivers/consul.py` & `tooz-4.0.0/tooz/drivers/consul.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/drivers/etcd.py` & `tooz-4.0.0/tooz/drivers/etcd.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/drivers/etcd3.py` & `tooz-4.0.0/tooz/drivers/etcd3.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/drivers/etcd3gw.py` & `tooz-4.0.0/tooz/drivers/etcd3gw.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/drivers/file.py` & `tooz-4.0.0/tooz/drivers/file.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/drivers/ipc.py` & `tooz-4.0.0/tooz/drivers/ipc.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/drivers/memcached.py` & `tooz-4.0.0/tooz/drivers/memcached.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/drivers/mysql.py` & `tooz-4.0.0/tooz/drivers/mysql.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,19 +54,24 @@
             #
             # So, we track locally the lock status with self.acquired
             if self.acquired is True:
                 if blocking:
                     raise _retry.TryAgain
                 return False
 
+            _, timeout = utils.convert_blocking(blocking)
             try:
                 if not self._conn.open:
                     self._conn.connect()
                 cur = self._conn.cursor()
-                cur.execute("SELECT GET_LOCK(%s, 0);", self.name)
+                cur.execute(
+                    ("SELECT GET_LOCK(%s, "
+                     f"{timeout if timeout is not None else '0'});"),
+                    self.name
+                )
                 # Can return NULL on error
                 if cur.fetchone()[0] == 1:
                     self.acquired = True
                     return True
             except pymysql.MySQLError as e:
                 utils.raise_with_cause(
                     tooz.ToozError,
```

### Comparing `tooz-3.2.0/tooz/drivers/pgsql.py` & `tooz-4.0.0/tooz/drivers/pgsql.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/drivers/redis.py` & `tooz-4.0.0/tooz/drivers/redis.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/drivers/zake.py` & `tooz-4.0.0/tooz/drivers/zake.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/drivers/zookeeper.py` & `tooz-4.0.0/tooz/drivers/zookeeper.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,19 +91,25 @@
       zookeeper://[USERNAME:PASSWORD@][HOST[:PORT]][?OPTION1=VALUE1[&OPTION2=VALUE2[&...]]]
 
     Currently the following options will be proxied to the contained client:
 
     ================  ===============================  ====================
     Name              Source                           Default
     ================  ===============================  ====================
-    hosts             url netloc + 'hosts' option key  localhost:2181
-    timeout           'timeout' options key            10.0 (kazoo default)
+    ca                'ca' options key                 None
+    certfile          'certfile' options key           None
     connection_retry  'connection_retry' options key   None
     command_retry     'command_retry' options key      None
+    hosts             url netloc + 'hosts' option key  localhost:2181
+    keyfile           'keyfile' options key            None
+    keyfile_password  'keyfile_password' options key   None
     randomize_hosts   'randomize_hosts' options key    True
+    timeout           'timeout' options key            10.0 (kazoo default)
+    use_ssl           'use_ssl' options key            False
+    verify_certs      'verify_certs' options key       True
     ================  ===============================  ====================
 
     .. _kazoo: http://kazoo.readthedocs.org/
     .. _zookeeper: http://zookeeper.apache.org/
     .. _msgpack: http://msgpack.org/
     """
     #: Default namespace when none is provided.
@@ -468,21 +474,27 @@
 
         maybe_hosts = [parsed_url.netloc] + list(options.get('hosts', []))
         hosts = list(filter(None, maybe_hosts))
         if not hosts:
             hosts = ['localhost:2181']
         randomize_hosts = options.get('randomize_hosts', True)
         client_kwargs = {
-            'hosts': ",".join(hosts),
-            'timeout': float(options.get('timeout', self.timeout)),
+            'auth_data': auth_data,
+            'ca': options.get('ca', None),
+            'certfile': options.get('certfile', None),
             'connection_retry': options.get('connection_retry'),
             'command_retry': options.get('command_retry'),
-            'randomize_hosts': strutils.bool_from_string(randomize_hosts),
-            'auth_data': auth_data,
             'default_acl': default_acl,
+            'hosts': ",".join(hosts),
+            'keyfile': options.get('keyfile', None),
+            'keyfile_password': options.get('keyfile_password', None),
+            'randomize_hosts': strutils.bool_from_string(randomize_hosts),
+            'timeout': float(options.get('timeout', self.timeout)),
+            'use_ssl': bool(options.get('use_ssl', False)),
+            'verify_certs': bool(options.get('verify_certs', True)),
         }
         handler_kind = options.get('handler')
         if handler_kind:
             try:
                 handler_cls = self.HANDLERS[handler_kind]
             except KeyError:
                 raise ValueError("Unknown handler '%s' requested"
```

### Comparing `tooz-3.2.0/tooz/hashring.py` & `tooz-4.0.0/tooz/hashring.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/locking.py` & `tooz-4.0.0/tooz/locking.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/partitioner.py` & `tooz-4.0.0/tooz/partitioner.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/tests/__init__.py` & `tooz-4.0.0/tooz/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/tests/drivers/test_etcd3.py` & `tooz-4.0.0/tooz/tests/drivers/test_etcd3.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/tests/drivers/test_etcd3gw.py` & `tooz-4.0.0/tooz/tests/drivers/test_etcd3gw.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/tests/drivers/test_file.py` & `tooz-4.0.0/tooz/tests/drivers/test_file.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/tests/test_coordination.py` & `tooz-4.0.0/tooz/tests/test_coordination.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/tests/test_etcd.py` & `tooz-4.0.0/tooz/tests/test_etcd.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/tests/test_hashring.py` & `tooz-4.0.0/tooz/tests/test_hashring.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/tests/test_memcache.py` & `tooz-4.0.0/tooz/tests/test_memcache.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/tests/test_mysql.py` & `tooz-4.0.0/tooz/tests/test_mysql.py`

 * *Files 15% similar despite different names*

```diff
@@ -81,7 +81,20 @@
                 verify_mode="yes",
                 cert="/cert/not/there",
                 key="/key/not/there",
                 cipher="spam,ham"
             )
 
         )
+
+    @mock.patch("pymysql.Connect")
+    def test_parsing_timeout_settings(self, sql_mock):
+        c = self._create_coordinator("mysql://localhost:3306/test")
+        c.start()
+
+        name = tests.get_random_uuid()
+        blocking_value = 10.12
+        lock = c.get_lock(name)
+        with mock.patch.object(lock, 'acquire', wraps=True, autospec=True) as \
+                mock_acquire:
+            with lock(blocking_value):
+                mock_acquire.assert_called_once_with(blocking_value)
```

### Comparing `tooz-3.2.0/tooz/tests/test_partitioner.py` & `tooz-4.0.0/tooz/tests/test_partitioner.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/tests/test_postgresql.py` & `tooz-4.0.0/tooz/tests/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/tests/test_utils.py` & `tooz-4.0.0/tooz/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz/utils.py` & `tooz-4.0.0/tooz/utils.py`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz.egg-info/PKG-INFO` & `tooz-4.0.0/tooz.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tooz
-Version: 3.2.0
+Version: 4.0.0
 Summary: Coordination library for distributed systems.
 Home-page: https://docs.openstack.org/tooz/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: Tooz
         ====
@@ -37,20 +37,20 @@
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: System :: Distributed Computing
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Provides-Extra: consul
 Provides-Extra: etcd
 Provides-Extra: etcd3
 Provides-Extra: etcd3gw
 Provides-Extra: ipc
 Provides-Extra: memcached
 Provides-Extra: mysql
```

### Comparing `tooz-3.2.0/tooz.egg-info/SOURCES.txt` & `tooz-4.0.0/tooz.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 releasenotes/notes/hashring-algo-8a279397b8ff8a6a.yaml
 releasenotes/notes/join_group_create-5095ec02e20c7242.yaml
 releasenotes/notes/memcached-fix-lock-release-I6fc33b8e0a88510.yaml
 releasenotes/notes/mysql-0.10.0-7660f75a1c57a920.yaml
 releasenotes/notes/mysql-tls-support-88941e2ebaf938b4.yaml
 releasenotes/notes/partitioner-4005767d287dc7c9.yaml
 releasenotes/notes/redis-connect-retries-c9adfc81eb06a4ab.yaml
+releasenotes/notes/zookeeper_tls-808355fd2ab1acae.yaml
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
```

### Comparing `tooz-3.2.0/tooz.egg-info/entry_points.txt` & `tooz-4.0.0/tooz.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `tooz-3.2.0/tooz.egg-info/requires.txt` & `tooz-4.0.0/tooz.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 stestr>=2.0.0
 testtools>=1.4.0
 
 [zake]
 zake>=0.1.6
 
 [zookeeper]
-kazoo>=2.2
+kazoo>=2.6
```

### Comparing `tooz-3.2.0/tox.ini` & `tooz-4.0.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     postgresql: TOOZ_TEST_DRIVERS = postgresql
     etcd: TOOZ_TEST_DRIVERS = etcd,etcd --cluster
     etcd3: TOOZ_TEST_DRIVERS = etcd
     etcd3: TOOZ_TEST_ETCD3 = 1
     etcd3gw: TOOZ_TEST_DRIVERS = etcd
     etcd3gw: TOOZ_TEST_ETCD3GW = 1
     consul: TOOZ_TEST_DRIVERS = consul
+allowlist_externals =
+    {toxinidir}/run-tests.sh
+    {toxinidir}/run-examples.sh
 # NOTE(tonyb): This project has chosen to *NOT* consume upper-constraints.txt
 commands =
     {toxinidir}/run-tests.sh stestr run "{posargs}"
     {toxinidir}/run-examples.sh
 
 [testenv:venv]
 # This target is used by the gate go run Sphinx to build the doc
@@ -51,14 +54,16 @@
     {toxinidir}/run-tests.sh stestr run "{posargs}"
     {toxinidir}/run-examples.sh
     coverage combine
     coverage html -d cover
     coverage xml -o cover/coverage.xml
 
 [testenv:docs]
+setenv = {[testenv]setenv}
+    PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION=python
 deps = -r{toxinidir}/doc/requirements.txt
 commands = sphinx-build -W -b html doc/source doc/build/html
 
 [testenv:pep8]
 deps = hacking>=4.0.0,<4.1.0
       doc8
       pre-commit>=2.6.0
```

