# Comparing `tmp/pmbootstrap-1.8.3.tar.gz` & `tmp/pmbootstrap-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pmbootstrap-1.8.3.tar", last modified: Sun Sep 29 22:40:00 2019, max compression
+gzip compressed data, was "dist/pmbootstrap-1.9.0.tar", last modified: Mon Oct  7 21:01:03 2019, max compression
```

## Comparing `pmbootstrap-1.8.3.tar` & `pmbootstrap-1.9.0.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/
--rwxrwxr-x   0 user      (1000) user      (1000)     2077 2018-10-12 07:16:05.000000 pmbootstrap-1.8.3/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmbootstrap.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3556 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmbootstrap.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)       26 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmbootstrap.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmbootstrap.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       42 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmbootstrap.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmbootstrap.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)     7261 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmbootstrap.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     4930 2019-07-05 19:13:40.000000 pmbootstrap-1.8.3/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/test/
--rw-rw-r--   0 user      (1000) user      (1000)     2127 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_cross_compile_distcc.py
--rw-rw-r--   0 user      (1000) user      (1000)     2963 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_config_user.py
--rw-rw-r--   0 user      (1000) user      (1000)     1128 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_version_validate.py
--rw-rw-r--   0 user      (1000) user      (1000)     6643 2019-09-18 20:07:36.000000 pmbootstrap-1.8.3/test/test_aportgen_device_wizard.py
--rw-rw-r--   0 user      (1000) user      (1000)     6276 2019-03-03 09:44:00.000000 pmbootstrap-1.8.3/test/test_helpers_package.py
--rw-rw-r--   0 user      (1000) user      (1000)     2771 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_bootimg.py
--rw-rw-r--   0 user      (1000) user      (1000)     5495 2019-03-03 09:44:00.000000 pmbootstrap-1.8.3/test/test_helpers_repo_missing.py
--rw-rw-r--   0 user      (1000) user      (1000)     2483 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_chroot_interactive_shell.py
--rw-rw-r--   0 user      (1000) user      (1000)    11921 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_parse_apkindex.py
--rw-rw-r--   0 user      (1000) user      (1000)     1578 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_repo.py
--rw-rw-r--   0 user      (1000) user      (1000)    15171 2019-09-18 20:07:36.000000 pmbootstrap-1.8.3/test/test_build_package.py
--rw-rw-r--   0 user      (1000) user      (1000)     1236 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_frontend.py
--rw-rw-r--   0 user      (1000) user      (1000)     6723 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_pkgrel_bump.py
--rw-rw-r--   0 user      (1000) user      (1000)     1622 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_file.py
--rw-rw-r--   0 user      (1000) user      (1000)     2968 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_keys.py
--rw-rw-r--   0 user      (1000) user      (1000)     5330 2019-07-05 19:13:40.000000 pmbootstrap-1.8.3/test/test_run_core.py
--rw-rw-r--   0 user      (1000) user      (1000)     9736 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_questions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2633 2019-07-05 19:13:40.000000 pmbootstrap-1.8.3/test/test_parse_apkbuild.py
--rw-rw-r--   0 user      (1000) user      (1000)     2542 2019-07-05 19:13:40.000000 pmbootstrap-1.8.3/test/test_newapkbuild.py
--rw-rw-r--   0 user      (1000) user      (1000)     1865 2019-01-22 07:57:30.000000 pmbootstrap-1.8.3/test/test_folder_size.py
--rw-rw-r--   0 user      (1000) user      (1000)     5459 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_parse_depends.py
--rw-rw-r--   0 user      (1000) user      (1000)     6844 2019-07-05 19:13:40.000000 pmbootstrap-1.8.3/test/test_qemu_running_processes.py
--rw-rw-r--   0 user      (1000) user      (1000)     2103 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_install.py
--rw-rw-r--   0 user      (1000) user      (1000)     4830 2019-09-16 20:00:48.000000 pmbootstrap-1.8.3/test/test_aportgen.py
--rw-rw-r--   0 user      (1000) user      (1000)     2700 2019-07-05 19:13:40.000000 pmbootstrap-1.8.3/test/test_version.py
--rw-rw-r--   0 user      (1000) user      (1000)     1644 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_helpers_pmaports.py
--rw-rw-r--   0 user      (1000) user      (1000)     1658 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_mount.py
--rw-rw-r--   0 user      (1000) user      (1000)     3352 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_build_is_necessary.py
--rw-rw-r--   0 user      (1000) user      (1000)     5488 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_apk_static.py
--rw-rw-r--   0 user      (1000) user      (1000)     5923 2019-02-15 15:54:55.000000 pmbootstrap-1.8.3/test/test_envkernel.py
--rw-rw-r--   0 user      (1000) user      (1000)     4104 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/test/test_shell_escape.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmb/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmb/chroot/
--rw-rw-r--   0 user      (1000) user      (1000)     3774 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/chroot/shutdown.py
--rw-rw-r--   0 user      (1000) user      (1000)      964 2019-04-24 14:07:00.000000 pmbootstrap-1.8.3/pmb/chroot/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2212 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/chroot/binfmt.py
--rw-rw-r--   0 user      (1000) user      (1000)     3503 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/chroot/other.py
--rw-rw-r--   0 user      (1000) user      (1000)     4218 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/chroot/init.py
--rw-rw-r--   0 user      (1000) user      (1000)     3334 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/chroot/root.py
--rw-rw-r--   0 user      (1000) user      (1000)     4870 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/chroot/initfs.py
--rw-rw-r--   0 user      (1000) user      (1000)     1968 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/chroot/user.py
--rw-rw-r--   0 user      (1000) user      (1000)    10337 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/chroot/apk.py
--rw-rw-r--   0 user      (1000) user      (1000)     6260 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/chroot/zap.py
--rw-rw-r--   0 user      (1000) user      (1000)     2385 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/chroot/initfs_hooks.py
--rw-rw-r--   0 user      (1000) user      (1000)     4581 2019-05-19 17:55:07.000000 pmbootstrap-1.8.3/pmb/chroot/mount.py
--rw-rw-r--   0 user      (1000) user      (1000)     9424 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/chroot/distccd.py
--rw-rw-r--   0 user      (1000) user      (1000)     6789 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/chroot/apk_static.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmb/config/
--rw-rw-r--   0 user      (1000) user      (1000)    14567 2019-09-29 22:39:59.000000 pmbootstrap-1.8.3/pmb/config/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    15606 2019-09-16 20:00:48.000000 pmbootstrap-1.8.3/pmb/config/init.py
--rw-rw-r--   0 user      (1000) user      (1000)      906 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/config/save.py
--rw-rw-r--   0 user      (1000) user      (1000)     1767 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/config/load.py
--rw-rw-r--   0 user      (1000) user      (1000)     2005 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/config/merge_with_args.py
--rw-rw-r--   0 user      (1000) user      (1000)     5143 2019-07-05 19:13:40.000000 pmbootstrap-1.8.3/pmb/config/pmaports.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmb/data/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmb/data/keys/
--rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.8.3/pmb/data/keys/alpine-devel@lists.alpinelinux.org-4a6a0840.rsa.pub
--rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.8.3/pmb/data/keys/alpine-devel@lists.alpinelinux.org-58cbb476.rsa.pub
--rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.8.3/pmb/data/keys/alpine-devel@lists.alpinelinux.org-5243ef4b.rsa.pub
--rw-rw-r--   0 user      (1000) user      (1000)      499 2018-10-09 04:56:02.000000 pmbootstrap-1.8.3/pmb/data/keys/README
--rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.8.3/pmb/data/keys/alpine-devel@lists.alpinelinux.org-5261cecb.rsa.pub
--rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.8.3/pmb/data/keys/pmos-5a03a13a.rsa.pub
--rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.8.3/pmb/data/keys/alpine-devel@lists.alpinelinux.org-58199dcc.rsa.pub
--rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.8.3/pmb/data/keys/alpine-devel@lists.alpinelinux.org-58e4f17d.rsa.pub
--rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.8.3/pmb/data/keys/alpine-devel@lists.alpinelinux.org-524d27bb.rsa.pub
--rw-rw-r--   0 user      (1000) user      (1000)     5932 2018-10-09 04:56:02.000000 pmbootstrap-1.8.3/pmb/data/qemu-user-binfmt.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmb/flasher/
--rw-rw-r--   0 user      (1000) user      (1000)      887 2019-03-03 09:44:00.000000 pmbootstrap-1.8.3/pmb/flasher/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2016 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/flasher/init.py
--rw-rw-r--   0 user      (1000) user      (1000)     2701 2019-09-26 21:12:43.000000 pmbootstrap-1.8.3/pmb/flasher/run.py
--rw-rw-r--   0 user      (1000) user      (1000)     4766 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/flasher/frontend.py
--rw-rw-r--   0 user      (1000) user      (1000)     2249 2019-09-26 21:12:43.000000 pmbootstrap-1.8.3/pmb/flasher/variables.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmb/export/
--rw-rw-r--   0 user      (1000) user      (1000)      796 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/export/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2909 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/export/symlinks.py
--rw-rw-r--   0 user      (1000) user      (1000)     4758 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/export/odin.py
--rw-rw-r--   0 user      (1000) user      (1000)     1017 2018-10-09 04:56:02.000000 pmbootstrap-1.8.3/pmb/export/frontend.py
--rw-rw-r--   0 user      (1000) user      (1000)     3248 2019-02-15 15:54:55.000000 pmbootstrap-1.8.3/pmb/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmb/parse/
--rw-rw-r--   0 user      (1000) user      (1000)     5745 2019-09-16 20:00:48.000000 pmbootstrap-1.8.3/pmb/parse/kconfig.py
--rw-rw-r--   0 user      (1000) user      (1000)     9845 2019-07-05 19:13:40.000000 pmbootstrap-1.8.3/pmb/parse/version.py
--rw-rw-r--   0 user      (1000) user      (1000)      996 2019-02-15 15:54:55.000000 pmbootstrap-1.8.3/pmb/parse/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3833 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/parse/bootimg.py
--rw-rw-r--   0 user      (1000) user      (1000)     3976 2019-09-26 21:12:43.000000 pmbootstrap-1.8.3/pmb/parse/deviceinfo.py
--rw-rw-r--   0 user      (1000) user      (1000)     1639 2019-07-05 19:13:40.000000 pmbootstrap-1.8.3/pmb/parse/binfmt_info.py
--rw-rw-r--   0 user      (1000) user      (1000)     5336 2019-09-18 20:07:36.000000 pmbootstrap-1.8.3/pmb/parse/arch.py
--rw-rw-r--   0 user      (1000) user      (1000)    28173 2019-09-18 20:07:36.000000 pmbootstrap-1.8.3/pmb/parse/arguments.py
--rw-rw-r--   0 user      (1000) user      (1000)     6245 2019-04-24 14:07:00.000000 pmbootstrap-1.8.3/pmb/parse/depends.py
--rw-rw-r--   0 user      (1000) user      (1000)    14350 2019-04-24 14:07:00.000000 pmbootstrap-1.8.3/pmb/parse/apkindex.py
--rw-rw-r--   0 user      (1000) user      (1000)    10159 2019-07-05 19:13:40.000000 pmbootstrap-1.8.3/pmb/parse/_apkbuild.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmb/qemu/
--rw-rw-r--   0 user      (1000) user      (1000)      714 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/qemu/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    12179 2019-07-05 19:13:40.000000 pmbootstrap-1.8.3/pmb/qemu/run.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmb/aportgen/
--rw-rw-r--   0 user      (1000) user      (1000)     3798 2019-09-16 20:00:48.000000 pmbootstrap-1.8.3/pmb/aportgen/gcc.py
--rw-rw-r--   0 user      (1000) user      (1000)     2517 2019-09-16 20:00:48.000000 pmbootstrap-1.8.3/pmb/aportgen/binutils.py
--rw-rw-r--   0 user      (1000) user      (1000)     3493 2019-04-24 14:07:00.000000 pmbootstrap-1.8.3/pmb/aportgen/grub_efi.py
--rw-rw-r--   0 user      (1000) user      (1000)     3174 2019-09-16 20:00:48.000000 pmbootstrap-1.8.3/pmb/aportgen/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3790 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/aportgen/busybox_static.py
--rw-rw-r--   0 user      (1000) user      (1000)     9632 2019-03-03 09:44:00.000000 pmbootstrap-1.8.3/pmb/aportgen/device.py
--rw-rw-r--   0 user      (1000) user      (1000)     5355 2019-03-10 01:44:16.000000 pmbootstrap-1.8.3/pmb/aportgen/musl.py
--rw-rw-r--   0 user      (1000) user      (1000)     7707 2019-09-16 20:00:48.000000 pmbootstrap-1.8.3/pmb/aportgen/core.py
--rw-rw-r--   0 user      (1000) user      (1000)     4737 2019-01-22 07:57:30.000000 pmbootstrap-1.8.3/pmb/aportgen/linux.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmb/helpers/
--rw-rw-r--   0 user      (1000) user      (1000)     2615 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/helpers/file.py
--rw-rw-r--   0 user      (1000) user      (1000)     7592 2019-04-24 14:07:00.000000 pmbootstrap-1.8.3/pmb/helpers/package.py
--rw-rw-r--   0 user      (1000) user      (1000)      681 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/helpers/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     6673 2019-04-24 14:07:00.000000 pmbootstrap-1.8.3/pmb/helpers/other.py
--rw-rw-r--   0 user      (1000) user      (1000)     6341 2019-03-03 09:44:00.000000 pmbootstrap-1.8.3/pmb/helpers/repo_missing.py
--rw-rw-r--   0 user      (1000) user      (1000)     2663 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/helpers/http.py
--rw-rw-r--   0 user      (1000) user      (1000)     1211 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/helpers/ui.py
--rw-rw-r--   0 user      (1000) user      (1000)     3122 2019-05-19 17:55:07.000000 pmbootstrap-1.8.3/pmb/helpers/git.py
--rw-rw-r--   0 user      (1000) user      (1000)     3768 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/helpers/logging.py
--rw-rw-r--   0 user      (1000) user      (1000)     3886 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/helpers/mount.py
--rw-rw-r--   0 user      (1000) user      (1000)     7388 2019-03-03 09:44:00.000000 pmbootstrap-1.8.3/pmb/helpers/repo.py
--rw-rw-r--   0 user      (1000) user      (1000)     3171 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/helpers/run.py
--rw-rw-r--   0 user      (1000) user      (1000)    12449 2019-09-16 20:00:48.000000 pmbootstrap-1.8.3/pmb/helpers/frontend.py
--rw-rw-r--   0 user      (1000) user      (1000)     2329 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/helpers/cli.py
--rw-rw-r--   0 user      (1000) user      (1000)     7915 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/helpers/args.py
--rw-rw-r--   0 user      (1000) user      (1000)     6376 2019-04-24 14:07:00.000000 pmbootstrap-1.8.3/pmb/helpers/pmaports.py
--rw-rw-r--   0 user      (1000) user      (1000)     6502 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/helpers/pkgrel_bump.py
--rw-rw-r--   0 user      (1000) user      (1000)    12983 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/helpers/run_core.py
--rw-rw-r--   0 user      (1000) user      (1000)     1608 2019-01-10 21:07:28.000000 pmbootstrap-1.8.3/pmb/helpers/devices.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmb/build/
--rw-rw-r--   0 user      (1000) user      (1000)      988 2019-09-18 20:07:36.000000 pmbootstrap-1.8.3/pmb/build/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3078 2019-04-24 14:07:00.000000 pmbootstrap-1.8.3/pmb/build/autodetect.py
--rw-rw-r--   0 user      (1000) user      (1000)     6637 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/build/other.py
--rw-rw-r--   0 user      (1000) user      (1000)     3712 2019-09-18 20:07:36.000000 pmbootstrap-1.8.3/pmb/build/init.py
--rw-rw-r--   0 user      (1000) user      (1000)    19436 2019-04-24 14:07:00.000000 pmbootstrap-1.8.3/pmb/build/_package.py
--rw-rw-r--   0 user      (1000) user      (1000)     7499 2019-05-19 17:55:07.000000 pmbootstrap-1.8.3/pmb/build/envkernel.py
--rw-rw-r--   0 user      (1000) user      (1000)     2495 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/build/newapkbuild.py
--rw-rw-r--   0 user      (1000) user      (1000)     5956 2019-07-05 19:13:40.000000 pmbootstrap-1.8.3/pmb/build/menuconfig.py
--rw-rw-r--   0 user      (1000) user      (1000)     1788 2019-07-05 19:13:40.000000 pmbootstrap-1.8.3/pmb/build/checksum.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/pmb/install/
--rw-rw-r--   0 user      (1000) user      (1000)     1864 2019-05-19 17:55:07.000000 pmbootstrap-1.8.3/pmb/install/file.py
--rw-rw-r--   0 user      (1000) user      (1000)     2919 2019-03-03 09:44:00.000000 pmbootstrap-1.8.3/pmb/install/recovery.py
--rw-rw-r--   0 user      (1000) user      (1000)      907 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/install/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3300 2019-01-22 07:57:30.000000 pmbootstrap-1.8.3/pmb/install/format.py
--rw-rw-r--   0 user      (1000) user      (1000)     2988 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/install/losetup.py
--rw-rw-r--   0 user      (1000) user      (1000)    20572 2019-09-16 20:00:48.000000 pmbootstrap-1.8.3/pmb/install/_install.py
--rw-rw-r--   0 user      (1000) user      (1000)     5990 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/install/blockdevice.py
--rw-rw-r--   0 user      (1000) user      (1000)     3014 2019-01-03 07:47:42.000000 pmbootstrap-1.8.3/pmb/install/partition.py
--rw-rw-r--   0 user      (1000) user      (1000)    35141 2018-10-09 04:56:02.000000 pmbootstrap-1.8.3/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       67 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)       45 2018-10-09 04:56:02.000000 pmbootstrap-1.8.3/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     7261 2019-09-29 22:40:00.000000 pmbootstrap-1.8.3/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/
+-rwxrwxr-x   0 user      (1000) user      (1000)     2077 2018-10-12 07:16:05.000000 pmbootstrap-1.9.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmbootstrap.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3556 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmbootstrap.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       26 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmbootstrap.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmbootstrap.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       42 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmbootstrap.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmbootstrap.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     7261 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmbootstrap.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     4930 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/test/
+-rw-rw-r--   0 user      (1000) user      (1000)     2127 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_cross_compile_distcc.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2963 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_config_user.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1128 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_version_validate.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6643 2019-09-18 20:07:36.000000 pmbootstrap-1.9.0/test/test_aportgen_device_wizard.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5324 2019-10-07 21:01:02.000000 pmbootstrap-1.9.0/test/test_helpers_package.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2771 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_bootimg.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5481 2019-10-07 21:01:02.000000 pmbootstrap-1.9.0/test/test_helpers_repo_missing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2483 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_chroot_interactive_shell.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11921 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_parse_apkindex.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1578 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_repo.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15171 2019-09-18 20:07:36.000000 pmbootstrap-1.9.0/test/test_build_package.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1236 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_frontend.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6723 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_pkgrel_bump.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1622 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_file.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2968 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_keys.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5330 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/test/test_run_core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9736 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_questions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2633 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/test/test_parse_apkbuild.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2542 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/test/test_newapkbuild.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1865 2019-01-22 07:57:30.000000 pmbootstrap-1.9.0/test/test_folder_size.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5459 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_parse_depends.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6844 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/test/test_qemu_running_processes.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2103 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_install.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4830 2019-09-16 20:00:48.000000 pmbootstrap-1.9.0/test/test_aportgen.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2700 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/test/test_version.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1644 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_helpers_pmaports.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1658 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_mount.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3352 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_build_is_necessary.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5488 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_apk_static.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5923 2019-02-15 15:54:55.000000 pmbootstrap-1.9.0/test/test_envkernel.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4104 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_shell_escape.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/chroot/
+-rw-rw-r--   0 user      (1000) user      (1000)     3774 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/shutdown.py
+-rw-rw-r--   0 user      (1000) user      (1000)      964 2019-04-24 14:07:00.000000 pmbootstrap-1.9.0/pmb/chroot/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2212 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/binfmt.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3503 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/other.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4218 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/init.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3334 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/root.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4870 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/initfs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1968 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/user.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10337 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/apk.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6260 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/zap.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2385 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/initfs_hooks.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4581 2019-05-19 17:55:07.000000 pmbootstrap-1.9.0/pmb/chroot/mount.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9424 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/distccd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6789 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/apk_static.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/config/
+-rw-rw-r--   0 user      (1000) user      (1000)    14567 2019-10-07 21:01:02.000000 pmbootstrap-1.9.0/pmb/config/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15606 2019-09-16 20:00:48.000000 pmbootstrap-1.9.0/pmb/config/init.py
+-rw-rw-r--   0 user      (1000) user      (1000)      906 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/config/save.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1767 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/config/load.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2005 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/config/merge_with_args.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5143 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/pmb/config/pmaports.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/data/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/data/keys/
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-4a6a0840.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-58cbb476.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-5243ef4b.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      499 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/README
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-5261cecb.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/pmos-5a03a13a.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-58199dcc.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-58e4f17d.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-524d27bb.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)     5932 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/qemu-user-binfmt.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/flasher/
+-rw-rw-r--   0 user      (1000) user      (1000)      887 2019-03-03 09:44:00.000000 pmbootstrap-1.9.0/pmb/flasher/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2016 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/flasher/init.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2701 2019-09-26 21:12:43.000000 pmbootstrap-1.9.0/pmb/flasher/run.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4766 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/flasher/frontend.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2249 2019-09-26 21:12:43.000000 pmbootstrap-1.9.0/pmb/flasher/variables.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/export/
+-rw-rw-r--   0 user      (1000) user      (1000)      796 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/export/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2909 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/export/symlinks.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4758 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/export/odin.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1017 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/export/frontend.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3248 2019-02-15 15:54:55.000000 pmbootstrap-1.9.0/pmb/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/parse/
+-rw-rw-r--   0 user      (1000) user      (1000)     5745 2019-09-16 20:00:48.000000 pmbootstrap-1.9.0/pmb/parse/kconfig.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9845 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/pmb/parse/version.py
+-rw-rw-r--   0 user      (1000) user      (1000)      996 2019-02-15 15:54:55.000000 pmbootstrap-1.9.0/pmb/parse/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3833 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/parse/bootimg.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3976 2019-09-26 21:12:43.000000 pmbootstrap-1.9.0/pmb/parse/deviceinfo.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1639 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/pmb/parse/binfmt_info.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5336 2019-09-18 20:07:36.000000 pmbootstrap-1.9.0/pmb/parse/arch.py
+-rw-rw-r--   0 user      (1000) user      (1000)    28173 2019-09-18 20:07:36.000000 pmbootstrap-1.9.0/pmb/parse/arguments.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6245 2019-04-24 14:07:00.000000 pmbootstrap-1.9.0/pmb/parse/depends.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14350 2019-04-24 14:07:00.000000 pmbootstrap-1.9.0/pmb/parse/apkindex.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10159 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/pmb/parse/_apkbuild.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/qemu/
+-rw-rw-r--   0 user      (1000) user      (1000)      714 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/qemu/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12179 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/pmb/qemu/run.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/aportgen/
+-rw-rw-r--   0 user      (1000) user      (1000)     3798 2019-09-16 20:00:48.000000 pmbootstrap-1.9.0/pmb/aportgen/gcc.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2517 2019-09-16 20:00:48.000000 pmbootstrap-1.9.0/pmb/aportgen/binutils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3493 2019-04-24 14:07:00.000000 pmbootstrap-1.9.0/pmb/aportgen/grub_efi.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3233 2019-10-07 21:01:02.000000 pmbootstrap-1.9.0/pmb/aportgen/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3790 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/aportgen/busybox_static.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9632 2019-03-03 09:44:00.000000 pmbootstrap-1.9.0/pmb/aportgen/device.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5355 2019-03-10 01:44:16.000000 pmbootstrap-1.9.0/pmb/aportgen/musl.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7707 2019-09-16 20:00:48.000000 pmbootstrap-1.9.0/pmb/aportgen/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4737 2019-01-22 07:57:30.000000 pmbootstrap-1.9.0/pmb/aportgen/linux.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/helpers/
+-rw-rw-r--   0 user      (1000) user      (1000)     2615 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/file.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6785 2019-10-07 21:01:02.000000 pmbootstrap-1.9.0/pmb/helpers/package.py
+-rw-rw-r--   0 user      (1000) user      (1000)      681 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6673 2019-04-24 14:07:00.000000 pmbootstrap-1.9.0/pmb/helpers/other.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5936 2019-10-07 21:01:02.000000 pmbootstrap-1.9.0/pmb/helpers/repo_missing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2663 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/http.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1211 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/ui.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3122 2019-05-19 17:55:07.000000 pmbootstrap-1.9.0/pmb/helpers/git.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3768 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/logging.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3886 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/mount.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7388 2019-03-03 09:44:00.000000 pmbootstrap-1.9.0/pmb/helpers/repo.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3171 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/run.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12449 2019-09-16 20:00:48.000000 pmbootstrap-1.9.0/pmb/helpers/frontend.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2329 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/cli.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7915 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/args.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6376 2019-04-24 14:07:00.000000 pmbootstrap-1.9.0/pmb/helpers/pmaports.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6502 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/pkgrel_bump.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12983 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/run_core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1608 2019-01-10 21:07:28.000000 pmbootstrap-1.9.0/pmb/helpers/devices.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/build/
+-rw-rw-r--   0 user      (1000) user      (1000)      988 2019-09-18 20:07:36.000000 pmbootstrap-1.9.0/pmb/build/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3078 2019-04-24 14:07:00.000000 pmbootstrap-1.9.0/pmb/build/autodetect.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6775 2019-10-07 21:01:02.000000 pmbootstrap-1.9.0/pmb/build/other.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3712 2019-09-18 20:07:36.000000 pmbootstrap-1.9.0/pmb/build/init.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19436 2019-04-24 14:07:00.000000 pmbootstrap-1.9.0/pmb/build/_package.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7499 2019-05-19 17:55:07.000000 pmbootstrap-1.9.0/pmb/build/envkernel.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2495 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/build/newapkbuild.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5956 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/pmb/build/menuconfig.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1788 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/pmb/build/checksum.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/install/
+-rw-rw-r--   0 user      (1000) user      (1000)     1864 2019-05-19 17:55:07.000000 pmbootstrap-1.9.0/pmb/install/file.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2919 2019-03-03 09:44:00.000000 pmbootstrap-1.9.0/pmb/install/recovery.py
+-rw-rw-r--   0 user      (1000) user      (1000)      907 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/install/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3300 2019-01-22 07:57:30.000000 pmbootstrap-1.9.0/pmb/install/format.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2988 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/install/losetup.py
+-rw-rw-r--   0 user      (1000) user      (1000)    20576 2019-10-07 21:01:02.000000 pmbootstrap-1.9.0/pmb/install/_install.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5990 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/install/blockdevice.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3014 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/install/partition.py
+-rw-rw-r--   0 user      (1000) user      (1000)    35141 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       67 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)       45 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     7261 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/PKG-INFO
```

### Comparing `pmbootstrap-1.8.3/setup.py` & `pmbootstrap-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmbootstrap.egg-info/SOURCES.txt` & `pmbootstrap-1.9.0/pmbootstrap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmbootstrap.egg-info/PKG-INFO` & `pmbootstrap-1.9.0/pmbootstrap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmbootstrap
-Version: 1.8.3
+Version: 1.9.0
 Summary: A sophisticated chroot / build / flash tool to develop and install postmarketOS
 Home-page: https://www.postmarketos.org
 Author: postmarketOS Developers
 Author-email: info@postmarketos.org
 License: GPLv3
 Description: # pmbootstrap
         [**Introduction**](https://postmarketos.org/blog/2017/05/26/intro/) | [**Security Warning**](https://ollieparanoid.github.io/post/security-warning/) | [**Devices**](https://wiki.postmarketos.org/wiki/Devices)
```

### Comparing `pmbootstrap-1.8.3/README.md` & `pmbootstrap-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_cross_compile_distcc.py` & `pmbootstrap-1.9.0/test/test_cross_compile_distcc.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_config_user.py` & `pmbootstrap-1.9.0/test/test_config_user.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_version_validate.py` & `pmbootstrap-1.9.0/test/test_version_validate.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_aportgen_device_wizard.py` & `pmbootstrap-1.9.0/test/test_aportgen_device_wizard.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_helpers_package.py` & `pmbootstrap-1.9.0/test/test_helpers_package.py`

 * *Files 12% similar despite different names*

```diff
@@ -150,36 +150,7 @@
     monkeypatch.setattr(pmb.helpers.pmaports, "get", fake_pmaports_get)
 
     fake_pmaport["arch"] = ["armhf"]
     assert func(args, "a", "armhf", False) is True
 
     fake_pmaport["arch"] = ["all", "!armhf"]
     assert func(args, "a", "armhf", False) is False
-
-
-def test_helpers_package_check_arch_recurse(args, monkeypatch):
-    """ Test pmb.helpers.package.check_arch_recurse() """
-    # Test data
-    func = pmb.helpers.package.check_arch_recurse
-    depends = ["a", "b", "c"]
-    arch_check_results = {}
-
-    def fake_depends_recurse(args, pkgname, arch):
-        return depends
-    monkeypatch.setattr(pmb.helpers.package, "depends_recurse",
-                        fake_depends_recurse)
-
-    def fake_check_arch(args, pkgname, arch):
-        return arch_check_results[pkgname]
-    monkeypatch.setattr(pmb.helpers.package, "check_arch", fake_check_arch)
-
-    # Result: True
-    arch_check_results = {"a": True,
-                          "b": True,
-                          "c": True}
-    assert func(args, "a", "armhf") is True
-
-    # Result: False
-    arch_check_results = {"a": True,
-                          "b": False,
-                          "c": True}
-    assert func(args, "a", "armhf") is False
```

### Comparing `pmbootstrap-1.8.3/test/test_bootimg.py` & `pmbootstrap-1.9.0/test/test_bootimg.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_helpers_repo_missing.py` & `pmbootstrap-1.9.0/test/test_helpers_repo_missing.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,38 +75,38 @@
 
 
 def test_filter_arch_packages(args, monkeypatch):
     """ Test ...repo_missing.filter_arch_packages() """
     func = pmb.helpers.repo_missing.filter_arch_packages
     check_arch = None
 
-    def stub(args, arch, pmaport):
+    def stub(args, arch, pmaport, binary=True):
         return check_arch
-    monkeypatch.setattr(pmb.helpers.package, "check_arch_recurse", stub)
+    monkeypatch.setattr(pmb.helpers.package, "check_arch", stub)
 
     check_arch = False
     assert func(args, "armhf", ["hello-world"]) == []
 
     check_arch = True
     assert func(args, "armhf", []) == []
 
 
 def test_get_relevant_packages(args, monkeypatch):
     """ Test ...repo_missing.get_relevant_packages() """
 
     # Set up fake return values
-    stub_data = {"check_arch_recurse": False,
+    stub_data = {"check_arch": False,
                  "depends_recurse": ["a", "b", "c", "d"],
                  "filter_arch_packages": ["a", "b", "c"],
                  "filter_aport_packages": ["b", "a"],
                  "filter_missing_packages": ["a"]}
 
-    def stub(args, arch, pmaport):
-        return stub_data["check_arch_recurse"]
-    monkeypatch.setattr(pmb.helpers.package, "check_arch_recurse", stub)
+    def stub(args, arch, pmaport, binary=True):
+        return stub_data["check_arch"]
+    monkeypatch.setattr(pmb.helpers.package, "check_arch", stub)
 
     def stub(args, arch, pmaport):
         return stub_data["depends_recurse"]
     monkeypatch.setattr(pmb.helpers.package, "depends_recurse", stub)
 
     def stub(args, arch, pmaport):
         return stub_data["filter_arch_packages"]
@@ -129,15 +129,15 @@
 
     # Package can't be built for given arch
     with pytest.raises(RuntimeError) as e:
         func(args, "armhf", "a")
     assert "can't be built" in str(e.value)
 
     # Package can be built for given arch
-    stub_data["check_arch_recurse"] = True
+    stub_data["check_arch"] = True
     assert func(args, "armhf", "a") == ["a"]
     assert func(args, "armhf", "a", True) == ["a", "b"]
 
 
 def test_generate_output_format(args, monkeypatch):
     """ Test ...repo_missing.generate_output_format() """
```

### Comparing `pmbootstrap-1.8.3/test/test_chroot_interactive_shell.py` & `pmbootstrap-1.9.0/test/test_chroot_interactive_shell.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_parse_apkindex.py` & `pmbootstrap-1.9.0/test/test_parse_apkindex.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_repo.py` & `pmbootstrap-1.9.0/test/test_repo.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_build_package.py` & `pmbootstrap-1.9.0/test/test_build_package.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_frontend.py` & `pmbootstrap-1.9.0/test/test_frontend.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_pkgrel_bump.py` & `pmbootstrap-1.9.0/test/test_pkgrel_bump.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_file.py` & `pmbootstrap-1.9.0/test/test_file.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_keys.py` & `pmbootstrap-1.9.0/test/test_keys.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_run_core.py` & `pmbootstrap-1.9.0/test/test_run_core.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_questions.py` & `pmbootstrap-1.9.0/test/test_questions.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_parse_apkbuild.py` & `pmbootstrap-1.9.0/test/test_parse_apkbuild.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_newapkbuild.py` & `pmbootstrap-1.9.0/test/test_newapkbuild.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_folder_size.py` & `pmbootstrap-1.9.0/test/test_folder_size.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_parse_depends.py` & `pmbootstrap-1.9.0/test/test_parse_depends.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_qemu_running_processes.py` & `pmbootstrap-1.9.0/test/test_qemu_running_processes.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_install.py` & `pmbootstrap-1.9.0/test/test_install.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_aportgen.py` & `pmbootstrap-1.9.0/test/test_aportgen.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_version.py` & `pmbootstrap-1.9.0/test/test_version.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_helpers_pmaports.py` & `pmbootstrap-1.9.0/test/test_helpers_pmaports.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_mount.py` & `pmbootstrap-1.9.0/test/test_mount.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_build_is_necessary.py` & `pmbootstrap-1.9.0/test/test_build_is_necessary.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_apk_static.py` & `pmbootstrap-1.9.0/test/test_apk_static.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_envkernel.py` & `pmbootstrap-1.9.0/test/test_envkernel.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/test/test_shell_escape.py` & `pmbootstrap-1.9.0/test/test_shell_escape.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/chroot/shutdown.py` & `pmbootstrap-1.9.0/pmb/chroot/shutdown.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/chroot/__init__.py` & `pmbootstrap-1.9.0/pmb/chroot/__init__.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/chroot/binfmt.py` & `pmbootstrap-1.9.0/pmb/chroot/binfmt.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/chroot/other.py` & `pmbootstrap-1.9.0/pmb/chroot/other.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/chroot/init.py` & `pmbootstrap-1.9.0/pmb/chroot/init.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/chroot/root.py` & `pmbootstrap-1.9.0/pmb/chroot/root.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/chroot/initfs.py` & `pmbootstrap-1.9.0/pmb/chroot/initfs.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/chroot/user.py` & `pmbootstrap-1.9.0/pmb/chroot/user.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/chroot/apk.py` & `pmbootstrap-1.9.0/pmb/chroot/apk.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/chroot/zap.py` & `pmbootstrap-1.9.0/pmb/chroot/zap.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/chroot/initfs_hooks.py` & `pmbootstrap-1.9.0/pmb/chroot/initfs_hooks.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/chroot/mount.py` & `pmbootstrap-1.9.0/pmb/chroot/mount.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/chroot/distccd.py` & `pmbootstrap-1.9.0/pmb/chroot/distccd.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/chroot/apk_static.py` & `pmbootstrap-1.9.0/pmb/chroot/apk_static.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/config/__init__.py` & `pmbootstrap-1.9.0/pmb/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from pmb.config.save import save
 from pmb.config.merge_with_args import merge_with_args
 
 
 #
 # Exported variables (internal configuration)
 #
-version = "1.8.3"
+version = "1.9.0"
 pmb_src = os.path.normpath(os.path.realpath(__file__) + "/../../..")
 apk_keys_path = pmb_src + "/pmb/data/keys"
 
 # Update this frequently to prevent a MITM attack with an outdated version
 # (which may contain a vulnerable apk/libressl, and allows an attacker to
 # exploit the system!)
 apk_tools_static_min_version = "2.10.4-r3"
```

### Comparing `pmbootstrap-1.8.3/pmb/config/init.py` & `pmbootstrap-1.9.0/pmb/config/init.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/config/save.py` & `pmbootstrap-1.9.0/pmb/config/save.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/config/load.py` & `pmbootstrap-1.9.0/pmb/config/load.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/config/merge_with_args.py` & `pmbootstrap-1.9.0/pmb/config/merge_with_args.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/config/pmaports.py` & `pmbootstrap-1.9.0/pmb/config/pmaports.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/data/qemu-user-binfmt.txt` & `pmbootstrap-1.9.0/pmb/data/qemu-user-binfmt.txt`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/flasher/__init__.py` & `pmbootstrap-1.9.0/pmb/flasher/__init__.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/flasher/init.py` & `pmbootstrap-1.9.0/pmb/flasher/init.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/flasher/run.py` & `pmbootstrap-1.9.0/pmb/flasher/run.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/flasher/frontend.py` & `pmbootstrap-1.9.0/pmb/flasher/frontend.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/flasher/variables.py` & `pmbootstrap-1.9.0/pmb/flasher/variables.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/export/__init__.py` & `pmbootstrap-1.9.0/pmb/export/__init__.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/export/symlinks.py` & `pmbootstrap-1.9.0/pmb/export/symlinks.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/export/odin.py` & `pmbootstrap-1.9.0/pmb/export/odin.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/export/frontend.py` & `pmbootstrap-1.9.0/pmb/export/frontend.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/__init__.py` & `pmbootstrap-1.9.0/pmb/__init__.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/parse/kconfig.py` & `pmbootstrap-1.9.0/pmb/parse/kconfig.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/parse/version.py` & `pmbootstrap-1.9.0/pmb/parse/version.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/parse/__init__.py` & `pmbootstrap-1.9.0/pmb/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/parse/bootimg.py` & `pmbootstrap-1.9.0/pmb/parse/bootimg.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/parse/deviceinfo.py` & `pmbootstrap-1.9.0/pmb/parse/deviceinfo.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/parse/binfmt_info.py` & `pmbootstrap-1.9.0/pmb/parse/binfmt_info.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/parse/arch.py` & `pmbootstrap-1.9.0/pmb/parse/arch.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/parse/arguments.py` & `pmbootstrap-1.9.0/pmb/parse/arguments.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/parse/depends.py` & `pmbootstrap-1.9.0/pmb/parse/depends.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/parse/apkindex.py` & `pmbootstrap-1.9.0/pmb/parse/apkindex.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/parse/_apkbuild.py` & `pmbootstrap-1.9.0/pmb/parse/_apkbuild.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/qemu/__init__.py` & `pmbootstrap-1.9.0/pmb/qemu/__init__.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/qemu/run.py` & `pmbootstrap-1.9.0/pmb/qemu/run.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/aportgen/gcc.py` & `pmbootstrap-1.9.0/pmb/aportgen/gcc.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/aportgen/binutils.py` & `pmbootstrap-1.9.0/pmb/aportgen/binutils.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/aportgen/grub_efi.py` & `pmbootstrap-1.9.0/pmb/aportgen/grub_efi.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/aportgen/__init__.py` & `pmbootstrap-1.9.0/pmb/aportgen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,7 +75,9 @@
         getattr(pmb.aportgen, prefix.replace("-", "_")).generate(args, pkgname)
 
     # Move to the aports folder
     if os.path.exists(path_target):
         pmb.helpers.run.user(args, ["rm", "-r", path_target])
     pmb.helpers.run.user(
         args, ["mv", args.work + "/aportgen", path_target])
+
+    logging.info("*** pmaport generated: " + path_target)
```

### Comparing `pmbootstrap-1.8.3/pmb/aportgen/busybox_static.py` & `pmbootstrap-1.9.0/pmb/aportgen/busybox_static.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/aportgen/device.py` & `pmbootstrap-1.9.0/pmb/aportgen/device.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/aportgen/musl.py` & `pmbootstrap-1.9.0/pmb/aportgen/musl.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/aportgen/core.py` & `pmbootstrap-1.9.0/pmb/aportgen/core.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/aportgen/linux.py` & `pmbootstrap-1.9.0/pmb/aportgen/linux.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/file.py` & `pmbootstrap-1.9.0/pmb/helpers/file.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/package.py` & `pmbootstrap-1.9.0/pmb/helpers/package.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 """
 Functions that work on both pmaports and (binary package) repos. See also:
 - pmb/helpers/pmaports.py (work on pmaports)
 - pmb/helpers/repo.py (work on binary package repos)
 """
 
-import logging
 import copy
 
 import pmb.helpers.pmaports
 import pmb.helpers.repo
 
 
 def get(args, pkgname, arch, replace_subpkgnames=False):
@@ -167,25 +166,7 @@
                   package, False otherwise
     """
     if binary:
         arches = get(args, pkgname, arch)["arch"]
     else:
         arches = pmb.helpers.pmaports.get(args, pkgname)["arch"]
     return pmb.helpers.pmaports.check_arches(arches, arch)
-
-
-def check_arch_recurse(args, pkgname, arch):
-    """ Recursively check if a package and its dependencies exist (binary repo)
-        or can be built (pmaports) for a certain architecture.
-        :param pkgname: name of the package
-        :param arch: architecture to check against
-        :returns: True when all the package's dependencies can be built or
-                  exist for the arch in question
-    """
-    for pkgname_i in depends_recurse(args, pkgname, arch):
-        if not check_arch(args, pkgname_i, arch):
-            if pkgname_i != pkgname:
-                logging.verbose(pkgname + ": (indirectly) depends on " +
-                                pkgname_i)
-            logging.verbose(pkgname_i + ": can't be built for " + arch)
-            return False
-    return True
```

### Comparing `pmbootstrap-1.8.3/pmb/helpers/__init__.py` & `pmbootstrap-1.9.0/pmb/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/other.py` & `pmbootstrap-1.9.0/pmb/helpers/other.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/repo_missing.py` & `pmbootstrap-1.9.0/pmb/helpers/repo_missing.py`

 * *Files 15% similar despite different names*

```diff
@@ -50,42 +50,37 @@
         if pmb.helpers.pmaports.find(args, pkgname, False):
             ret += [pkgname]
     return ret
 
 
 def filter_arch_packages(args, arch, pkgnames):
     """ Create a subset of pkgnames with packages removed that can not be
-        built for a certain arch. The check is recursive, if one of the
-        dependencies of a package can not be built for the arch in question,
-        then it will not be in the final list either.
+        built for a certain arch.
 
         :param arch: architecture (e.g. "armhf")
         :param pkgnames: list of package names (e.g. ["hello-world", "test12"])
         :returns: subset of pkgnames (e.g. ["hello-world"]) """
     ret = []
     for pkgname in pkgnames:
-        if pmb.helpers.package.check_arch_recurse(args, pkgname, arch):
+        if pmb.helpers.package.check_arch(args, pkgname, arch, False):
             ret += [pkgname]
     return ret
 
 
 def get_relevant_packages(args, arch, pkgname=None, built=False):
     """ Get all packages that can be built for the architecture in question.
 
         :param arch: architecture (e.g. "armhf")
         :param pkgname: only look at a specific package (and its dependencies)
         :param built: include packages that have already been built
         :returns: an alphabetically sorted list of pkgnames, e.g.:
                   ["devicepkg-dev", "hello-world", "osk-sdl"] """
     if pkgname:
-        if not pmb.helpers.package.check_arch_recurse(args, pkgname, arch):
-            raise RuntimeError(pkgname + " can't be built for " + arch + "."
-                               " Either itself or one if its dependencies is"
-                               " not available for that architecture. Run with"
-                               " -v for details.")
+        if not pmb.helpers.package.check_arch(args, pkgname, arch, False):
+            raise RuntimeError(pkgname + " can't be built for " + arch + ".")
         ret = pmb.helpers.package.depends_recurse(args, pkgname, arch)
     else:
         ret = pmb.helpers.pmaports.get_list(args)
         ret = filter_arch_packages(args, arch, ret)
     if built:
         ret = filter_aport_packages(args, arch, ret)
         if not len(ret):
@@ -140,16 +135,16 @@
                     "version": "1-r4"},
                    {"pkgname": "package-depending-on-hello-world",
                     "version": "0.5-r0",
                     "repo": "main"}]
     """
     # Log message
     packages_str = pkgname if pkgname else "all packages"
-    logging.info("Calculate packages that need to be built ({}, {}) - this may"
-                 " take some time".format(packages_str, arch))
+    logging.info("Calculate packages that need to be built ({}, {})"
+                 "".format(packages_str, arch))
 
     # Order relevant packages
     ret = get_relevant_packages(args, arch, pkgname, built)
 
     # Output format
     if overview:
         return ret
```

### Comparing `pmbootstrap-1.8.3/pmb/helpers/http.py` & `pmbootstrap-1.9.0/pmb/helpers/http.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/ui.py` & `pmbootstrap-1.9.0/pmb/helpers/ui.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/git.py` & `pmbootstrap-1.9.0/pmb/helpers/git.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/logging.py` & `pmbootstrap-1.9.0/pmb/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/mount.py` & `pmbootstrap-1.9.0/pmb/helpers/mount.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/repo.py` & `pmbootstrap-1.9.0/pmb/helpers/repo.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/run.py` & `pmbootstrap-1.9.0/pmb/helpers/run.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/frontend.py` & `pmbootstrap-1.9.0/pmb/helpers/frontend.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/cli.py` & `pmbootstrap-1.9.0/pmb/helpers/cli.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/args.py` & `pmbootstrap-1.9.0/pmb/helpers/args.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/pmaports.py` & `pmbootstrap-1.9.0/pmb/helpers/pmaports.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/pkgrel_bump.py` & `pmbootstrap-1.9.0/pmb/helpers/pkgrel_bump.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/run_core.py` & `pmbootstrap-1.9.0/pmb/helpers/run_core.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/helpers/devices.py` & `pmbootstrap-1.9.0/pmb/helpers/devices.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/build/__init__.py` & `pmbootstrap-1.9.0/pmb/build/__init__.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/build/autodetect.py` & `pmbootstrap-1.9.0/pmb/build/autodetect.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/build/other.py` & `pmbootstrap-1.9.0/pmb/build/other.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 You should have received a copy of the GNU General Public License
 along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
 """
 import glob
 import logging
 import os
 import shlex
