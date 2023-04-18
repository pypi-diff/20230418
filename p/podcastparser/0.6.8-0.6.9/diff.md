# Comparing `tmp/podcastparser-0.6.8.tar.gz` & `tmp/podcastparser-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podcastparser-0.6.8.tar", last modified: Thu Sep 23 05:56:03 2021, max compression
+gzip compressed data, was "podcastparser-0.6.9.tar", last modified: Wed Dec 14 07:00:25 2022, max compression
```

## Comparing `podcastparser-0.6.8.tar` & `podcastparser-0.6.9.tar`

### file list

```diff
@@ -1,142 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 05:56:03.069217 podcastparser-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-09-23 05:55:47.000000 podcastparser-0.6.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)      908 2021-09-23 05:55:47.000000 podcastparser-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      193 2021-09-23 05:55:47.000000 podcastparser-0.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2021-09-23 05:56:03.069217 podcastparser-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      766 2021-09-23 05:55:47.000000 podcastparser-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 05:56:03.049217 podcastparser-0.6.8/doc/
--rw-r--r--   0 runner    (1001) docker     (121)     5592 2021-09-23 05:55:47.000000 podcastparser-0.6.8/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 05:56:03.049217 podcastparser-0.6.8/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 05:55:47.000000 podcastparser-0.6.8/doc/_static/.empty
--rw-r--r--   0 runner    (1001) docker     (121)     7883 2021-09-23 05:55:47.000000 podcastparser-0.6.8/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     9304 2021-09-23 05:55:47.000000 podcastparser-0.6.8/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      486 2021-09-23 05:55:47.000000 podcastparser-0.6.8/makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 05:56:03.049217 podcastparser-0.6.8/podcastparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2021-09-23 05:56:03.000000 podcastparser-0.6.8/podcastparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4115 2021-09-23 05:56:03.000000 podcastparser-0.6.8/podcastparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-23 05:56:03.000000 podcastparser-0.6.8/podcastparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-09-23 05:56:03.000000 podcastparser-0.6.8/podcastparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    33710 2021-09-23 05:55:47.000000 podcastparser-0.6.8/podcastparser.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-09-23 05:55:47.000000 podcastparser-0.6.8/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-09-23 05:56:03.069217 podcastparser-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      997 2021-09-23 05:55:47.000000 podcastparser-0.6.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2475 2021-09-23 05:55:47.000000 podcastparser-0.6.8/test_podcastparser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 05:56:03.045217 podcastparser-0.6.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 05:56:03.069217 podcastparser-0.6.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)      451 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/atom_content_encoded.json
--rw-r--r--   0 runner    (1001) docker     (121)      693 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/atom_content_encoded.rss
--rw-r--r--   0 runner    (1001) docker     (121)      393 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/atom_published_updated.json
--rw-r--r--   0 runner    (1001) docker     (121)      618 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/atom_published_updated.rss
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/atom_relative_cover.json
--rw-r--r--   0 runner    (1001) docker     (121)      201 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/atom_relative_cover.rss
--rw-r--r--   0 runner    (1001) docker     (121)      393 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/atom_updated.json
--rw-r--r--   0 runner    (1001) docker     (121)      570 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/atom_updated.rss
--rw-r--r--   0 runner    (1001) docker     (121)      854 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/chapters.json
--rw-r--r--   0 runner    (1001) docker     (121)      815 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/chapters.rss
--rw-r--r--   0 runner    (1001) docker     (121)      356 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/duration.json
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/duration.rss
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/empty.json
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/empty.rss
--rw-r--r--   0 runner    (1001) docker     (121)      594 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/episode_itunes_author.json
--rw-r--r--   0 runner    (1001) docker     (121)      202 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/episode_itunes_author.rss
--rw-r--r--   0 runner    (1001) docker     (121)      561 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/episode_number.json
--rw-r--r--   0 runner    (1001) docker     (121)      197 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/episode_number.rss
--rw-r--r--   0 runner    (1001) docker     (121)      544 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/episode_number_invalid.json
--rw-r--r--   0 runner    (1001) docker     (121)      198 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/episode_number_invalid.rss
--rw-r--r--   0 runner    (1001) docker     (121)      570 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/episode_type.json
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/episode_type.rss
--rw-r--r--   0 runner    (1001) docker     (121)      539 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/episode_type_invalid.json
--rw-r--r--   0 runner    (1001) docker     (121)      245 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/episode_type_invalid.rss
--rw-r--r--   0 runner    (1001) docker     (121)      579 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/explicit_episode.json
--rw-r--r--   0 runner    (1001) docker     (121)      200 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/explicit_episode.rss
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/explicit_feed.json
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/explicit_feed.rss
--rw-r--r--   0 runner    (1001) docker     (121)       95 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/generator.json
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/generator.rss
--rw-r--r--   0 runner    (1001) docker     (121)      625 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/html_description.json
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/html_description.rss
--rw-r--r--   0 runner    (1001) docker     (121)      644 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/html_description_rss_both.json
--rw-r--r--   0 runner    (1001) docker     (121)      422 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/html_description_rss_both.rss
--rw-r--r--   0 runner    (1001) docker     (121)      625 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/html_in_description.json
--rw-r--r--   0 runner    (1001) docker     (121)      288 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/html_in_description.rss
--rw-r--r--   0 runner    (1001) docker     (121)      657 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/html_in_description_rss_both.json
--rw-r--r--   0 runner    (1001) docker     (121)      467 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/html_in_description_rss_both.rss
--rw-r--r--   0 runner    (1001) docker     (121)      657 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/html_in_description_rss_both_different.json
--rw-r--r--   0 runner    (1001) docker     (121)      466 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/html_in_description_rss_both_different.rss
--rw-r--r--   0 runner    (1001) docker     (121)      695 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/image_and_audio.json
--rw-r--r--   0 runner    (1001) docker     (121)      306 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/image_and_audio.rss
--rw-r--r--   0 runner    (1001) docker     (121)      158 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/image_url_on_newline.json
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/image_url_on_newline.rss
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_author.json
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_author.rss
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_duration.json
--rw-r--r--   0 runner    (1001) docker     (121)      214 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_duration.rss
--rw-r--r--   0 runner    (1001) docker     (121)      359 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_episode_image.json
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_episode_image.rss
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_no_xmlns.json
--rw-r--r--   0 runner    (1001) docker     (121)      168 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_no_xmlns.rss
--rw-r--r--   0 runner    (1001) docker     (121)      157 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_owner.json
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_owner.rss
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_owner_name_only.json
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_owner_name_only.rss
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_subtitle.json
--rw-r--r--   0 runner    (1001) docker     (121)      348 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_subtitle.rss
--rw-r--r--   0 runner    (1001) docker     (121)      875 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_type.json
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_type.rss
--rw-r--r--   0 runner    (1001) docker     (121)      853 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_type_garbage.json
--rw-r--r--   0 runner    (1001) docker     (121)      471 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_type_garbage.rss
--rw-r--r--   0 runner    (1001) docker     (121)      861 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_type_missing.json
--rw-r--r--   0 runner    (1001) docker     (121)      442 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_type_missing.rss
--rw-r--r--   0 runner    (1001) docker     (121)      873 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_type_serial.json
--rw-r--r--   0 runner    (1001) docker     (121)      472 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_type_serial.rss
--rw-r--r--   0 runner    (1001) docker     (121)      293 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_xmlns.json
--rw-r--r--   0 runner    (1001) docker     (121)      205 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/itunes_xmlns.rss
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/language.json
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/language.rss
--rw-r--r--   0 runner    (1001) docker     (121)      451 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/leading_space_url.json
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/leading_space_url.rss
--rw-r--r--   0 runner    (1001) docker     (121)      543 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/max_episodes.json
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/max_episodes.param.json
--rw-r--r--   0 runner    (1001) docker     (121)      299 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/max_episodes.rss
--rw-r--r--   0 runner    (1001) docker     (121)      362 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/media_episode_thumbnail.json
--rw-r--r--   0 runner    (1001) docker     (121)      227 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/media_episode_thumbnail.rss
--rw-r--r--   0 runner    (1001) docker     (121)      330 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/media_episode_thumbnail_atom.json
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/media_episode_thumbnail_atom.rss
--rw-r--r--   0 runner    (1001) docker     (121)      336 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/media_episode_thumbnail_atom_group.json
--rw-r--r--   0 runner    (1001) docker     (121)      267 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/media_episode_thumbnail_atom_group.rss
--rw-r--r--   0 runner    (1001) docker     (121)      368 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/media_episode_thumbnail_group.json
--rw-r--r--   0 runner    (1001) docker     (121)      270 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/media_episode_thumbnail_group.rss
--rw-r--r--   0 runner    (1001) docker     (121)      741 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/mediarss.json
--rw-r--r--   0 runner    (1001) docker     (121)      461 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/mediarss.rss
--rw-r--r--   0 runner    (1001) docker     (121)      606 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/multi_enclosures.json
--rw-r--r--   0 runner    (1001) docker     (121)      548 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/multi_enclosures.rss
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/new_feed_url.json
--rw-r--r--   0 runner    (1001) docker     (121)      151 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/new_feed_url.rss
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/no_enclosure.json
--rw-r--r--   0 runner    (1001) docker     (121)      187 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/no_enclosure.rss
--rw-r--r--   0 runner    (1001) docker     (121)      537 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/no_guid.json
--rw-r--r--   0 runner    (1001) docker     (121)      220 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/no_guid.rss
--rw-r--r--   0 runner    (1001) docker     (121)      519 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/no_permalink.json
--rw-r--r--   0 runner    (1001) docker     (121)      272 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/no_permalink.rss
--rw-r--r--   0 runner    (1001) docker     (121)      509 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/no_title.json
--rw-r--r--   0 runner    (1001) docker     (121)      166 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/no_title.rss
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/no_title_multi_enclosure.json
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/no_title_multi_enclosure.rss
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/no_url.json
--rw-r--r--   0 runner    (1001) docker     (121)      132 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/no_url.rss
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/paged_feed.json
--rw-r--r--   0 runner    (1001) docker     (121)      248 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/paged_feed.rss
--rw-r--r--   0 runner    (1001) docker     (121)      659 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/payment.json
--rw-r--r--   0 runner    (1001) docker     (121)      448 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/payment.rss
--rw-r--r--   0 runner    (1001) docker     (121)      583 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/permalink.json
--rw-r--r--   0 runner    (1001) docker     (121)      271 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/permalink.rss
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/redirect_new_location.json
--rw-r--r--   0 runner    (1001) docker     (121)      143 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/redirect_new_location.rss
--rw-r--r--   0 runner    (1001) docker     (121)      440 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/relative.json
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/relative.rss
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/relative_cover.json
--rw-r--r--   0 runner    (1001) docker     (121)      120 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/relative_cover.rss
--rw-r--r--   0 runner    (1001) docker     (121)      539 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/simple.json
--rw-r--r--   0 runner    (1001) docker     (121)      181 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/simple.rss
--rw-r--r--   0 runner    (1001) docker     (121)      310 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/yt-video-link.json
--rw-r--r--   0 runner    (1001) docker     (121)      312 2021-09-23 05:55:47.000000 podcastparser-0.6.8/tests/data/yt-video-link.rss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 07:00:25.560205 podcastparser-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-14 07:00:09.000000 podcastparser-0.6.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2022-12-14 07:00:09.000000 podcastparser-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2022-12-14 07:00:09.000000 podcastparser-0.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2022-12-14 07:00:25.560205 podcastparser-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2022-12-14 07:00:09.000000 podcastparser-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 07:00:25.548205 podcastparser-0.6.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2022-12-14 07:00:09.000000 podcastparser-0.6.9/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 07:00:25.548205 podcastparser-0.6.9/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 07:00:09.000000 podcastparser-0.6.9/doc/_static/.empty
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2022-12-14 07:00:09.000000 podcastparser-0.6.9/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9526 2022-12-14 07:00:09.000000 podcastparser-0.6.9/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2022-12-14 07:00:09.000000 podcastparser-0.6.9/makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 07:00:25.548205 podcastparser-0.6.9/podcastparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2022-12-14 07:00:25.000000 podcastparser-0.6.9/podcastparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2022-12-14 07:00:25.000000 podcastparser-0.6.9/podcastparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 07:00:25.000000 podcastparser-0.6.9/podcastparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-14 07:00:25.000000 podcastparser-0.6.9/podcastparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34657 2022-12-14 07:00:09.000000 podcastparser-0.6.9/podcastparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2022-12-14 07:00:09.000000 podcastparser-0.6.9/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2022-12-14 07:00:25.560205 podcastparser-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2022-12-14 07:00:09.000000 podcastparser-0.6.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2022-12-14 07:00:09.000000 podcastparser-0.6.9/test_podcastparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 07:00:25.544204 podcastparser-0.6.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 07:00:25.560205 podcastparser-0.6.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/atom_content_encoded.json
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/atom_content_encoded.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/atom_published_updated.json
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/atom_published_updated.rss
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/atom_relative_cover.json
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/atom_relative_cover.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/atom_updated.json
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/atom_updated.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/chapters.json
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/chapters.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/duration.json
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/duration.rss
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/empty.json
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/empty.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/episode_itunes_author.json
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/episode_itunes_author.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/episode_number.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/episode_number.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/episode_number_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/episode_number_invalid.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/episode_season.json
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/episode_season.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/episode_type.json
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/episode_type.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/episode_type_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/episode_type_invalid.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/explicit_episode.json
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/explicit_episode.rss
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/explicit_feed.json
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/explicit_feed.rss
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/generator.json
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/generator.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/html_description.json
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/html_description.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/html_description_rss_both.json
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/html_description_rss_both.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/html_in_description.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/html_in_description.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/html_in_description_rss_both.json
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/html_in_description_rss_both.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/html_in_description_rss_both_different.json
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/html_in_description_rss_both_different.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/image_and_audio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/image_and_audio.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/image_url_on_newline.json
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/image_url_on_newline.rss
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_author.json
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_author.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_categories.json
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_categories.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_categories_empty.json
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_categories_empty.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_duration.json
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_duration.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_episode_image.json
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_episode_image.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_keywords.json
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_keywords.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_no_xmlns.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_no_xmlns.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_owner.json
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_owner.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_owner_name_only.json
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_owner_name_only.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_subtitle.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_subtitle.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_type.json
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_type.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_type_garbage.json
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_type_garbage.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_type_missing.json
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_type_missing.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_type_serial.json
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_type_serial.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_xmlns.json
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/itunes_xmlns.rss
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/language.json
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/language.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/leading_space_url.json
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/leading_space_url.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/max_episodes.json
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/max_episodes.param.json
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/max_episodes.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/media_episode_thumbnail.json
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/media_episode_thumbnail.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/media_episode_thumbnail_atom.json
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/media_episode_thumbnail_atom.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/media_episode_thumbnail_atom_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/media_episode_thumbnail_atom_group.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/media_episode_thumbnail_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/media_episode_thumbnail_group.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/mediarss.json
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/mediarss.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/multi_enclosures.json
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/multi_enclosures.rss
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/new_feed_url.json
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/new_feed_url.rss
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/no_enclosure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/no_enclosure.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/no_guid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/no_guid.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/no_permalink.json
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/no_permalink.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/no_title.json
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/no_title.rss
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/no_title_multi_enclosure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/no_title_multi_enclosure.rss
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/no_url.json
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/no_url.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/paged_feed.json
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/paged_feed.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/payment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/payment.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/permalink.json
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/permalink.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/redirect_new_location.json
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/redirect_new_location.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/relative.json
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/relative.rss
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/relative_cover.json
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/relative_cover.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/simple.json
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/simple.rss
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/yt-video-link.json
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2022-12-14 07:00:09.000000 podcastparser-0.6.9/tests/data/yt-video-link.rss
```

### Comparing `podcastparser-0.6.8/LICENSE` & `podcastparser-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/PKG-INFO` & `podcastparser-0.6.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: podcastparser
-Version: 0.6.8
+Version: 0.6.9
 Summary:  Simplified, fast RSS parser 
 Home-page: http://gpodder.org/podcastparser/
 Author: Thomas Perl
 Author-email: m@thp.io
 License: ISC License
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 podcastparser: Simple, fast and efficient podcast parser
 ========================================================
 
