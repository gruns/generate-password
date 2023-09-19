# Generate Password

Simple Python utility that generates a strong password.

Options:

* `-u` Exclude uppercase letters. Default included.
* `-l` Exclude lowercase letters. Default included.
* `-n` Exclude numbers. Default included.
* `-s` Exclude special symbols. Default included.
* `-l` Password length. Default 12.

At least one character from every included character set is used in the
generated password. For example, if run with

```
generate-password -u
```

then the generated password will include at least one lowercase letter,
at least one number, and at least one symbol. This is useful for
password requirements like `Must include at least one number`, `Must
include at least one special character`, etc.