+import datetime
 
 import pmb.chroot
 import pmb.helpers.file
 import pmb.helpers.git
 import pmb.helpers.pmaports
 import pmb.helpers.run
 import pmb.parse.apkindex
@@ -107,17 +108,19 @@
         paths = glob.glob(args.work + "/packages/*")
 
     for path in paths:
         if os.path.isdir(path):
             path_arch = os.path.basename(path)
             path_repo_chroot = "/home/pmos/packages/pmos/" + path_arch
             logging.debug("(native) index " + path_arch + " repository")
+            description = str(datetime.datetime.now())
             commands = [
                 # Wrap the index command with sh so we can use '*.apk'
                 ["sh", "-c", "apk -q index --output APKINDEX.tar.gz_"
+                 " --description " + shlex.quote(description) + ""
                  " --rewrite-arch " + shlex.quote(path_arch) + " *.apk"],
                 ["abuild-sign", "APKINDEX.tar.gz_"],
                 ["mv", "APKINDEX.tar.gz_", "APKINDEX.tar.gz"]
             ]
             for command in commands:
                 pmb.chroot.user(args, command, working_dir=path_repo_chroot)
         else:
```

### Comparing `pmbootstrap-1.8.3/pmb/build/init.py` & `pmbootstrap-1.9.0/pmb/build/init.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/build/_package.py` & `pmbootstrap-1.9.0/pmb/build/_package.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/build/envkernel.py` & `pmbootstrap-1.9.0/pmb/build/envkernel.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/build/newapkbuild.py` & `pmbootstrap-1.9.0/pmb/build/newapkbuild.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/build/menuconfig.py` & `pmbootstrap-1.9.0/pmb/build/menuconfig.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/build/checksum.py` & `pmbootstrap-1.9.0/pmb/build/checksum.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/install/file.py` & `pmbootstrap-1.9.0/pmb/install/file.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/install/recovery.py` & `pmbootstrap-1.9.0/pmb/install/recovery.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/install/__init__.py` & `pmbootstrap-1.9.0/pmb/install/__init__.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/install/format.py` & `pmbootstrap-1.9.0/pmb/install/format.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/install/losetup.py` & `pmbootstrap-1.9.0/pmb/install/losetup.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/install/_install.py` & `pmbootstrap-1.9.0/pmb/install/_install.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
     copy_ssh_keys(args)
     embed_firmware(args)
     pmb.chroot.shutdown(args, True)
 
     # Convert rootfs to sparse using img2simg
     if args.deviceinfo["flash_sparse"] == "true" and not args.split and not args.sdcard:
         logging.info("(native) make sparse rootfs")
