# Username Validator

A simple Python CLI tool that validates usernames based on predefined rules.

This project was created as part of my Python learning journey to practice functions, loops, conditions, strings, and input validation.

## Features

* Checks username length.
* Checks allowed characters.
* Rejects usernames containing invalid characters.
* Displays the reason when a username is invalid.
* Simple command-line interface.
* No external dependencies.

## Validation Rules

A username is considered valid if:

* Its length is between **3 and 20 characters**.
* It contains only:

  * English letters (`a-z`, `A-Z`)
  * Numbers (`0-9`)
  * Underscores (`_`)

### Valid Examples

```text
axiom
axiom123
axiom_dev
```

### Invalid Examples

```text
ax
axiom@123
axiom-dev
```

## Example

### Valid Username

```text
Enter the username: axiom_dev
Valid ✓
```

### Invalid Username

```text
Enter the username: axiom@123
Reason: Invalid character: @
Invalid ✗
```

## Requirements

* Python 3.x

No external Python packages are required.

## Installation

Clone the repository:

```bash
git clone https://github.com/axima-omgary/uservalidator/
```

Enter the project directory:

```bash
cd uservalidator
```

Run the program:

```bash
python3 uservalidator.py
```

## How It Works

The program performs multiple validation checks:

```text
Username
   │
   ├──→ Length Check
   │       │
   │       └──→ Valid / Invalid
   │
   └──→ Character Check
           │
           └──→ Valid / Invalid
                    │
                    ↓
              Final Result
```

Allowed characters are defined as:

```python
allowed_chars = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789_"
```

Each character in the username is checked against the allowed characters.

## Concepts Practiced

This project helped me practice:

* Variables
* Functions
* Function parameters
* Return values
* Strings
* `input()`
* `len()`
* `for` loops
* `if` statements
* Boolean values
* `in` / `not in`
* Input validation

## Project Structure

```text
username-validator/
├── uservalidator.py
└── README.md
```

## Learning Goal

This project is part of a series of small Python projects designed to strengthen programming fundamentals through practical projects.

The projects will gradually introduce the concepts needed to build larger and more complex tools.

## Disclaimer

This project is intended for educational purposes.

## License

This project is licensed under the MIT License.