@@ -26,9 +25,7 @@
 ## Automated Release to Pypi
 
 To release, update the version number in podcastparser.py, commit and push.
 
 Then create an (annotated) tag and push it.
 
 The GitHub action will publish on pypi.
-
-
```

### Comparing `podcastparser-0.6.8/README.md` & `podcastparser-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/doc/Makefile` & `podcastparser-0.6.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/doc/conf.py` & `podcastparser-0.6.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/doc/index.rst` & `podcastparser-0.6.9/doc/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,17 @@
 
 **rss/channel/itunes:image**
     Podcast cover art (alternative).
 
 **rss/channel/itunes:type**
     Podcast type (whitespace is squashed).  One of 'episodic' or 'serial'.  
 
+**rss/channel/itunes:keywords**
+    Podcast keywords (whitespace is squashed).
+
 **rss/channel/atom:link@rel=payment**
     Podcast payment URL (e.g. Flattr).
 
 **rss/channel/generator**
     A string indicating the program used to generate the channel. (e.g. MightyInHouse Content System v2.3).
 
 **rss/channel/language**
@@ -101,14 +104,17 @@
 **rss/channel/itunes:author**
     The group responsible for creating the show.
 
 **rss/channel/itunes:owner**
     The podcast owner contact information.
     The <itunes:owner> tag information is for administrative communication about the podcast and isn't displayed in Apple Podcasts
 
