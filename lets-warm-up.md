# Lets Warm Up — CyLab Security Academy

**Category:** General Skills  
**Difficulty:** Easy  
**Platform:** CyLab Security Academy  
**Status:** Solved — November 22, 2026

## Challenge Description

"If I told you a word started with 0x70 in hexadecimal, what would it start with in ASCII?"

## My Approach

I first learned how binary, decimal, and hexadecimal number systems work.

I recognized that `0x70` represents a hexadecimal value.

To convert it into decimal:

`(7 × 16) + 0 = 112`

I then used the ASCII character ranges:

- Uppercase letters: 65–90
- Lowercase letters: 97–122

Since 112 falls within the lowercase range, I subtracted 97:

`112 - 97 = 15`

Starting from lowercase `a` at position 0, position 15 is `p`.

## Flag

`academy{p}`

## What I Learned

- How binary, decimal, and hexadecimal relate to each other.
- How hexadecimal values are converted to decimal.
- How ASCII represents uppercase and lowercase characters.
- How to calculate a letter's position using ASCII values.
- Why the correct flag format matters when submitting CTF solutions.

## Reflection

This was my first completed CTF challenge. Instead of simply looking up the answer, I took time to understand the underlying number systems and ASCII encoding.

I also learned that even when the technical solution is correct, submitting the wrong flag format can cause a challenge to be rejected.
