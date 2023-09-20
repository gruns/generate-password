# Generate Password

Simple Python utility that generates a strong password.

```
Usage:
  generate-password [-u] [-l] [-n] [-s] [--len <length>]

Options:
  -u, --no-uppercase           Exclude uppercase letters. (default: false)
  -l, --no-lowercase           Exclude lowercase letters. (default: false)
  -n, --no-numbers             Exclude numbers. (default: false)
  -s, --no-symbols             Exclude special symbols. (default: false)
  -e <length, --len <length>   Password length (default: 12).
  -h, --help                   Show this help message and exit.

Example:
  # generate-password
  TEm{m3{;Csvm

  # generate-password -s -e 4
  Va9U
```

Options:

* `-u`  Exclude uppercase letters. Default uppercase included.
* `-l`  Exclude lowercase letters. Default lowercase included.
* `-n`  Exclude numbers. Default numbers included.
* `-s`  Exclude special symbols. Default symbols included.
* `-e`  Password length. Default 12.

At least one character from every included character set is used in the
generated password. For example, if run with `-u` to exclude uppercase
characters

```
generate-password -u
```

then the generated password will include at least one lowercase letter,
at least one number, and at least one symbol. This is useful for
password requirements like `Must include at least one number`, `Must
include at least one special character`, etc.`