+**rss/channel/itunes:category**
+    The show category information.
+
 **rss/channel/itunes:explicit**
     Indicates whether podcast contains explicit material.
 
 **rss/channel/itunes:new-feed-url**
     The new podcast RSS Feed URL.
 
 **rss/redirect/newLocation**
@@ -180,14 +186,17 @@
 
 **rss/channel/item/itunes:explicit**
     Indicates whether episode contains explicit material.
 
 **rss/channel/item/itunes:author**
     The group responsible for creating the episode.
 
+**rss/channel/item/itunes:season**
+    The season number of the episode.
+
 **rss/channel/item/itunes:episode**
     An episode number.
 
 **rss/channel/item/itunes:episodeType**
     The episode type.
     This flag is used if an episode is a trailer or bonus content.
```

### Comparing `podcastparser-0.6.8/podcastparser.egg-info/PKG-INFO` & `podcastparser-0.6.9/podcastparser.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: podcastparser
-Version: 0.6.8
+Version: 0.6.9
 Summary:  Simplified, fast RSS parser 
 Home-page: http://gpodder.org/podcastparser/
 Author: Thomas Perl
 Author-email: m@thp.io
 License: ISC License
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 podcastparser: Simple, fast and efficient podcast parser
 ========================================================
 
@@ -26,9 +25,7 @@
 ## Automated Release to Pypi
 
 To release, update the version number in podcastparser.py, commit and push.
 
 Then create an (annotated) tag and push it.
 
 The GitHub action will publish on pypi.