-        pmb.chroot.apk.install(args, ["libsparse"])
+        pmb.chroot.apk.install(args, ["android-tools"])
         sys_image = args.device + ".img"
         sys_image_sparse = args.device + "-sparse.img"
         pmb.chroot.user(args, ["img2simg", sys_image, sys_image_sparse],
                         working_dir="/home/pmos/rootfs/")
         pmb.chroot.user(args, ["mv", "-f", sys_image_sparse, sys_image],
                         working_dir="/home/pmos/rootfs/")
```

### Comparing `pmbootstrap-1.8.3/pmb/install/blockdevice.py` & `pmbootstrap-1.9.0/pmb/install/blockdevice.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/pmb/install/partition.py` & `pmbootstrap-1.9.0/pmb/install/partition.py`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/LICENSE` & `pmbootstrap-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.8.3/PKG-INFO` & `pmbootstrap-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmbootstrap
-Version: 1.8.3
+Version: 1.9.0
 Summary: A sophisticated chroot / build / flash tool to develop and install postmarketOS
 Home-page: https://www.postmarketos.org
 Author: postmarketOS Developers
 Author-email: info@postmarketos.org
 License: GPLv3
 Description: # pmbootstrap
         [**Introduction**](https://postmarketos.org/blog/2017/05/26/intro/) | [**Security Warning**](https://ollieparanoid.github.io/post/security-warning/) | [**Devices**](https://wiki.postmarketos.org/wiki/Devices)
```

