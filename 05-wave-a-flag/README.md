# Wave a Flag — Linux Command-Line Basics

**Platform:** CyLab Security Academy
**Category:** General Skills
**Difficulty:** Easy
**Status:** Solved

## Challenge Objective

Execute a provided Linux program and discover how to display its hidden flag using command-line arguments.

## Environment

- CyLab Security Academy browser-based Linux workspace
- Linux terminal
- GNU command-line utilities

## Approach

### 1. Check for Download Tools

I verified that the `wget` utility was installed:

```bash
which wget
```

The terminal returned:

```text
/usr/bin/wget
```

### 2. Download the Challenge File

I copied the challenge file's URL and downloaded it directly into the Linux workspace using `wget`.

```bash
wget <challenge-file-url>
```

The file was saved as `warm`.

### 3. Inspect the File

I listed the files and their permissions:

```bash
ls -l
```

Then I identified the file format:

```bash
file warm
```

The terminal identified `warm` as a 64-bit ELF Linux executable.

### 4. Modify File Permissions

The downloaded file did not initially have executable permissions.

I enabled execution using:

```bash
chmod +x warm
```

### 5. Execute the Program

I ran the program with the `-h` help argument:

```bash
./warm -h
```

The program displayed its help information, including the challenge flag.

## Result

Successfully retrieved and submitted the flag using the Linux command line.

## Skills Practiced

- Navigating a Linux terminal
- Downloading files with `wget`
- Inspecting files using `file`
- Viewing permissions with `ls -l`
- Modifying permissions with `chmod`
- Running Linux executables
- Using command-line arguments

## What I Learned

This challenge introduced me to practical Linux command-line operations.

I learned that downloaded executables may require permission changes before they can run.

I also learned how command-line arguments such as `-h` can reveal useful information about a program.

These skills are relevant to Linux administration, troubleshooting, and cybersecurity.
