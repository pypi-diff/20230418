# Comparing `tmp/tinote-1.1.0.tar.gz` & `tmp/tinote-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinote-1.1.0.tar", last modified: Tue Apr 18 02:09:23 2023, max compression
+gzip compressed data, was "tinote-1.1.1.tar", last modified: Tue Apr 18 20:23:03 2023, max compression
```

## Comparing `tinote-1.1.0.tar` & `tinote-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 02:09:23.382849 tinote-1.1.0/
--rw-rw-rw-   0        0        0     2236 2023-04-18 02:09:23.381850 tinote-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1422 2023-04-17 21:21:01.000000 tinote-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 02:09:23.382849 tinote-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1459 2023-04-18 02:08:26.000000 tinote-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:09:23.362836 tinote-1.1.0/tinote/
--rw-rw-rw-   0        0        0        0 2023-04-15 02:09:36.000000 tinote-1.1.0/tinote/__init__.py
--rw-rw-rw-   0        0        0     9882 2023-04-18 02:03:30.000000 tinote-1.1.0/tinote/main.py
--rw-rw-rw-   0        0        0     1503 2023-04-18 02:06:31.000000 tinote-1.1.0/tinote/update.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:09:23.380861 tinote-1.1.0/tinote.egg-info/
--rw-rw-rw-   0        0        0     2236 2023-04-18 02:09:23.000000 tinote-1.1.0/tinote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-04-18 02:09:23.000000 tinote-1.1.0/tinote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 02:09:23.000000 tinote-1.1.0/tinote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-18 02:09:23.000000 tinote-1.1.0/tinote.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 02:09:23.000000 tinote-1.1.0/tinote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:23:03.233463 tinote-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-18 20:23:03.233463 tinote-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-18 20:22:51.000000 tinote-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:23:03.233463 tinote-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-18 20:22:51.000000 tinote-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:23:03.233463 tinote-1.1.1/tinote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:22:51.000000 tinote-1.1.1/tinote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-04-18 20:22:51.000000 tinote-1.1.1/tinote/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-18 20:22:51.000000 tinote-1.1.1/tinote/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:23:03.233463 tinote-1.1.1/tinote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-18 20:23:03.000000 tinote-1.1.1/tinote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-18 20:23:03.000000 tinote-1.1.1/tinote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:23:03.000000 tinote-1.1.1/tinote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 20:23:03.000000 tinote-1.1.1/tinote.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 20:23:03.000000 tinote-1.1.1/tinote.egg-info/top_level.txt
```

### Comparing `tinote-1.1.0/PKG-INFO` & `tinote-1.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-Metadata-Version: 2.1
-Name: tinote
-Version: 1.1.0
-Summary: A command-line note-taking tool
-Home-page: https://github.com/aPeter1/tinote
-Author: Alec Petersen
-Author-email: k.alecpetersen@gmail.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Terminals
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# Tinote
-
-Tinote is a lightweight command-line note-taking tool, designed for quick and easy note management. Keep track of your thoughts, ideas, or reminders directly from the terminal.
-
-## Installation
-
-Install Tinote using pip:
-
-```bash
-pip install tinote
-```
-
-## Usage
-
-Create a new note (if no category is provided, the last category will be used):
-
-```bash
-ti add "a note to remember" <optional category> <optional importance>
-```
-
-List all notes (verbose list will include importance and timestamp):
-
-```bash
-ti list [-v]
-```
-
-List notes with filters (category or importance):
-
-```bash
-ti list -c <category> -i <importance>
-```
-
-Add a sub-note to a note (currently only supports one level)
-
-```bash
-ti sub <parent_id> "Text of your sub-note" -i <importance>
-```
-
-Mark a note as checked/unchecked:
-
-```bash
-ti mark <note_id>
-```
-
-Delete a note:
-
-```bash
-ti delete <note_id>
-```
-
-Clear all notes or notes within a specified category:
-
-```bash
-ti clear
-ti clear -c <category>
-```
-
-## Features
-
-- Create and manage notes with optional categories and importance levels
-- List notes, with optional filters for categories and importance
-- Easily mark notes as checked/unchecked
-- Delete notes using their ID
-- Clear all notes or notes within a specified category
-- Automatically saves notes to a local JSON file for persistence
-
-## License
-
-MIT License
+Metadata-Version: 2.1
+Name: tinote
+Version: 1.1.1
+Summary: A command-line note-taking tool
+Home-page: https://github.com/aPeter1/tinote
+Author: Alec Petersen
+Author-email: k.alecpetersen@gmail.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Terminals
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+![Logo](assets/color-logo-no-background.png)
+
+Tinote is a lightweight command-line note-taking tool, designed for quick and easy note management. Keep track of your thoughts, ideas, or reminders directly from the terminal.
+
+## Installation
+
+Install Tinote using pip:
+
+```bash
+pip install tinote
+```
+
+## Usage
+
+Create a new note (if no category is provided, the last category will be used):
+
+```bash
+ti add "a note to remember" <optional category> <optional importance>
+```
+
+List all notes (verbose list will include importance and timestamp):
+
+```bash
+ti list [-v]
+```
+
+List notes with filters (category or importance):
+
+```bash
+ti list -c <category> -i <importance>
+```
+
+Add a sub-note to a note (currently only supports one level)
+
+```bash
+ti sub <parent_id> "Text of your sub-note" -i <importance>
+```
+
+Mark a note as checked/unchecked:
+
+```bash
+ti mark <note_id>
+```
+
+Delete a note:
+
+```bash
+ti delete <note_id>
+```
+
+Clear all notes or notes within a specified category:
+
+```bash
+ti clear
+ti clear -c <category>
+```
+
+## Features
+
+- Create and manage notes with optional categories and importance levels
+- List notes, with optional filters for categories and importance
+- Easily mark notes as checked/unchecked
+- Delete notes using their ID
+- Clear all notes or notes within a specified category
+- Automatically saves notes to a local JSON file for persistence
+
+## License
+
+MIT License
```

### Comparing `tinote-1.1.0/tinote/main.py` & `tinote-1.1.1/tinote/main.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,257 +1,257 @@
-import json
-import argparse
-import os
-from datetime import datetime
-import textwrap
-
-
-NOTES_FILE = os.path.expanduser("~/.ti_notes.json")
-
-
-def save_notes(notes, max_id, last_category):
-    with open(NOTES_FILE, "w") as f:
-        json.dump({"notes": notes, "max_id": max_id, "last_category": last_category}, f, indent=2)
-
-
-def load_notes():
-    if not os.path.exists(NOTES_FILE):
-        return [], 0, "unknown"  # Return max_id as 0 for an empty file
-
-    with open(NOTES_FILE, "r") as f:
-        content = f.read().strip()
-        if not content:
-            return [], 0, "unknown"  # Return max_id as 0 for an empty file
-
-        data = json.loads(content)
-        notes, max_id, last_category = data.get("notes", []), data.get("max_id", 0), data.get("last_category",
-                                                                                              "unknown")
-        return notes, max_id, last_category
-
-
-def create_note(note, category, importance):
-    notes, max_id, last_category = load_notes()
-    category = last_category if category is None else category
-
-    new_id = max_id + 1
-
-    new_note = {
-        "id": new_id,  # Use the new ID
-        "note": note,
-        "category": category,
-        "importance": importance,
-        "created_timestamp": datetime.now().isoformat(),
-        "marked_timestamp": None,
-        "subs": [],
-        "checked": False,
-    }
-
-    notes.append(new_note)
-    save_notes(notes, new_id, category)  # Update max_id
-
-    print("Note added successfully.")
-
-
-def create_sub_note(note, parent_id, importance):
-    notes, max_id, last_category = load_notes()
-
-    for n in notes:
-        if n["id"] == parent_id:
-            parent_note = n
-            break
-    else:
-        print("Parent does not exist.")
-        return
-
-    new_id = max_id + 1
-
-    new_note = {
-        "id": new_id,  # Use the new ID
-        "parent": parent_id,
-        "note": note,
-        "category": parent_note["category"],
-        "importance": importance,
-        "created_timestamp": datetime.now().isoformat(),
-        "marked_timestamp": None,
-        "checked": False,
-    }
-
-    try:
-        parent_note["subs"].append(new_note)
-    except KeyError:
-        parent_note["subs"] = [new_note]
-
-    save_notes(notes, new_id, last_category)
-
-    print("Sub-note added successfully.")
-
-
-def format_note(note_text, sub=False):
-    bullet_indent = "\t\t" if sub else "\t"
-    lines = note_text.split("*")
-    formatted_lines = [lines[0]] + [f"{bullet_indent}* {line.strip()}" for line in lines[1:]]
-    return "\n".join(formatted_lines)
-
-
-def list_notes(category=None, importance=None, verbose=None):
-    notes, _, _ = load_notes()
-
-    if not category:
-        sorted_notes = sorted(notes, key=lambda x: x['category'])
-    else:
-        sorted_notes = [note for note in notes if note['category'] == category]
-
-    def display_notes(notes_list, indent=0):
-        for note in notes_list:
-            if importance and note["importance"] != importance:
-                continue
-
-            checked_symbol = "✔" if note["checked"] else "✘"
-            importance_symbol = f"[{note['importance']}]" if note["importance"] is not None and verbose else ""
-            created_timestamp = f'(Created {note["created_timestamp"]})' if verbose else ""
-            marked_timestamp = f'(Mark Updated {note["marked_timestamp"]})' if verbose and note["marked_timestamp"] is not None else ""
-
-            lines = textwrap.wrap(note['note'], width=80 - indent)
-            first_line = lines.pop(0)
-
-            print(
-                f"{indent * ' '}{checked_symbol} {note['id']} {first_line} "
-                f"{importance_symbol} {created_timestamp} {marked_timestamp}"
-            )
-
-            for line in lines:
-                print(f"{indent * ' '}   {line}")
-
-            try:
-                if note["subs"]:
-                    display_notes(note["subs"], indent + 4)
-            except KeyError:
-                pass
-
-    grouped_notes = {}
-    for note in sorted_notes:
-        grouped_notes.setdefault(note['category'], []).append(note)
-
-    for category, cat_notes in grouped_notes.items():
-        print(f"\n{category.upper()}{'-' * (80 - len(category))}")
-        display_notes(cat_notes)
-
-
-def mark_note(note_id, checked=True):
-    notes, max_id, last_category = load_notes()
-
-    for note in notes:
-        if note["id"] == note_id:
-            note["checked"] = checked
-            note["marked_timestamp"] = datetime.now().isoformat()
-            save_notes(notes, max_id, last_category)
-            print(f"Note {'marked' if checked else 'unmarked'} successfully.")
-            return
-
-        for index, sub in enumerate(note["subs"]):
-            if sub["id"] == note_id:
-                sub["checked"] = checked
-                note["marked_timestamp"] = datetime.now().isoformat()
-                save_notes(notes, max_id, last_category)
-                print(f"Note {'marked' if checked else 'unmarked'} successfully.")
-                return
-    else:
-        print("Invalid note ID.")
-
-
-def delete_note(note_id):
-    notes, max_id, last_category = load_notes()
-
-    for index, note in enumerate(notes):
-        if note["id"] == note_id:
-            del notes[index]
-            save_notes(notes, max_id, last_category)
-            print("Note deleted successfully.")
-            return
-
-        for sub_index, sub in enumerate(note["subs"]):
-            if sub["id"] == note_id:
-                del note["subs"][sub_index]
-                save_notes(notes, max_id, last_category)
-                print("Note deleted successfully.")
-                return
-    else:
-        print("Invalid note ID.")
-
-
-def clear_notes(category=None):
-    notes, max_id, last_category = load_notes()
-    if category:
-        notes = [note for note in notes if note['category'] != category]
-    else:
-        notes = []
-
-    save_notes(notes, max_id, last_category)
-    if category:
-        print(f"Successfully cleared all notes in category '{category}'.")
-    else:
-        print("Successfully cleared all notes.")
-
-
-def main():
-    parser = argparse.ArgumentParser(description="A command-line tool for taking quick notes.", prog="ti")
-    subparsers = parser.add_subparsers(dest="subcommand")
-
-    # Add subparser for 'add' command
-    add_parser = subparsers.add_parser("add", help="Add a new note.")
-    add_parser.add_argument("note", type=str, help="The content of the note.")
-    add_parser.add_argument("category", type=str, nargs="?", default=None,
-                            help="Optional category for the note. If none is provided, the last category will be used.")
-    add_parser.add_argument("importance", type=int, nargs="?", default=None,
-                            help="Optional importance level for the note (integer).")
-    add_parser.add_argument("-c", "--category", type=str, default=None,
-                            help="Optional category for the note. If none is provided, the last category will be used.",
-                            dest="category_keyword")
-    add_parser.add_argument("-i", "--importance", type=int, default=None,
-                            help="Optional importance level for the note (integer).", dest="importance_keyword")
-
-    sub_parser = subparsers.add_parser('sub', help='Add a sub-note to a note')
-    sub_parser.add_argument('parent_id', type=int, help='Parent note ID')
-    sub_parser.add_argument('note', type=str, help='Sub-note text')
-    sub_parser.add_argument("-i", "--importance", type=int, default=None,
-                            help="Optional importance level for the note (integer).")
-
-    # Add subparser for 'list' command
-    list_parser = subparsers.add_parser("list", help="List all notes.")
-    list_parser.add_argument("-c", "--category", type=str, default=None, help="List notes from a specific category.")
-    list_parser.add_argument("-i", "--importance", type=int, default=None,
-                             help="List notes with a specific importance level.")
-    list_parser.add_argument("-v", "--verbose", action="store_true",
-                             help="Show importance and timestamp with each note.")
-
-    mark_parser = subparsers.add_parser("mark", help="Mark a note as checked or unchecked.")
-    mark_parser.add_argument("id", type=int, help="The ID of the note to mark.")
-    mark_parser.add_argument("-u", "--uncheck", action="store_true", help="Unmark the note instead of marking it.")
-
-    delete_parser = subparsers.add_parser("delete", help="Delete a note.")
-    delete_parser.add_argument("id", type=int, help="The ID of the note to delete.")
-
-    clear_parser = subparsers.add_parser('clear', help='Clear all notes or notes in the specified category')
-    clear_parser.add_argument('-c', '--category', type=str, help='Category of notes to clear (optional)')
-
-    args = parser.parse_args()
-
-    if args.subcommand == "add":
-        category = args.category_keyword if args.category_keyword is not None else args.category
-        importance = args.importance_keyword if args.importance_keyword is not None else args.importance
-        create_note(args.note, category, importance)
-    elif args.subcommand == "list":
-        list_notes(args.category, args.importance, args.verbose)
-    elif args.subcommand == "mark":
-        mark_note(args.id, not args.uncheck)
-    elif args.subcommand == "delete":
-        delete_note(args.id)
-    elif args.subcommand == 'clear':
-        clear_notes(args.category)
-    elif args.subcommand == 'sub':
-        create_sub_note(args.note, args.parent_id, args.importance)
-    else:
-        parser.print_help()
-
-
-if __name__ == "__main__":
-    main()
+import json
+import argparse
+import os
+from datetime import datetime
+import textwrap
+
+
+NOTES_FILE = os.path.expanduser("~/.ti_notes.json")
+
+
+def save_notes(notes, max_id, last_category):
+    with open(NOTES_FILE, "w") as f:
+        json.dump({"notes": notes, "max_id": max_id, "last_category": last_category}, f, indent=2)
+
+
+def load_notes():
+    if not os.path.exists(NOTES_FILE):
+        return [], 0, "unknown"  # Return max_id as 0 for an empty file
+
+    with open(NOTES_FILE, "r") as f:
+        content = f.read().strip()
+        if not content:
+            return [], 0, "unknown"  # Return max_id as 0 for an empty file
+
+        data = json.loads(content)
+        notes, max_id, last_category = data.get("notes", []), data.get("max_id", 0), data.get("last_category",
+                                                                                              "unknown")
+        return notes, max_id, last_category
+
+
+def create_note(note, category, importance):
+    notes, max_id, last_category = load_notes()
+    category = last_category if category is None else category
+
+    new_id = max_id + 1
+
+    new_note = {
+        "id": new_id,  # Use the new ID
+        "note": note,
+        "category": category,
+        "importance": importance,
+        "created_timestamp": datetime.now().isoformat(),
+        "marked_timestamp": None,
+        "subs": [],
+        "checked": False,
+    }
+
+    notes.append(new_note)
+    save_notes(notes, new_id, category)  # Update max_id
+
+    print("Note added successfully.")
+
+
+def create_sub_note(note, parent_id, importance):
+    notes, max_id, last_category = load_notes()
+
+    for n in notes:
+        if n["id"] == parent_id:
+            parent_note = n
+            break
+    else:
+        print("Parent does not exist.")
+        return
+
+    new_id = max_id + 1
+
+    new_note = {
+        "id": new_id,  # Use the new ID
+        "parent": parent_id,
+        "note": note,
+        "category": parent_note["category"],
+        "importance": importance,
+        "created_timestamp": datetime.now().isoformat(),
+        "marked_timestamp": None,
+        "checked": False,
+    }
+
+    try:
+        parent_note["subs"].append(new_note)
+    except KeyError:
+        parent_note["subs"] = [new_note]
+
+    save_notes(notes, new_id, last_category)
+
+    print("Sub-note added successfully.")
+
+
+def format_note(note_text, sub=False):
+    bullet_indent = "\t\t" if sub else "\t"
+    lines = note_text.split("*")
+    formatted_lines = [lines[0]] + [f"{bullet_indent}* {line.strip()}" for line in lines[1:]]
+    return "\n".join(formatted_lines)
+
+
+def list_notes(category=None, importance=None, verbose=None):
+    notes, _, _ = load_notes()
+
+    if not category:
+        sorted_notes = sorted(notes, key=lambda x: x['category'])
+    else:
+        sorted_notes = [note for note in notes if note['category'] == category]
+
+    def display_notes(notes_list, indent=0):
+        for note in notes_list:
+            if importance and note["importance"] != importance:
+                continue
+
+            checked_symbol = "✔" if note["checked"] else "✘"
+            importance_symbol = f"[{note['importance']}]" if note["importance"] is not None and verbose else ""
+            created_timestamp = f'(Created {note["created_timestamp"]})' if verbose else ""
+            marked_timestamp = f'(Mark Updated {note["marked_timestamp"]})' if verbose and note["marked_timestamp"] is not None else ""
+
+            lines = textwrap.wrap(note['note'], width=80 - indent)
+            first_line = lines.pop(0)
+
+            print(
+                f"{indent * ' '}{checked_symbol} {note['id']} {first_line} "
+                f"{importance_symbol} {created_timestamp} {marked_timestamp}"
+            )
+
+            for line in lines:
+                print(f"{indent * ' '}   {line}")
+
+            try:
+                if note["subs"]:
+                    display_notes(note["subs"], indent + 4)
+            except KeyError:
+                pass
+
+    grouped_notes = {}
+    for note in sorted_notes:
+        grouped_notes.setdefault(note['category'], []).append(note)
+
+    for category, cat_notes in grouped_notes.items():
+        print(f"\n{category.upper()}{'-' * (80 - len(category))}")
+        display_notes(cat_notes)
+
+
+def mark_note(note_id, checked=True):
+    notes, max_id, last_category = load_notes()
+
+    for note in notes:
+        if note["id"] == note_id:
+            note["checked"] = checked
+            note["marked_timestamp"] = datetime.now().isoformat()
+            save_notes(notes, max_id, last_category)
+            print(f"Note {'marked' if checked else 'unmarked'} successfully.")
+            return
+
+        for index, sub in enumerate(note["subs"]):
+            if sub["id"] == note_id:
+                sub["checked"] = checked
+                note["marked_timestamp"] = datetime.now().isoformat()
+                save_notes(notes, max_id, last_category)
+                print(f"Note {'marked' if checked else 'unmarked'} successfully.")
+                return
+    else:
+        print("Invalid note ID.")
+
+
+def delete_note(note_id):
+    notes, max_id, last_category = load_notes()
+
+    for index, note in enumerate(notes):
+        if note["id"] == note_id:
+            del notes[index]
+            save_notes(notes, max_id, last_category)
+            print("Note deleted successfully.")
+            return
+
+        for sub_index, sub in enumerate(note["subs"]):
+            if sub["id"] == note_id:
+                del note["subs"][sub_index]
+                save_notes(notes, max_id, last_category)
+                print("Note deleted successfully.")
+                return
+    else:
+        print("Invalid note ID.")
+
+
+def clear_notes(category=None):
+    notes, max_id, last_category = load_notes()
+    if category:
+        notes = [note for note in notes if note['category'] != category]
+    else:
+        notes = []
+
+    save_notes(notes, max_id, last_category)
+    if category:
+        print(f"Successfully cleared all notes in category '{category}'.")
+    else:
+        print("Successfully cleared all notes.")
+
+
+def main():
+    parser = argparse.ArgumentParser(description="A command-line tool for taking quick notes.", prog="ti")
+    subparsers = parser.add_subparsers(dest="subcommand")
+
+    # Add subparser for 'add' command
+    add_parser = subparsers.add_parser("add", help="Add a new note.")
+    add_parser.add_argument("note", type=str, help="The content of the note.")
+    add_parser.add_argument("category", type=str, nargs="?", default=None,
+                            help="Optional category for the note. If none is provided, the last category will be used.")
+    add_parser.add_argument("importance", type=int, nargs="?", default=None,
+                            help="Optional importance level for the note (integer).")
+    add_parser.add_argument("-c", "--category", type=str, default=None,
+                            help="Optional category for the note. If none is provided, the last category will be used.",
+                            dest="category_keyword")
+    add_parser.add_argument("-i", "--importance", type=int, default=None,
+                            help="Optional importance level for the note (integer).", dest="importance_keyword")
+
+    sub_parser = subparsers.add_parser('sub', help='Add a sub-note to a note')
+    sub_parser.add_argument('parent_id', type=int, help='Parent note ID')
+    sub_parser.add_argument('note', type=str, help='Sub-note text')
+    sub_parser.add_argument("-i", "--importance", type=int, default=None,
+                            help="Optional importance level for the note (integer).")
+
+    # Add subparser for 'list' command
+    list_parser = subparsers.add_parser("list", help="List all notes.")
+    list_parser.add_argument("-c", "--category", type=str, default=None, help="List notes from a specific category.")
+    list_parser.add_argument("-i", "--importance", type=int, default=None,
+                             help="List notes with a specific importance level.")
+    list_parser.add_argument("-v", "--verbose", action="store_true",
+                             help="Show importance and timestamp with each note.")
+
+    mark_parser = subparsers.add_parser("mark", help="Mark a note as checked or unchecked.")
+    mark_parser.add_argument("id", type=int, help="The ID of the note to mark.")
+    mark_parser.add_argument("-u", "--uncheck", action="store_true", help="Unmark the note instead of marking it.")
+
+    delete_parser = subparsers.add_parser("delete", help="Delete a note.")
+    delete_parser.add_argument("id", type=int, help="The ID of the note to delete.")
+
+    clear_parser = subparsers.add_parser('clear', help='Clear all notes or notes in the specified category')
+    clear_parser.add_argument('-c', '--category', type=str, help='Category of notes to clear (optional)')
+
+    args = parser.parse_args()
+
+    if args.subcommand == "add":
+        category = args.category_keyword if args.category_keyword is not None else args.category
+        importance = args.importance_keyword if args.importance_keyword is not None else args.importance
+        create_note(args.note, category, importance)
+    elif args.subcommand == "list":
+        list_notes(args.category, args.importance, args.verbose)
+    elif args.subcommand == "mark":
+        mark_note(args.id, not args.uncheck)
+    elif args.subcommand == "delete":
+        delete_note(args.id)
+    elif args.subcommand == 'clear':
+        clear_notes(args.category)
+    elif args.subcommand == 'sub':
+        create_sub_note(args.note, args.parent_id, args.importance)
+    else:
+        parser.print_help()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `tinote-1.1.0/tinote/update.py` & `tinote-1.1.1/tinote/update.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import json
-import os
-from tinote import main
-
-
-def update(final_version):
-    data_file = main.NOTES_FILE
-
-    # Check if the data file exists
-    if not os.path.exists(data_file):
-        return
-
-    # Load the user's data file
-    with open(data_file, 'r') as f:
-        data = json.load(f)
-
-    # Get the current version from the data
-    current_version = data.get("version", "1.0.x")
-
-    # Define a dictionary of update actions keyed by the version they should be applied to
-    update_actions = [
-        ("1.1.0", update_1_0_x_to_1_1_x)
-    ]
-
-    # Apply the update actions in order
-    for version, update_action in update_actions:
-        if current_version < version:
-            print(f"Updating user data file from {current_version} to {version}")
-            data = update_action(data)
-            current_version = version
-
-    # Update the data version and save the updated data
-    data["version"] = final_version
-    with open(data_file, 'w') as f:
-        json.dump(data, f, indent=2)
-
-
-def update_1_0_x_to_1_1_x(data):
-    notes, _, _ = data.get("notes", []), data.get("max_id", 0), data.get("last_category", "unknown")
-
-    for note in notes:
-        try:
-            note["created_timestamp"] = note["timestamp"]
-            note["marked_timestamp"] = None
-            note["subs"] = [] if "subs" not in note.keys() else note["subs"]
-
-            del note["timestamp"]
-        except KeyError:
-            pass
-
-    return data
+import json
+import os
+from tinote import main
+
+
+def update(final_version):
+    data_file = main.NOTES_FILE
+
+    # Check if the data file exists
+    if not os.path.exists(data_file):
+        return
+
+    # Load the user's data file
+    with open(data_file, 'r') as f:
+        data = json.load(f)
+
+    # Get the current version from the data
+    current_version = data.get("version", "1.0.x")
+
+    # Define a dictionary of update actions keyed by the version they should be applied to
+    update_actions = [
+        ("1.1.0", update_1_0_x_to_1_1_x)
+    ]
+
+    # Apply the update actions in order
+    for version, update_action in update_actions:
+        if current_version < version:
+            print(f"Updating user data file from {current_version} to {version}")
+            data = update_action(data)
+            current_version = version
+
+    # Update the data version and save the updated data
+    data["version"] = final_version
+    with open(data_file, 'w') as f:
+        json.dump(data, f, indent=2)
+
+
+def update_1_0_x_to_1_1_x(data):
+    notes = data.get("notes", [])
+
+    for note in notes:
+        try:
+            note["created_timestamp"] = note["timestamp"]
+            note["marked_timestamp"] = None
+            note["subs"] = [] if "subs" not in note.keys() else note["subs"]
+
+            del note["timestamp"]
+        except KeyError:
+            pass
+
+    return data
```