-
-
```

### Comparing `podcastparser-0.6.8/podcastparser.egg-info/SOURCES.txt` & `podcastparser-0.6.9/podcastparser.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 tests/data/empty.rss
 tests/data/episode_itunes_author.json
 tests/data/episode_itunes_author.rss
 tests/data/episode_number.json
 tests/data/episode_number.rss
 tests/data/episode_number_invalid.json
 tests/data/episode_number_invalid.rss
+tests/data/episode_season.json
+tests/data/episode_season.rss
 tests/data/episode_type.json
 tests/data/episode_type.rss
 tests/data/episode_type_invalid.json
 tests/data/episode_type_invalid.rss
 tests/data/explicit_episode.json
 tests/data/explicit_episode.rss
 tests/data/explicit_feed.json
@@ -58,18 +60,24 @@
 tests/data/html_in_description_rss_both_different.rss
 tests/data/image_and_audio.json
 tests/data/image_and_audio.rss
 tests/data/image_url_on_newline.json
 tests/data/image_url_on_newline.rss
 tests/data/itunes_author.json
 tests/data/itunes_author.rss
+tests/data/itunes_categories.json
+tests/data/itunes_categories.rss
+tests/data/itunes_categories_empty.json
+tests/data/itunes_categories_empty.rss
 tests/data/itunes_duration.json
 tests/data/itunes_duration.rss
 tests/data/itunes_episode_image.json
 tests/data/itunes_episode_image.rss
