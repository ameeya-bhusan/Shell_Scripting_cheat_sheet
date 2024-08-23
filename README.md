# 📝 Shell Scripting Cheat Sheet

A quick reference guide for shell scripting, including basic commands, control structures, and useful tips.

## Table of Contents

- [Basic Commands](#basic-commands)
- [Variables](#variables)
- [Control Structures](#control-structures)
  - [If Statements](#if-statements)
  - [Loops](#loops)
- [Functions](#functions)
- [File Operations](#file-operations)
- [String Operations](#string-operations)
- [Useful Tips](#useful-tips)
- [References](#references)

---

## Basic Commands

| Description                          | Command                          |
|--------------------------------------|----------------------------------|
| Print text                           | `echo "Hello, World!"`            |
| List directory contents              | `ls`                              |
| Change directory                     | `cd /path/to/directory`           |
| Print working directory              | `pwd`                             |
| Copy files                           | `cp source.txt destination.txt`   |
| Move files                           | `mv oldname.txt newname.txt`      |
| Remove files                         | `rm filename.txt`                 |
| Create directory                     | `mkdir new_directory`             |
| Remove directory                     | `rmdir directory`                 |

---

## Variables

| Description                          | Command                          |
|--------------------------------------|----------------------------------|
| Declare a variable                   | `variable_name=value`            |
| Access a variable                    | `$variable_name`                 |
| Export a variable                    | `export variable_name=value`     |
| Unset a variable                     | `unset variable_name`            |

---

## Control Structures

### If Statements

| Description                          | Command                          |
|--------------------------------------|----------------------------------|
| Basic if statement                   | `if [ condition ]; then commands; fi` |
| If-else statement                    | `if [ condition ]; then commands; else commands; fi` |
| Nested if statements                 | `if [ condition ]; then if [ condition ]; then commands; fi; fi` |

### Loops

| Description                          | Command                          |
|--------------------------------------|----------------------------------|
| For loop                             | `for var in list; do commands; done` |
| While loop                           | `while [ condition ]; do commands; done` |
| Until loop                           | `until [ condition ]; do commands; done` |

---

## Functions

| Description                          | Command                          |
|--------------------------------------|----------------------------------|
| Define a function                    | `function_name() { commands; }`  |
| Call a function                      | `function_name`                  |
| Function with arguments              | `function_name() { param1=$1; commands; }` |
| Access arguments                     | `$1`, `$2`, etc.                 |

---

## File Operations

| Description                          | Command                          |
|--------------------------------------|----------------------------------|
| Check if file exists                 | `[ -e filename ]`                |
| Check if directory exists            | `[ -d directory ]`              |
| Check if file is readable            | `[ -r filename ]`                |
| Check if file is writable            | `[ -w filename ]`                |
| Check if file is executable          | `[ -x filename ]`                |
| Create an empty file                 | `touch filename.txt`             |

---

## String Operations

| Description                          | Command                          |
|--------------------------------------|----------------------------------|
| String length                        | `echo ${#string}`                 |
| Substring                             | `echo ${string:start:length}`     |
| Replace substring                    | `echo ${string/old/new}`          |
| Convert to uppercase                 | `echo ${string^^}`                |
| Convert to lowercase                 | `echo ${string,,}`                |

---

## Useful Tips

- **Shebang**: Use `#!/bin/bash` at the top of your script to specify the interpreter.
- **Debugging**: Use `bash -x script.sh` to debug your script.
- **Permissions**: Make scripts executable with `chmod +x script.sh`.
- **Script location**: Add scripts to your `PATH` for easy access.

---

## References

- [GNU Bash Manual](https://www.gnu.org/software/bash/manual/)
- [Bash Scripting Guide](https://tldp.org/LDP/abs/html/)
- [ShellCheck](https://www.shellcheck.net/) (Online shell script analysis)

---

This `README.md` serves as a quick reference guide for shell scripting, providing essential commands, control structures, functions, and useful tips.
