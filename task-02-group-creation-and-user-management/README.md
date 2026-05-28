# Task 2 - Group Creation and User Assignment

## Task Statement

The system admin team has streamlined access management by implementing group-based access control.

### Requirements
- Create a group named `developers`
- Perform the task on all App Servers
- Add user `stark` to the group
- Create the user if it does not already exist

---

## Solution

### Step 1: Create the Group

```bash
sudo groupadd developers
```

### Step 2: Create User `stark` (if Not exists)

```bash
id stark || sudo useradd stark
```

### Step 3: Add User to the Group

```bash
sudo usermod -aG developers stark
```

### Step 4: Verify Group Membership

```bash
id stark
```

# Expected Output:

```bash
uid=1001(stark) gid=1001(stark) groups=1001(stark),developers
```

# Task completed successfully 🚀

## Skills Learned:
- Linux Group Management
- Group-Based Access Control (GBAC)
- User Creation and Management
- Adding Users to Groups
- Linux Access Administration