+tests/data/itunes_keywords.json
+tests/data/itunes_keywords.rss
 tests/data/itunes_no_xmlns.json
 tests/data/itunes_no_xmlns.rss
 tests/data/itunes_owner.json
 tests/data/itunes_owner.rss
 tests/data/itunes_owner_name_only.json
 tests/data/itunes_owner_name_only.rss
 tests/data/itunes_subtitle.json
```

### Comparing `podcastparser-0.6.8/podcastparser.py` & `podcastparser-0.6.9/podcastparser.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,56 +18,28 @@
 # PERFORMANCE OF THIS SOFTWARE.
 #
 
 """ Simplified, fast RSS parser """
 
 # Will be parsed by setup.py to determine package metadata
 __author__ = 'Thomas Perl <m@thp.io>'
-__version__ = '0.6.8'
+__version__ = '0.6.9'
 __website__ = 'http://gpodder.org/podcastparser/'
 __license__ = 'ISC License'
 
 from xml import sax
 
 import re
 import os
 import time
 
-try:
-    # Python 2
-    from htmlentitydefs import entitydefs
-    entitydefs = dict((key, value.decode('latin-1')) for key, value in entitydefs.iteritems())
-    chr = unichr
-except ImportError:
-    # Python 3
-    from html.entities import entitydefs
-
-try:
-    # Python 2
-    import urlparse
-except ImportError:
-    # Python 3
-    from urllib import parse as urlparse
-
-try:
-    # Python 2
-    from rfc822 import parsedate_tz
-    import calendar
-    # This is taken from Python 3's email._parseaddr, since it handles
-    # pre-epoch dates better than what Python 2 does (time.mktime())
-    def mktime_tz(data):
-        if data[9] is None:
-            # No zone info, so localtime is better assumption than GMT
-            return time.mktime(data[:8] + (-1,))
-        else:
-            t = calendar.timegm(data)
-            return t - data[9]
-except ImportError:
-    # Python 3
-    from email.utils import mktime_tz, parsedate_tz
+from html.entities import entitydefs
+
+from urllib import parse as urlparse
+from email.utils import mktime_tz, parsedate_tz
 
 import logging
 logger = logging.getLogger(__name__)
 
 
 class Target(object):
     WANT_TEXT = False
