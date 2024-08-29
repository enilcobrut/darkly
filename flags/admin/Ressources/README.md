# Penetration Testing Report: Localhost Web Enumeration

## Overview

with goeboster we found two suspicious pages were discovered using `GoBuster`, a tool for brute-forcing URLs and directories on a web server. Additionally, a password hash was identified, which was found to correspond to the password `qwerty@`.

### Discovered Pages

1. **Admin Page**: `localhost:8080/admin`
2. **Whatever Page**: `localhost:8080/whatever`

### Discovered Password Hash

- **Hash**: Corresponding password found to be `qwerty@`

## Steps to Reproduce

### 1. Using GoBuster to Discover Hidden Pages

To find hidden or potentially sensitive directories on the server, we used `GoBuster` with the following command:

```bash
gobuster dir -u http://localhost:8080 -w /path/to/wordlist.txt
