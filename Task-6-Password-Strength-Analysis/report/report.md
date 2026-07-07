# Task 6 - Create a Strong Password and Evaluate Its Strength

## Student Information

| Field | Details |
|--------|---------|
| **Name** | PRASIDDHA PAL |
| **Branch** | CSE (2027) |
| **Internship** | Cyber Security Internship |
| **Organization** | Elevate Labs |
| **Task** | Task 6 - Create a Strong Password and Evaluate Its Strength |
| **Status** | ✅ Completed |

---

# Objective

To understand the characteristics of strong passwords by creating passwords with different complexity levels and evaluating them using an online password strength checker.

---

# Tools Used

- Ubuntu Linux
- Web Browser
- PasswordMeter (or another password strength checker)

---

# Procedure

## Step 1: Create Sample Passwords

Three passwords with different complexity levels were created for testing.

| Password Example | Complexity |
|------------------|------------|
| `password123` | Weak |
| `P@ssword123!` | Medium |
| `M7#qLp9!vR2@xK8` | Strong |

> **Note:** These are sample passwords created for demonstration only. They are **not** intended for real-world use.

---

## Step 2: Evaluate Password Strength

Each password was tested using an online password strength checker.

The following factors were considered:

- Password Length
- Uppercase Letters
- Lowercase Letters
- Numbers
- Symbols
- Randomness
- Predictability

---

## Step 3: Results

| Password | Strength | Observation |
|----------|----------|-------------|
| `password123` | Weak | Common word with predictable numbers |
| `P@ssword123!` | Medium | Better complexity but still partially predictable |
| `M7#qLp9!vR2@xK8` | Very Strong | Long, random, and difficult to guess |

---

# Analysis

### Weak Password

- Contains a common dictionary word.
- Easy to guess.
- Vulnerable to dictionary and brute-force attacks.

### Medium Password

- Includes uppercase letters, numbers, and symbols.
- More secure than a weak password but still based on a common word.

### Strong Password

- Uses a long and random combination of characters.
- Includes uppercase letters, lowercase letters, numbers, and symbols.
- Provides significantly better resistance against password attacks.

---

# Common Password Attacks

## Brute Force Attack

Attempts every possible password combination until the correct password is found.

## Dictionary Attack

Uses a predefined list of common words and leaked passwords.

## Credential Stuffing

Uses usernames and passwords leaked from one website to try logging into other websites.

---

# Best Practices

- Use passwords with at least 12–16 characters.
- Combine uppercase letters, lowercase letters, numbers, and symbols.
- Avoid personal information such as names and birthdays.
- Do not reuse passwords across multiple accounts.
- Use a password manager to generate and store passwords securely.
- Enable Multi-Factor Authentication (MFA) whenever possible.

---

# Learning Outcomes

- Learned how password strength is evaluated.
- Understood why password length and randomness are important.
- Explored common password attacks.
- Identified best practices for creating secure passwords.

---

# Screenshots

Add screenshots in the `screenshots/` folder.

```
screenshots/
├── 01-weak-password.png
├── 02-medium-password.png
├── 03-strong-password.png
└── 04-summary.png
```

---

# Repository Structure

```text
Task-6-Password-Strength-Analysis/
├── README.md
├── REPORT.md
└── screenshots/
    ├── 01-weak-password.png
    ├── 02-medium-password.png
    ├── 03-strong-password.png
    └── 04-summary.png
```

---

# Conclusion

Password strength depends on length, complexity, and randomness. Strong passwords are much more resistant to brute-force and dictionary attacks than short or predictable passwords. Following password security best practices and enabling Multi-Factor Authentication (MFA) greatly improves account security.