@@ -102,14 +74,20 @@
 
 class PodcastAttr(Target):
     WANT_TEXT = True
 
     def end(self, handler, text):
         handler.set_podcast_attr(self.key, self.filter_func(text))
 
+class PodcastAttrList(Target):
+    WANT_TEXT = True
+
+    def end(self, handler, text):
+        handler.set_podcast_attr(self.key, self.filter_func(text).split(', '))
+
 
 class PodcastAttrType(Target):
     WANT_TEXT = True
 
     def end(self, handler, text):
         value = self.filter_func(text)
         if value in ('episodic', 'serial'):
@@ -181,14 +159,23 @@
             handler.set_episode_attr(self.key, self.filter_func(value))
 
 
 class EpisodeAttrFromUrl(EpisodeAttrFromHref):
     ATTRIBUTE = 'url'
 
 
+class EpisodeAttrSeason(EpisodeAttr):
+    def end(self, handler, text):
+        try:
+            episode_season = int(text)
+        except ValueError:
+            episode_season = 0
+        handler.set_episode_attr(self.key, episode_season)
+
+
 class EpisodeAttrNumber(EpisodeAttr):
     def end(self, handler, text):
         value = self.filter_func(text)
         try:
             episode_num = int(value)
         except ValueError:
             return
@@ -327,14 +314,30 @@
 
     def end(self, handler, text):
         if not self.overwrite and handler.get_episode_attr(self.key):
             return
         handler.append_itunes_owner(self.key, self.filter_func(text))
 
 
+class ItunesCategoryAttr(Target):
+    def start(self, handler, attrs):
+        # Let's use an empty string as a fallback for first-level categories
+        # in case there is a valid sub-category.
+        value = attrs.get('text', '')
+        handler.append_itunes_category(self.key, self.filter_func(value))
+
+
+class ItunesSubCategoryAttr(Target):
+    def start(self, handler, attrs):
+        value = attrs.get('text')
+        if not value:
+            return
+        handler.append_itunes_subcategory(self.key, self.filter_func(value))
+
+
 class ItunesOwnerItem(Target):
     def start(self, handler, attrs):
         handler.add_itunes_owner()
 
 
 class PodcastAttrExplicit(Target):
     WANT_TEXT = True
@@ -654,16 +657,16 @@
         return 0
 
     parsed = parsedate_tz(text)
     if parsed is not None:
         try:
             pubtimeseconds = int(mktime_tz(parsed))
             return pubtimeseconds
-        except(OverflowError,ValueError):
-            logger.warning('bad pubdate %s is before epoch or after end of time (2038)',parsed)
+        except(OverflowError, ValueError):
+            logger.warning('bad pubdate %s is before epoch or after end of time (2038)', parsed)
             return 0
 
     try:
         parsed = time.strptime(text[:19], '%Y-%m-%dT%H:%M:%S')
         if parsed is not None:
             m = re.match(r'^(?:Z|([+-])([0-9]{2})[:]([0-9]{2}))$', text[19:])
             if m:
@@ -695,18 +698,24 @@
     'rss/channel/description': PodcastAttr('description', squash_whitespace_not_nl),
     'rss/channel/image/url': PodcastAttrRelativeLink('cover_url'),
     'rss/channel/itunes:image': PodcastAttrFromHref('cover_url'),
     'rss/channel/itunes:type': PodcastAttrType('type', squash_whitespace),
     'rss/channel/atom:link': PodcastAtomLink(),
     'rss/channel/generator': PodcastAttr('generator', squash_whitespace),
     'rss/channel/language': PodcastAttr('language', squash_whitespace),
