# Question 1 - Linux Environment Verification

## Objective
Verify the Linux environment and user account details using Linux commands.

## Commands Executed

### 1. Check Username

Command:
```bash
whoami
```

Output:
```text
chand
```

Observation:
This command displays the currently logged-in user. The output confirms that the active user is `chand`.

---

### 2. Check User Groups

Command:
```bash
groups
```

Output:
```text
chand adm cdrom sudo dip plugdev users
```

Observation:
This command displays all groups associated with the current user account. The user belongs to administrative and device access groups.

---

### 3. Check Current Shell

Command:
```bash
echo $SHELL
```

Output:
```text
/bin/bash
```

Observation:
This command displays the default shell being used. The output shows that the Bash shell is active.

---

### 4. Check Current Working Directory

Command:
```bash
pwd
```

Output:
```text
/home/chand
```

Observation:
This command prints the current working directory. The user is currently working inside the home directory.

---

### 5. List Files and Directories

Command:
```bash
ls -la
```

Observation:
This command lists all files and directories, including hidden files. The output shows configuration files such as `.bashrc`, `.profile`, and `.cache`.

---

### 6. Verify Network Connectivity

Command:
```bash
ping -c 4 google.com
```

Observation:
This command sends four ICMP packets to Google. All packets were received successfully with 0% packet loss, confirming network connectivity.

## Files Included

- Environment_Report.txt
- Screenshots of command execution
