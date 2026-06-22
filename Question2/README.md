# Question 2 - Secure Project Workspace Setup

## Objective

Create a secure project workspace and configure appropriate file permissions.

---

## Command 1: Check Umask Value

### Command

```bash
umask
```

### Observation

This command displays the default permission mask used when new files and directories are created. The umask value determines which permissions are removed from newly created objects. Understanding the umask helps in managing file security. It provides insight into the default access control settings of the system.

---

## Command 2: Create Project Workspace Structure

### Command

```bash
mkdir -p ProjectWorkspace/docs ProjectWorkspace/src ProjectWorkspace/reports
```

### Observation

This command creates the project workspace along with the required subdirectories. The `-p` option allows parent directories to be created automatically if they do not already exist. A structured directory layout helps organize project files efficiently. It also improves project management and accessibility.

---

## Command 3: Display Directory Structure

### Command

```bash
ls -R ProjectWorkspace
```

### Observation

This command recursively lists all directories and files within the project workspace. It helps verify that the required folder structure has been created successfully. The output confirms the presence of the docs, src, and reports directories. This serves as validation of the workspace setup.

---

## Command 4: Check File Permissions Before Modification

### Command

```bash
ls -l ProjectWorkspace/docs
```

### Observation

This command displays file permissions in long format before any modifications are made. The output shows the default permissions assigned by the operating system. Reviewing these permissions helps establish a baseline for comparison. It is useful for understanding how permission changes affect file security.

---

## Command 5: Modify File Permissions

### Command

```bash
chmod 600 ProjectWorkspace/docs/project_plan.txt
```

### Observation

This command changes the file permissions to 600. The owner receives read and write permissions, while all permissions for group members and other users are removed. Restricting access in this way improves data security. It ensures that only the file owner can view or modify the file.

---

## Command 6: Verify Permissions After Modification

### Command

```bash
ls -l ProjectWorkspace/docs
```

### Observation

This command verifies that the permission changes were applied successfully. The output should show permission settings corresponding to mode 600. Comparing the output before and after modification demonstrates the effect of the chmod command. This confirms that access restrictions are now in place.

---

## Command 7: Check Ownership Details

### Command

```bash
stat ProjectWorkspace/docs/project_plan.txt
```

### Observation

This command provides detailed information about the file, including ownership, permissions, size, and timestamps. The output identifies the owner and group associated with the file. Ownership information is important for permission management and security administration. It confirms which user has control over the file.

---

## Security Explanation

File permissions help protect project data from unauthorized access and modification. Setting permissions to 600 ensures that only the file owner can read and modify the file. Other users on the system cannot access the contents. Combined with proper ownership management, these controls improve the security of sensitive project documents.

## Files Included

* Project_Workspace_Report.txt
* Screenshots of command execution