+
+    'rss/channel/itunes:category': ItunesCategoryAttr('itunes_categories'),
+    'rss/channel/itunes:category/itunes:category': ItunesSubCategoryAttr('itunes_categories'),
+    'rss/channel/itunes:category/itunes:category/itunes:category': ItunesSubCategoryAttr('itunes_categories'),
+
     'rss/channel/itunes:author': PodcastAttr('itunes_author', squash_whitespace),
     'rss/channel/itunes:owner': ItunesOwnerItem('itunes_owner', squash_whitespace),
     'rss/channel/itunes:explicit': PodcastAttrExplicit('explicit', squash_whitespace),
     'rss/channel/itunes:new-feed-url': PodcastAttr('new_url', squash_whitespace),
+    'rss/channel/itunes:keywords': PodcastAttrList('itunes_keywords', squash_whitespace),
     'rss/redirect/newLocation': PodcastAttr('new_url', squash_whitespace),
 
     'rss/channel/itunes:owner/itunes:email': ItunesOwnerAttr('email', squash_whitespace),
     'rss/channel/itunes:owner/itunes:name': ItunesOwnerAttr('name', squash_whitespace),
 
     'rss/channel/item': EpisodeItem(),
     'rss/channel/item/guid': EpisodeGuid('guid'),
@@ -718,14 +727,15 @@
     'rss/channel/item/itunes:subtitle': EpisodeAttr('subtitle', squash_whitespace),
     'rss/channel/item/content:encoded': EpisodeAttr('description_html'),
     'rss/channel/item/itunes:duration': EpisodeAttr('total_time', parse_time),
     'rss/channel/item/pubDate': EpisodeAttr('published', parse_pubdate),
     'rss/channel/item/atom:link': AtomLink(),
     'rss/channel/item/itunes:explicit': EpisodeAttrExplicit('explicit', squash_whitespace),
     'rss/channel/item/itunes:author': EpisodeAttr('itunes_author', squash_whitespace),
+    'rss/channel/item/itunes:season': EpisodeAttrSeason('season', squash_whitespace),
     'rss/channel/item/itunes:episode': EpisodeAttrNumber('number', squash_whitespace),
     'rss/channel/item/itunes:episodeType': EpisodeAttrType('type', squash_whitespace),
 
     'rss/channel/item/itunes:image': EpisodeAttrFromHref('episode_art_url'),
     'rss/channel/item/media:thumbnail': EpisodeAttrFromUrl('episode_art_url'),
     'rss/channel/item/media:group/media:thumbnail': EpisodeAttrFromUrl('episode_art_url'),
 
@@ -864,14 +874,24 @@
 
     def add_itunes_owner(self):
         self.data['itunes_owner'] = {}
 
     def append_itunes_owner(self, key, value):
         self.data['itunes_owner'][key] = value
 
+    def add_itunes_categories(self):
+        self.data['itunes_categories'] = []
+
+    def append_itunes_category(self, key, value):
+        self.data.setdefault('itunes_categories', []).append([value])
+
+    def append_itunes_subcategory(self, key, value):
+        entry = self.data['itunes_categories'][-1]
+        entry.append(value)
+
     def startElement(self, name, attrs):
         self.namespace = Namespace(attrs, self.namespace)
         name = self.namespace.map(name)
         if not self.path_stack and name not in VALID_ROOTS:
             raise FeedParseError(
                 msg='Unsupported feed type: {}'.format(name),
                 exception=None,
@@ -984,26 +1004,30 @@
 
     if scheme not in ('http', 'https', 'ftp', 'file'):
         return None
 
     # urlunsplit might return "a slighty different, but equivalent URL"
     return urlparse.urlunsplit((scheme, netloc, path, query, fragment))
 
+
 HTML_TEST = re.compile(r'<[a-z][a-z0-9]*(?:\s.*?>|\/?>)', re.IGNORECASE | re.DOTALL)
+
+
 def is_html(text):
     """Heuristically tell if text is HTML
 
     By looking for an open tag (more or less:)
     >>> is_html('<h1>HELLO</h1>')
     True
     >>> is_html('a < b < c')
     False
     """
     return bool(HTML_TEST.search(text))
 
+
 def remove_html_tags(html):
     """
     Remove HTML tags from a string and replace numeric and
     named entities with the corresponding character, so the
     HTML text can be displayed in a simple text view.
     """
     if html is None:
```

### Comparing `podcastparser-0.6.8/setup.py` & `podcastparser-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/test_podcastparser.py` & `podcastparser-0.6.9/test_podcastparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,15 @@
 # PERFORMANCE OF THIS SOFTWARE.
 #
 
 
 import os
 import glob
 import json
-try:
-    # Python 2
-    from StringIO import StringIO
-except ImportError:
-    # Python 3
-    from io import StringIO
+import io
 
 
 import pytest
 import podcastparser
 
 
 class TestPodcastparser:
@@ -60,9 +55,9 @@
         '<html><body/></html>',
         '<foo xmlns="http://example.com/foo.xml"><bar/></foo>',
         '<baz:foo xmlns:baz="http://example.com/baz.xml"><baz:bar/></baz:foo>',
     ]
     @pytest.mark.parametrize("feed", feeds)
     def test_fail_parse(self, feed):
         with pytest.raises(podcastparser.FeedParseError):
