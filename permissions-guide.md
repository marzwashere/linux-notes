# Linux File Permissions Reference

A quick breakdown of how file ownership and permissions work in Linux.

## 1. The Core Commands
* `chmod`: Changes file or directory access permissions.
* `chown`: Changes the user and group ownership of a file or directory.

## 2. Understanding Octal Notation (chmod)
Permissions are represented by three digits (Owner, Group, Others), where each digit is a sum of:
* **4** = Read (r)
* **2** = Write (w)
* **1** = Execute (x)

*Example:* `chmod 755 script.sh`
* **7** (4+2+1): Owner has Read, Write, and Execute.
* **5** (4+0+1): Group has Read and Execute.
* **5** (4+0+1): Others have Read and Execute.

## 3. Quick Troubleshooting
* **Symptom:** `Permission denied` when trying to run a script.
* **Fix:** Grant execution rights using `chmod +x filename` or `chmod 755 filename`.

## 4. Troubleshooting: Missing `chmod` / `coreutils`
* **Symptom:** Running `chmod` returns `Command 'chmod' not found`.
* **Cause:** The core system utilities package (`coreutils`) may be missing in a minimal environment.
* **Fix:** Install the package via apt:
* **Verification:** Confirm the binary location and version:
