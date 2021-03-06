﻿#Rainbow Table

Command line script that works with rainbow tables. Capable of generating hashes based on a list of passwords, and then using generated hashes to decipher hashed passwords. Currently supports md5 and sha1.

Usage:

```
> python rainbow_table.py -ops (generate|crack) [options] <input.txt> <output.txt>
```
Leave "output.txt" blank when generating rainbow table, as the script will write the hashes to a file called "database.rbt."

Possible options:

```
-ops, --operations      This is the operations flag. It can be either ‘generate’ or ‘crack’
-t, --type              This is the type of hash to use. It can be either ‘md5’ or ‘sha1’
-i, --input             This is the input file to be used. It is used for both operations.
-o, --output            This is the output file to be used. It is used only for ‘crack’
```
