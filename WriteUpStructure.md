# <Challenge Name>

> **TL;DR**
>
> Briefly summarize the challenge, the vulnerability/concept involved, and the overall solution path.
>
> Example:
> "This challenge involved exploiting an XXE vulnerability to retrieve a hidden file. After enumerating the XML parser behavior, I crafted a malicious payload that disclosed the flag."

---

# Challenge Information

| Field | Value |
|---------|--------|
| CTF | <CTF Name> |
| Year | <Year> |
| Category | <Web / Pwn / Crypto / Rev / Misc / Forensics> |
| Points | <Points> |
| Difficulty | <Easy / Medium / Hard> |
| Author | <Author (optional)> |

## Challenge Description

```text
<Paste the original challenge description here>
```

---

# Initial Thoughts

Describe your first impressions.

Questions considered:

- What immediately stood out?
- Was the challenge hinting at a particular vulnerability?
- What assumptions did you make initially?

---

# Enumeration / Recon

Document everything you observed.

## Files Provided

```text
challenge.zip
└── app.py
```

## Services

```bash
nmap -sV target
```

Output:

```text
<output>
```

## Website Behavior

- Observed:
- Inputs:
- Cookies:
- Headers:
- Parameters:

### Screenshot

![Initial page](images/initial_page.png)

---

# Rabbit Holes

Document ideas that did **not** work.

## Attempt 1

Why it seemed promising:

- ...

What was tried:

```bash
...
```

Why it failed:

- ...

---

# Analysis

Explain the thought process.

## Interesting Observation

Describe what was discovered.

Example:

- User input was reflected.
- No sanitization appeared to exist.
- Error messages leaked useful information.

### Evidence

```text
...
```

### Screenshot

![Interesting behavior](images/behavior.png)

---

# Developing the Exploit

Describe how the solution evolved.

## Step 1

Reasoning:

- ...

Command:

```bash
...
```

Output:

```text
...
```

---

## Step 2

Reasoning:

- ...

Command:

```bash
...
```

Output:

```text
...
```

---

# Final Exploit

## Payload

```text
...
```

## Script

```python
#!/usr/bin/env python3

# Explain what each section does

from pwn import *

# Connect
conn = remote("host", 1337)

# Exploit logic
...

# Retrieve flag
print(conn.recvall())
```

---

# Flag

```text
flag{...}
```

---

# Why It Worked

Explain the underlying concept.

## Vulnerability

- Buffer Overflow
- SQL Injection
- XXE
- Format String
- RSA Weakness
- etc.

### Technical Explanation

Describe:

1. Root cause.
2. Why the payload succeeds.
3. Why protections failed.
4. How the challenge designer intended the solve.

---

# Alternative Approaches

Other possible solution paths:

- ...
- ...
- ...

---

# Lessons Learned

Things worth remembering:

- ...
- ...
- ...

Useful commands:

```bash
...
```

Useful techniques:

- ...
- ...

---

# References

## Articles

- <link>
- <link>

## Tools Used

- Burp Suite
- Ghidra
- pwntools
- CyberChef
- Wireshark
- IDA
- angr

## Documentation

- ...
- ...

---

# Reproducibility

## Environment

| Component | Version |
|------------|---------|
| OS | Kali Linux 2025 |
| Python | 3.12 |
| pwntools | 4.x |
| gcc | 13.x |

## Files

```text
.
├── exploit.py
├── challenge
├── libc.so.6
└── README.md
```

---

# Appendix

## Full Outputs

```text
...
```

## Extra Screenshots

![Screenshot](images/example.png)

---

# Summary

**Challenge:** <Name>

**Key Concept:** <Main vulnerability>

**Main Takeaway:**

> One or two sentences summarizing what this challenge teaches.