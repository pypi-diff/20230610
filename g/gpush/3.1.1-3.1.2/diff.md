# Comparing `tmp/gpush-3.1.1.tar.gz` & `tmp/gpush-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpush-3.1.1.tar", last modified: Sun Apr 23 12:32:35 2023, max compression
+gzip compressed data, was "gpush-3.1.2.tar", last modified: Sat Jun 10 19:18:34 2023, max compression
```

## Comparing `gpush-3.1.1.tar` & `gpush-3.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:32:35.185988 gpush-3.1.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-23 12:32:30.000000 gpush-3.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1718 2023-04-23 12:32:35.185988 gpush-3.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1606 2023-04-23 12:32:30.000000 gpush-3.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-23 12:32:32.000000 gpush-3.1.1/_version.py
--rw-r--r--   0 root         (0) root         (0)     4220 2023-04-23 12:32:35.000000 gpush-3.1.1/gpush
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:32:35.185988 gpush-3.1.1/gpush.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1718 2023-04-23 12:32:35.000000 gpush-3.1.1/gpush.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2023-04-23 12:32:35.000000 gpush-3.1.1/gpush.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 12:32:35.000000 gpush-3.1.1/gpush.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2023-04-23 12:32:35.000000 gpush-3.1.1/gpush.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-23 12:32:35.000000 gpush-3.1.1/gpush.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)     4220 2023-04-23 12:32:30.000000 gpush-3.1.1/gpush.py
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-23 12:32:30.000000 gpush-3.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 12:32:35.185988 gpush-3.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      774 2023-04-23 12:32:30.000000 gpush-3.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 19:18:34.767153 gpush-3.1.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-10 19:18:32.000000 gpush-3.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3432 2023-06-10 19:18:34.767153 gpush-3.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3320 2023-06-10 19:18:32.000000 gpush-3.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-10 19:18:32.000000 gpush-3.1.2/_version.py
+-rw-r--r--   0 root         (0) root         (0)     5296 2023-06-10 19:18:34.000000 gpush-3.1.2/gpush
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 19:18:34.767153 gpush-3.1.2/gpush.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3432 2023-06-10 19:18:34.000000 gpush-3.1.2/gpush.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2023-06-10 19:18:34.000000 gpush-3.1.2/gpush.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 19:18:34.000000 gpush-3.1.2/gpush.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-06-10 19:18:34.000000 gpush-3.1.2/gpush.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-10 19:18:34.000000 gpush-3.1.2/gpush.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)     5296 2023-06-10 19:18:32.000000 gpush-3.1.2/gpush.py
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-10 19:18:32.000000 gpush-3.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-10 19:18:34.767153 gpush-3.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      773 2023-06-10 19:18:32.000000 gpush-3.1.2/setup.py
```

### Comparing `gpush-3.1.1/LICENSE` & `gpush-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpush-3.1.1/gpush` & `gpush-3.1.2/gpush`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 #!/usr/bin/env python3
 
 """
-Python script to handle git commit and push to standardise commit messages using conventional commit
-messages.
+Python script to handle git commit and push commit messages using conventional commit messages.
 
 Usage: gpush.py
 """
 
 import argparse
+import logging
+import sys
 
 import inquirer
 from git import Repo
+from git.exc import GitError
 
 from _version import __version__
 
 VERSION = __version__
 
+# Setup logging
+
+
+logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
+
 parser = argparse.ArgumentParser(
     prog="gpush " + VERSION,
     description="Git commit helper for conventional commit messages",
 )
 parser.add_argument(
     "--version", action="store_true", help="Option to print the current version only"
 )
@@ -47,118 +54,149 @@
 
 
 args = parser.parse_args()
 
 
 def get_version():
     """
-    Function to return the current version of gpush.py
+    Return the current version of gpush.py.
 
-    :return: String containing the current version of gpush.py
+    Returns:
+        String: Current version of gpush.py
     """
     return VERSION
 
 
 def git_commit(commit_message):
     """
-    Function to commit changes to Git on the current branch for the repository
-    :param commit_message: String containing the conventional commit message formatted commit
-    message
-    :return: True/False
+    Commit changes to Git on the current branch for the repository.
+
+    Args:
+        commit_message: String containing the conventional commit message formatted commit message
+
+    Raises:
+        GitError: If there is an issue with the call to git
+
+    Returns:
+        True if commit is successful
     """
     try:
         repo = Repo(search_parent_directories=True)
         repo.index.write()
         repo.git.commit("-m" + commit_message)
-        print("committing: " + commit_message)
-        print("Committed successfully")
-    except Exception as error_message:
-        print("Some error occured while committing the code:")
-        print(str(error_message))
+        logging.info("committing: %s", commit_message)
+        logging.info("Committed successfully")
+    except GitError as error_message:
+        logging.info("Some error occured while committing the code:")
+        logging.info(str(error_message))
         raise
 
     return True
 
 
 def git_push():
     """
-    Function to push commit up to Git on the current branch for the repository
+    Push commit up to Git on the current branch for the repository.
 
-    :return: True/False
+    Raises:
+        GitError: If there is an issue with the call to git
+        Exception: If there is some other issue
+
+    Returns:
+        True if push is successful
     """
     try:
         if str(args.branch) != "current":
             branch_name = str(args.branch)
         else:
             repo = Repo(search_parent_directories=True)
             branch_name = repo.active_branch
         repo = Repo(search_parent_directories=True)
         repo.create_head(branch_name)
         repo.git.push("--set-upstream", "origin", branch_name)
-        print("Pushed successfully")
+        logging.info("Pushed successfully")
+    except GitError as error_message:
+        logging.info("Some error occurred while pushing the code:")
+        logging.info(str(error_message))
+        raise GitError from error_message
     except Exception as error_message:
-        print("Some error occurred while pushing the code:")
-        print(str(error_message))
-        raise
+        logging.info("Some error occurred while pushing the code:")
+        logging.info(str(error_message))
+        raise Exception from error_message
 
     return True
 
 
 def collect_details():
     """
-    Function that collects commit message detail from the committer and executes git commit
-    and push.
+    Collect commit message detail from the committer and executes git commit and push.
+
+    Raises:
+        KeyboardInterrupt: If user exits the script
 
-    :return: True/False
+    Returns:
+        commit_message_final: String containing the conventional commit message.
     """
-    questions = [
-        inquirer.List(
-            "type",
-            message="What type of commit is this?",
-            choices=["fix", "feat", "docs", "ci"],
-        ),
-        inquirer.List(
-            "breaking_change",
-            message="Does the commit include breaking changes?",
-            choices=["Yes", "No"],
-        ),
-        inquirer.Text("commit_message", message="What's your commit message"),
-    ]
+    try:
+        questions = [
+            inquirer.List(
+                "type",
+                message="What type of commit is this?",
+                choices=["fix", "feat", "docs", "ci"],
+            ),
+            inquirer.List(
+                "breaking_change",
+                message="Does the commit include breaking changes?",
+                choices=["Yes", "No"],
+            ),
+            inquirer.Text(
+                "commit_message",
+                message="What's your commit message",
+            ),
+        ]
+        answers = inquirer.prompt(questions, raise_keyboard_interrupt=True)
+    except KeyboardInterrupt as error_message:
+        raise KeyboardInterrupt from error_message
 
-    answers = inquirer.prompt(questions)
     if answers["breaking_change"] == "Yes":
         is_breaking_change = "!"
     else:
         is_breaking_change = ""
 
     commit_message_final = (
         answers["type"] + is_breaking_change + ": " + answers["commit_message"]
     )
+
     return commit_message_final
 
 
 def main():
     """
-    Main function to execute the script
-    :return:
+    Execute the script.
+
+    Returns:
+        True
     """
     if args.version:
-        print(get_version())
+        logging.info(get_version())
     else:
         try:
             if args.no_commit:
                 if str(args.message) != "None":
                     commit_message = args.message
                 else:
                     commit_message = collect_details()
                 git_commit(commit_message)
             if args.no_push:
                 git_push()
         except Exception as error_message:
-            print("Some error occurred while pushing the code:")
-            print(str(error_message))
-            raise
+            logging.info("Some error occurred while pushing the code:")
+            logging.info(str(error_message))
+            sys.exit(1)
+        except KeyboardInterrupt:
+            logging.info("Okay! Bye!")
+            sys.exit(0)
     return True
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gpush-3.1.1/gpush.py` & `gpush-3.1.2/gpush.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 #!/usr/bin/env python3
 
 """
-Python script to handle git commit and push to standardise commit messages using conventional commit
-messages.
+Python script to handle git commit and push commit messages using conventional commit messages.
 
 Usage: gpush.py
 """
 
 import argparse
+import logging
+import sys
 
 import inquirer
 from git import Repo
+from git.exc import GitError
 
 from _version import __version__
 
 VERSION = __version__
 
+# Setup logging
+
+
+logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
+
 parser = argparse.ArgumentParser(
     prog="gpush " + VERSION,
     description="Git commit helper for conventional commit messages",
 )
 parser.add_argument(
     "--version", action="store_true", help="Option to print the current version only"
 )
@@ -47,118 +54,149 @@
 
 
 args = parser.parse_args()
 
 
 def get_version():
     """
-    Function to return the current version of gpush.py
+    Return the current version of gpush.py.
 
-    :return: String containing the current version of gpush.py
+    Returns:
+        String: Current version of gpush.py
     """
     return VERSION
 
 
 def git_commit(commit_message):
     """
-    Function to commit changes to Git on the current branch for the repository
-    :param commit_message: String containing the conventional commit message formatted commit
-    message
-    :return: True/False
+    Commit changes to Git on the current branch for the repository.
+
+    Args:
+        commit_message: String containing the conventional commit message formatted commit message
+
+    Raises:
+        GitError: If there is an issue with the call to git
+
+    Returns:
+        True if commit is successful
     """
     try:
         repo = Repo(search_parent_directories=True)
         repo.index.write()
         repo.git.commit("-m" + commit_message)
-        print("committing: " + commit_message)
-        print("Committed successfully")
-    except Exception as error_message:
-        print("Some error occured while committing the code:")
-        print(str(error_message))
+        logging.info("committing: %s", commit_message)
+        logging.info("Committed successfully")
+    except GitError as error_message:
+        logging.info("Some error occured while committing the code:")
+        logging.info(str(error_message))
         raise
 
     return True
 
 
 def git_push():
     """
-    Function to push commit up to Git on the current branch for the repository
+    Push commit up to Git on the current branch for the repository.
 
-    :return: True/False
+    Raises:
+        GitError: If there is an issue with the call to git
+        Exception: If there is some other issue
+
+    Returns:
+        True if push is successful
     """
     try:
         if str(args.branch) != "current":
             branch_name = str(args.branch)
         else:
             repo = Repo(search_parent_directories=True)
             branch_name = repo.active_branch
         repo = Repo(search_parent_directories=True)
         repo.create_head(branch_name)
         repo.git.push("--set-upstream", "origin", branch_name)
-        print("Pushed successfully")
+        logging.info("Pushed successfully")
+    except GitError as error_message:
+        logging.info("Some error occurred while pushing the code:")
+        logging.info(str(error_message))
+        raise GitError from error_message
     except Exception as error_message:
-        print("Some error occurred while pushing the code:")
-        print(str(error_message))
-        raise
+        logging.info("Some error occurred while pushing the code:")
+        logging.info(str(error_message))
+        raise Exception from error_message
 
     return True
 
 
 def collect_details():
     """
-    Function that collects commit message detail from the committer and executes git commit
-    and push.
+    Collect commit message detail from the committer and executes git commit and push.
+
+    Raises:
+        KeyboardInterrupt: If user exits the script
 
-    :return: True/False
+    Returns:
+        commit_message_final: String containing the conventional commit message.
     """
-    questions = [
-        inquirer.List(
-            "type",
-            message="What type of commit is this?",
-            choices=["fix", "feat", "docs", "ci"],
-        ),
-        inquirer.List(
-            "breaking_change",
-            message="Does the commit include breaking changes?",
-            choices=["Yes", "No"],
-        ),
-        inquirer.Text("commit_message", message="What's your commit message"),
-    ]
+    try:
+        questions = [
+            inquirer.List(
+                "type",
+                message="What type of commit is this?",
+                choices=["fix", "feat", "docs", "ci"],
+            ),
+            inquirer.List(
+                "breaking_change",
+                message="Does the commit include breaking changes?",
+                choices=["Yes", "No"],
+            ),
+            inquirer.Text(
+                "commit_message",
+                message="What's your commit message",
+            ),
+        ]
+        answers = inquirer.prompt(questions, raise_keyboard_interrupt=True)
+    except KeyboardInterrupt as error_message:
+        raise KeyboardInterrupt from error_message
 
-    answers = inquirer.prompt(questions)
     if answers["breaking_change"] == "Yes":
         is_breaking_change = "!"
     else:
         is_breaking_change = ""
 
     commit_message_final = (
         answers["type"] + is_breaking_change + ": " + answers["commit_message"]
     )
+
     return commit_message_final
 
 
 def main():
     """
-    Main function to execute the script
-    :return:
+    Execute the script.
+
+    Returns:
+        True
     """
     if args.version:
-        print(get_version())
+        logging.info(get_version())
     else:
         try:
             if args.no_commit:
                 if str(args.message) != "None":
                     commit_message = args.message
                 else:
                     commit_message = collect_details()
                 git_commit(commit_message)
             if args.no_push:
                 git_push()
         except Exception as error_message:
-            print("Some error occurred while pushing the code:")
-            print(str(error_message))
-            raise
+            logging.info("Some error occurred while pushing the code:")
+            logging.info(str(error_message))
+            sys.exit(1)
+        except KeyboardInterrupt:
+            logging.info("Okay! Bye!")
+            sys.exit(0)
     return True
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gpush-3.1.1/setup.py` & `gpush-3.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Setup file for python-semantic-versioning
-"""
+"""Setup file for python-semantic-versioning."""
 from setuptools import setup
 
 from _version import __version__
 
 with open("README.md", encoding="UTF-8") as readme_file:
     readme_contents = readme_file.read()
```