### Comparing `tinote-1.1.0/tinote.egg-info/PKG-INFO` & `tinote-1.1.1/tinote.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-Metadata-Version: 2.1
-Name: tinote
-Version: 1.1.0
-Summary: A command-line note-taking tool
-Home-page: https://github.com/aPeter1/tinote
-Author: Alec Petersen
-Author-email: k.alecpetersen@gmail.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Terminals
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# Tinote
-
-Tinote is a lightweight command-line note-taking tool, designed for quick and easy note management. Keep track of your thoughts, ideas, or reminders directly from the terminal.
-
-## Installation
-
-Install Tinote using pip:
-
-```bash
-pip install tinote
-```
-
-## Usage
-
-Create a new note (if no category is provided, the last category will be used):
-
-```bash
-ti add "a note to remember" <optional category> <optional importance>
-```
-
-List all notes (verbose list will include importance and timestamp):
-
-```bash
-ti list [-v]
-```
-
-List notes with filters (category or importance):
-
-```bash
-ti list -c <category> -i <importance>
-```
-
-Add a sub-note to a note (currently only supports one level)
-
-```bash
-ti sub <parent_id> "Text of your sub-note" -i <importance>
-```
-
-Mark a note as checked/unchecked:
-
-```bash
-ti mark <note_id>
-```
-
-Delete a note:
-
-```bash
-ti delete <note_id>
-```
-
-Clear all notes or notes within a specified category:
-
-```bash
-ti clear
-ti clear -c <category>
-```
-
-## Features
-
-- Create and manage notes with optional categories and importance levels
-- List notes, with optional filters for categories and importance
-- Easily mark notes as checked/unchecked
-- Delete notes using their ID
-- Clear all notes or notes within a specified category
-- Automatically saves notes to a local JSON file for persistence
-
-## License
-
-MIT License
+Metadata-Version: 2.1
+Name: tinote
+Version: 1.1.1
+Summary: A command-line note-taking tool
+Home-page: https://github.com/aPeter1/tinote
+Author: Alec Petersen
+Author-email: k.alecpetersen@gmail.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Terminals
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+![Logo](assets/color-logo-no-background.png)
+
+Tinote is a lightweight command-line note-taking tool, designed for quick and easy note management. Keep track of your thoughts, ideas, or reminders directly from the terminal.
+
+## Installation
+
+Install Tinote using pip:
+
+```bash
+pip install tinote
+```
+
+## Usage
+
+Create a new note (if no category is provided, the last category will be used):
+
+```bash
+ti add "a note to remember" <optional category> <optional importance>
+```
+
+List all notes (verbose list will include importance and timestamp):
+
+```bash
+ti list [-v]
+```
+
+List notes with filters (category or importance):
+
+```bash
+ti list -c <category> -i <importance>
+```
+
+Add a sub-note to a note (currently only supports one level)
+
+```bash
+ti sub <parent_id> "Text of your sub-note" -i <importance>
+```
+
+Mark a note as checked/unchecked:
+
+```bash
+ti mark <note_id>
+```
+
+Delete a note:
+
+```bash
+ti delete <note_id>
+```
+
+Clear all notes or notes within a specified category:
+
+```bash
+ti clear
+ti clear -c <category>
+```
+
+## Features
+
+- Create and manage notes with optional categories and importance levels
+- List notes, with optional filters for categories and importance
+- Easily mark notes as checked/unchecked
+- Delete notes using their ID
+- Clear all notes or notes within a specified category
+- Automatically saves notes to a local JSON file for persistence
+
+## License
+
+MIT License
```