-            podcastparser.parse('file://example.com/feed.xml', StringIO(feed))
+            podcastparser.parse('file://example.com/feed.xml', io.StringIO(feed))
```

### Comparing `podcastparser-0.6.8/tests/data/atom_content_encoded.rss` & `podcastparser-0.6.9/tests/data/atom_content_encoded.rss`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/atom_published_updated.rss` & `podcastparser-0.6.9/tests/data/atom_published_updated.rss`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/atom_updated.rss` & `podcastparser-0.6.9/tests/data/atom_updated.rss`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/chapters.json` & `podcastparser-0.6.9/tests/data/chapters.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/chapters.rss` & `podcastparser-0.6.9/tests/data/chapters.rss`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/episode_itunes_author.json` & `podcastparser-0.6.9/tests/data/episode_itunes_author.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/episode_number.json` & `podcastparser-0.6.9/tests/data/episode_number.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/episode_number_invalid.json` & `podcastparser-0.6.9/tests/data/episode_number_invalid.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/episode_type.json` & `podcastparser-0.6.9/tests/data/episode_type.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/episode_type_invalid.json` & `podcastparser-0.6.9/tests/data/episode_type_invalid.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/explicit_episode.json` & `podcastparser-0.6.9/tests/data/explicit_episode.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/html_description.json` & `podcastparser-0.6.9/tests/data/html_description.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/html_description_rss_both.json` & `podcastparser-0.6.9/tests/data/html_description_rss_both.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/html_in_description.json` & `podcastparser-0.6.9/tests/data/html_in_description.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/html_in_description_rss_both.json` & `podcastparser-0.6.9/tests/data/html_in_description_rss_both.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/html_in_description_rss_both_different.json` & `podcastparser-0.6.9/tests/data/html_in_description_rss_both_different.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/image_and_audio.json` & `podcastparser-0.6.9/tests/data/image_and_audio.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/itunes_type.json` & `podcastparser-0.6.9/tests/data/itunes_type.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/itunes_type_garbage.json` & `podcastparser-0.6.9/tests/data/itunes_type_garbage.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/itunes_type_missing.json` & `podcastparser-0.6.9/tests/data/itunes_type_missing.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/itunes_type_serial.json` & `podcastparser-0.6.9/tests/data/itunes_type_serial.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/max_episodes.json` & `podcastparser-0.6.9/tests/data/max_episodes.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/mediarss.json` & `podcastparser-0.6.9/tests/data/mediarss.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/multi_enclosures.json` & `podcastparser-0.6.9/tests/data/multi_enclosures.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/multi_enclosures.rss` & `podcastparser-0.6.9/tests/data/multi_enclosures.rss`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/no_enclosure.json` & `podcastparser-0.6.9/tests/data/no_enclosure.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/no_guid.json` & `podcastparser-0.6.9/tests/data/no_guid.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/no_permalink.json` & `podcastparser-0.6.9/tests/data/no_permalink.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/payment.json` & `podcastparser-0.6.9/tests/data/payment.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/permalink.json` & `podcastparser-0.6.9/tests/data/permalink.json`

 * *Files identical despite different names*

### Comparing `podcastparser-0.6.8/tests/data/simple.json` & `podcastparser-0.6.9/tests/data/simple.json`

 * *Files identical despite different names*

