# Comparing `tmp/pr-review-bot-0.2.0.tar.gz` & `tmp/pr-review-bot-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr-review-bot-0.2.0.tar", last modified: Sun Apr 16 04:11:14 2023, max compression
+gzip compressed data, was "pr-review-bot-0.2.1.tar", last modified: Tue Apr 18 03:17:58 2023, max compression
```

## Comparing `pr-review-bot-0.2.0.tar` & `pr-review-bot-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:11:14.100895 pr-review-bot-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 04:10:58.000000 pr-review-bot-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-16 04:11:14.100895 pr-review-bot-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-16 04:10:58.000000 pr-review-bot-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:11:14.100895 pr-review-bot-0.2.0/pr_review_bot/
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-16 04:10:58.000000 pr-review-bot-0.2.0/pr_review_bot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:11:14.100895 pr-review-bot-0.2.0/pr_review_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-16 04:11:14.000000 pr-review-bot-0.2.0/pr_review_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-16 04:11:14.000000 pr-review-bot-0.2.0/pr_review_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 04:11:14.000000 pr-review-bot-0.2.0/pr_review_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-16 04:11:14.000000 pr-review-bot-0.2.0/pr_review_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-16 04:11:14.000000 pr-review-bot-0.2.0/pr_review_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-16 04:10:58.000000 pr-review-bot-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 04:11:14.100895 pr-review-bot-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:11:14.100895 pr-review-bot-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-16 04:10:58.000000 pr-review-bot-0.2.0/tests/test_pr_review_bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:17:58.854063 pr-review-bot-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 03:17:42.000000 pr-review-bot-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-04-18 03:17:58.854063 pr-review-bot-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-18 03:17:42.000000 pr-review-bot-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:17:58.854063 pr-review-bot-0.2.1/pr_review_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-18 03:17:42.000000 pr-review-bot-0.2.1/pr_review_bot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:17:58.854063 pr-review-bot-0.2.1/pr_review_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-04-18 03:17:58.000000 pr-review-bot-0.2.1/pr_review_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-18 03:17:58.000000 pr-review-bot-0.2.1/pr_review_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 03:17:58.000000 pr-review-bot-0.2.1/pr_review_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 03:17:58.000000 pr-review-bot-0.2.1/pr_review_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 03:17:58.000000 pr-review-bot-0.2.1/pr_review_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-18 03:17:42.000000 pr-review-bot-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 03:17:58.854063 pr-review-bot-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:17:58.854063 pr-review-bot-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-18 03:17:42.000000 pr-review-bot-0.2.1/tests/test_pr_review_bot.py
```

### Comparing `pr-review-bot-0.2.0/LICENSE` & `pr-review-bot-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pr-review-bot-0.2.0/PKG-INFO` & `pr-review-bot-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-review-bot
-Version: 0.2.0
+Version: 0.2.1
 Summary: Automated PR review bot using GPT-3.5-turbo
 Author-email: Kyryl Truskovskyi <truskovskiyk@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -268,9 +268,9 @@
 pr-review-bot --help
 ```
 
 ## Testing 
 
 
 ```
-pytest --cov=pr_review_bot test_pr_review_bot.py
+pytest --cov=pr_review_bot ./tests
 ```
```

### Comparing `pr-review-bot-0.2.0/README.md` & `pr-review-bot-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -58,9 +58,9 @@
 pr-review-bot --help
 ```
 
 ## Testing 
 
 
 ```
-pytest --cov=pr_review_bot test_pr_review_bot.py
+pytest --cov=pr_review_bot ./tests
 ```
```

### Comparing `pr-review-bot-0.2.0/pr_review_bot/__init__.py` & `pr-review-bot-0.2.1/pr_review_bot/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,20 +22,24 @@
 ghapi = GhApi(token=settings.TOKEN, owner=settings.OWNER, repo=settings.REPO_NAME)
 
 app = typer.Typer()
 
 def get_open_prs() -> List[Any]:
     return ghapi.pulls.list(state='open')
 
+
+def get_patch(pr_file: Any) -> str:
+    return pr_file.patch if pr_file.changes != 0 else 'no changes'
+
 def analyze_pr(pr: Any) -> Dict[str, Union[str, float]]:
     pr_description = pr.body
 
     # Read all PR files
     pr_files = ghapi.pulls.list_files(pr.number)
-    pr_content = "\n".join(f"filename: {file.filename}: status: {file.status} patch: {file.patch}" for file in pr_files)
+    pr_content = "\n\n\n".join(f"filename: {file.filename}: status: {file.status} patch: {get_patch(file)} " for file in pr_files)
 
     # Read all PR comments
     comments = ghapi.issues.list_comments(pr.number)
     pr_comments = "\n".join(comment.body for comment in comments)
 
     text = f"pr_description\n {pr_description}, \npr_content\n = {pr_content}, \npr_comments\n = {pr_comments}"
 
@@ -47,30 +51,41 @@
     response = openai.ChatCompletion.create(
         model=settings.MODEL_NAME,
         messages=messages,
     )
 
     review_cost = response['usage']['total_tokens'] * settings.PRICE_PER_TOKEN
     review = response.choices[0].message['content'].strip()
-    review = f"Review \n\n{review}\n \n\nReview costs \n\n{review_cost} USD"
+    review = f"Review from GPT \n\n{review}\n \n\nReview costs \n\n{review_cost} USD"
 
     event = "COMMENT"
 
     if "approve" in review.lower():
         event = "APPROVE"
     elif "request changes" in review.lower():
         event = "REQUEST_CHANGES"
 
     return {
         'body': review,
         'event': event
     }
 
-def submit_review(pr: Any, review: Dict[str, Union[str, float]]) -> None:
-    ghapi.pulls.create_review(pr.number, body=review['body'], event=review['event'])
+def submit_review(pr: Any, review: Dict[str, Union[str, float]], label_name: str = "pr_review_bot") -> None:
+    pr_number = pr.number
+
+    # Create the label if it doesn't exist
+    labels = ghapi.issues.list_labels_for_repo()
+    if not any(label.name == label_name for label in labels):
+        ghapi.issues.create_label(name=label_name, color="d73a4a", description="Label for autogenerated reviews")
+
+    # Add the label to the PR
+    ghapi.issues.add_labels(issue_number=pr_number, labels=[label_name])
+
+    # Submit the review
+    ghapi.pulls.create_review(pr_number, body=review['body'], event=review['event'])
 
 @app.command()
 def review_all_open_pr() -> None:
     open_prs = get_open_prs()
     for pr in open_prs:
         review = analyze_pr(pr)
         if review:
```

### Comparing `pr-review-bot-0.2.0/pr_review_bot.egg-info/PKG-INFO` & `pr-review-bot-0.2.1/pr_review_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-review-bot
-Version: 0.2.0
+Version: 0.2.1
 Summary: Automated PR review bot using GPT-3.5-turbo
 Author-email: Kyryl Truskovskyi <truskovskiyk@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -268,9 +268,9 @@
 pr-review-bot --help
 ```
 
 ## Testing 
 
 
 ```
-pytest --cov=pr_review_bot test_pr_review_bot.py
+pytest --cov=pr_review_bot ./tests
 ```
```

### Comparing `pr-review-bot-0.2.0/pyproject.toml` & `pr-review-bot-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pr-review-bot"
-version = "0.2.0"
+version = "0.2.1"
 description = "Automated PR review bot using GPT-3.5-turbo"
 authors = [
     {name = "Kyryl Truskovskyi", email = "truskovskiyk@gmail.com"}
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
```

