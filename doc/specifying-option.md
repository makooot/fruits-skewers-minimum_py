# Option format
Option format has short option, and long option.

Short option format begins with a single hyphen (-) followed by a single character (uppercase or lowercase).
The options without value is chainable.  For example, `-abc` is equivalent to `-a -b -c`.  However, only the last option can have a value. For example, `-abcd=efgh`  is equivalent to `-a -b -c -d=efgh`; in this case, `d` has value.

Long option format begin with two hyphens (--), followed by two or more characters (lowercase English letters and hyphens).

# Value specification
The name and value are connected by an equals sign (=).  For example, `--host=example.com`.
