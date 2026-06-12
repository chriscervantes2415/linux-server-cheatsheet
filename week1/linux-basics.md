# Week 1 - Linux Fundamentals

## Linux Filesystem

### Important directories

| Directory | Purpose |
|------------|---------|
| `/home` | User files |
| `/etc` | Configuration files |
| `/var/log` | Logs |
| `/root` | Root user home |
| `/tmp` | Temporary files |

---

## Users and Groups

### Check current user

```bash
whoami
```

### Check groups

```bash
groups
```

### Check user details

```bash
id
```

---

## Permissions

### View permissions

```bash
ls -l
```

Example:

```text
-rwxr-xr-x
```

Meaning:

- owner → rwx
- group → r-x
- others → r-x

### Common permissions

```text
755 = rwxr-xr-x
644 = rw-r--r--
777 = rwxrwxrwx (unsafe)
```

### Make file executable

```bash
chmod +x deploy.sh
```

### Change ownership

```bash
sudo chown user:group file
```
