# Linux CLI Fundamentals & Filesystem Architecture (WADF Module 1, Week 1)
**Course:** WADF-2026 – Web Application & Digital Forensics Fundamentals  
**Student Name:** Kenneth Ukata  
**Registration Number:** FCDF2617034  
**Environment:** Debian Linux (Kali Linux `kali@KENNETH`)  

---

## 📌 Lab Overview
This repository contains terminal logs, command research, and documentation for **WADF Module 1 (Week 01)**. The objective of this lab exercise was to master foundational Linux Command Line Interface (CLI) operations, explore native help utilities (`man`, `help`, `apropos`), analyze exit statuses, navigate relative/absolute paths, and audit core Linux Filesystem Hierarchy Standard (FHS) directories.

---

## 🛠️ Utilities & Concepts Coverered
* **CLI Orientation & Baseline:** Environment identification (`whoami`, `hostname`, `uname -r`), release verification (`/etc/os-release`), and disk space usage (`df -h`).
* **Command Research & Help Systems:** Querying utility flags and manuals for `ls`, `cd`, `tar`, and `pwd`.
* **Path Navigation & Sandbox Management:** Navigating parent (`..`) and child directories, relative vs. absolute paths, and standard file operations (`mkdir`, `touch`, `cp`, `mv`, `rm`).
* **Filesystem Hierarchy Standard (FHS):** Inspecting system directories (`/`, `/etc`, `/var`, `/home`, `/tmp`, `/usr`).

---

## 📂 Command Research Summary

| Command | Help Method Used | Documented Flag / Option 1 | Documented Flag / Option 2 |
| :--- | :--- | :--- | :--- |
| **`ls`** | `ls --help` | `-a` (Do not ignore entries starting with `.`) | `-h` (With `-l`, print human readable sizes) |
| **`cd`** | `help cd` | `-P` (Use the physical directory structure) | `-L` (Force symbolic links) |
| **`tar`** | `apropos archive` / `man tar` | `-c` (Create a new archive) | `-x` (Extract files from an archive) |
| **`pwd`** | `man pwd` | `-L` (Print `$PWD` if it names current directory) | `-P` (Avoid all symlinks and print physical path) |

---

## 🏗️ Filesystem Architecture (FHS) Analysis

* **`/` (Root):** The absolute foundational point of the entire Linux hierarchical filesystem directory tree.
* **`/etc`:** Holds core host-specific system configuration files, startup scripts, and administration settings.
* **`/var`:** Stores variable data files that dynamically change during system operation (log metrics, spool directories, temporary locks).
* **`/home`:** Contains individual user personal storage directories, application preferences, and private documents.
* **`/tmp`:** Global temporary scratch space accessible by all users for short-lived operational files, protected by sticky security permissions.
* **`/usr`:** Houses user utilities, core shared libraries, read-only system binaries, and program documentation resources.

---

## 💡 Key Takeaway & Reflection
> *"This lab reinforced that with patience and systematic practice, complex terminal operations can be understood, controlled, and mastered. Beyond learning how to check exit statuses or navigate relative paths, it built foundational confidence in facing CLI technical hurdles without panic."*
