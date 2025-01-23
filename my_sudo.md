---
status: in progress
---

## Tasks
- [ ] Initial Setup & Core Structure:
    - [x] Create a Makefile with required rules (re, clean, fclean) ✅ 2025-01-21
    - [x] Set up the basic program structure with argument parsing ✅ 2025-01-21
    - [x] Implement the -h help display functionality ✅ 2025-01-21
    - [ ] Set up error handling (exit code 84 for errors)
- [ ] Sudoers File Parsing:
    - [x] Create functions to read and parse /etc/sudoers file ✅ 2025-01-21
    - [x] Focus on User Aliases parsing as required ✅ 2025-01-21
    - [x] Handle the "ALL=(ALL) ALL" specification ✅ 2025-01-21
    - [x] Implement user permission validation ✅ 2025-01-21
    - [ ] Implement group permission validation
- [ ] User Authentication:
    - [x] Implement password reading from stdin
    - [x] Create functions to read and parse /etc/shadow file
    - [x] Implement password verification using crypt()
    - [x] Add the 3-attempt limit for password entry
    - [x] Ensure secure password handling
- [ ] Command Execution:
    - [x] Implement the core command execution functionality ✅ 2025-01-21
    - [ ] Handle the -u flag for executing as different user
    - [ ] Handle the -g flag for executing with different group
    - [ ] Handle the -s flag for shell execution
    - [ ] Implement environment variable handling (especially for SHELL)
    - [ ] Handle the -E flag for executing with different env vars

## to resolve
- [ ] if only ```sudo``` error 84 and print usage
- [x] remove forbiden functions getpw*, getgr* ✅ 2025-01-23
