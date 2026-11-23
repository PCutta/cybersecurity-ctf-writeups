# convertme.py — Python and Binary Conversion

**Platform:** CyLab Security Academy
**Category:** General Skills
**Difficulty:** Easy
**Status:** Solved

## Challenge Objective

Download and run a Python script that asks the user to convert a decimal number into binary to retrieve the challenge flag.

## Environment

- CyLab Security Academy browser-based Linux workspace
- Linux terminal
- Python 3

## Approach

### 1. Download the Python Script

I used the Linux `wget` command to download the provided Python script directly into the CyLab workspace.

```bash
wget <challenge-file-url>
```

The file was saved as `convertme.py`.

### 2. Inspect the Downloaded Files

I used the following command to check the files in the current directory:

```bash
ls -l
```

This displayed the Python script alongside the other files in the workspace.

### 3. Attempt to Execute the Script

I changed the file permissions using:

```bash
chmod +x convertme.py
```

My initial attempt to execute the script directly produced an error.

This helped me understand that Python scripts are different from compiled Linux executables.

### 4. Run the Script Using Python

I learned that Python scripts can be executed using the Python 3 interpreter:

```bash
python3 convertme.py
```

The script ran successfully and presented a decimal-to-binary conversion question.

### 5. Solve the Binary Conversion

The script asked me to convert the decimal number **39** into binary.

I identified the powers of two that add up to 39:

32 + 4 + 2 + 1 = 39

| Place Value | 32 | 16 | 8 | 4 | 2 | 1 |
|---|---|---|---|---|---|---|
| Binary Digit | 1 | 0 | 0 | 1 | 1 | 1 |

Therefore:

**39 in decimal = 100111 in binary**

I entered the binary value, and the script confirmed that my answer was correct.

## Result

Successfully executed the Python script, completed the binary conversion, retrieved the flag, and solved the challenge.

## Skills Practiced

- Downloading files using `wget`
- Working with a Linux terminal
- Viewing file permissions using `ls -l`
- Changing permissions using `chmod`
- Running Python scripts with `python3`
- Troubleshooting command-line errors
- Converting decimal numbers into binary

## What I Learned

This challenge helped me understand the difference between running compiled Linux executables and executing Python scripts through an interpreter.

I also reinforced my knowledge of binary number systems and gained experience troubleshooting commands in a Linux environment.

These skills are useful for Python programming, Linux administration, IT support, and cybersecurity.
