# Appndix: Command Line Commands

## File Tree Navigation
 `ls` lists all files and directories in the working directory.
  - `ls -a` lists all contents in working directory, includes hidden files and directories.
  - `ls -l` lists all contents of a directory in long format.
  - `ls -t` orders files and directories by the time they were last modified.
- `pwd` "print working directory"
- `rm` deletes files.
  - `rm -r` deletes a directory and all its child directories. 
- `touch` creates a new empty file in the working directory. 


## Input/Output Redirection
- `>` takes the standard output of the command on the left and redirects it to the file on the right.
- `>>` takes the standard output of the command on the left and *appends* it to the file on the right.
- `<` takes the standard input from the file on the right and inputs it into the program on the left.
- `|` is a "pipe". It takes the standard output of the command on the left, and *pipes* it as standard input to the command on the right.


## Alias 
- `alias` allows you to create keyboard shortcuts (aliases).


## Grep
`grep` stands for "global regular expression print". It searches files for lines that match a pattern and returns the results. 
Case sensitive.
[Grep Documentation located here](https://www.gnu.org/software/grep/manual/grep.html#Command_002dline-Options).

Syntax of grep command:
```bash
grep [option...] [patterns] [file...]
```
There can be zero or more options and zero or more files. 
Typically, patterns should be quoted.

- `grep -i` for case insensitive grep.
- `grep -R` ("Recursive") searches all files in a directory and outputs filenames and lines containing matched results. 
- `grep -Rl` ("Recursive" and "files with matches") searches all files in a directory and outputs only filenames with matched results.


## Uniq
`uniq` "unique". Takes a filename or standard input and prints out every line, removing any exact duplicates.

Syntax of uniq command:
```bash
uniq [option] [INPUT[OUTPUT]]
```
Options for uniq command:
- `-c` or `--count` to prefix lines by the number of occurrences.
- `-d` or `--repeated` only prints the repeated lines, not lines which aren't repeated.
- `-D` or `--all-repeated[=METHOD]` prints all duplicate lines. 
- `-u` or `--unique` to print only unique lines (non-duplicate lines).
- `-i` or `--ignore-case` to ignore the case sensitivity of characters when comparing.
- `-f` or `--skip-fields=N` skip fields to filter duplicate lines (for example, skip one column to filter for uniqueness in the next column). Avoid comparing the first N fields.
- `-s` or `--skip-char=N`skip characters (like the skip fields option). Avoid comparing the first N characters. 
- `-w` or `--check-chars=N` to consider characters (like checking characters, but only consider certain characters. For example, `-w 2` will consider only the first two characters for uniqueness).

*Note:* `sort` the input first to filter all unique lines, not just contiguous ones.


## Sort
[Sort documentation found here](https://ss64.com/bash/sort.html).
Tool to sort, merge, or compare all the lines from the files given (or standard input).

Sort command syntax:
```bash
sort [options] [file...]
sort [options] ... --files0-from=F
```

Sort command ordering options:
- `-b, --ignore-leading-blanks` to ignore leading blanks.
- `-d, --dictionary-order` to consider only blanks and alphanumeric characters.
- `-f, --ignore-case` to fold lower case to upper case characters.
- `-g, --general-numeric-sort` to compare according to general numerical value.
- `-i, --ignore-nonprinting` to consider only printable characters.
- `-M, --month-sort` to compare (unknown) < 'JAN' < ... < 'DEC'
- `-h, --human-numeric-sort` to compare human readable numbers (e.g., 2K 1G)
- `-n, --numeric-sort` to compare according to string numerical value.
- `-R, --random-sort` to sort by random hash of keys.
- `-random-source=FILE` to get random bytes from FILE.
- `-r, --reverse` to reverse the result of comparisons.
- `-sort=WORD` to sort according to *WORD* (word can be `general-numeric`, `human-numeric`, `month`, `numeric`, `random`, `version`)
- `-V, --version-sort` for natural sort of (version) numbers within text.

Other options given in sort man page (linked above).
Descriptions of how lines are compared and sorted given in man page. 
Examples of sort command also given in man page.


## Misc.
- `sed` "stream editor". Accepts standard input and modifies it based on an *expression* before displaying it as output data.
- `sort` takes a file name or standard input and orders each line alphabetically, printing it to standard output.
- `source` activates changes in bash profile for current session.



## Background Commands and Persistent Sessions

To run a command in the background, add ampersand to the end of the command:
```bash
command &
```
To suppress the `stdout` and `stderr` messages, use:
```bash
command > /dev/null 2>&1 &
```
To display the status of all stoped and background jobs in the current shell session:
```bash
jobs -l
```
To bring a background process to the foreground, use the `fg` command (or `fg %1` if you have multiple background jobs.

To terminate the background process, use the `kill` command followed by the process ID (which can be obtained through the `jobs -l` command, above. In this example it's 12928):
```bash
kill -9 12928
```

Generally, if connection drops or you exit the shell session, the background process terminates. 
To keep the process running, use the `disown` command or start the process with the `nohup` command.

Alternatively, use [Tmux](https://linuxize.com/post/getting-started-with-tmux/) ("terminal multiplexer") to switch between multiple programs in one terminal. 
Tmux sessions are persistent; programs will continue to run even if you exit the shell or are disconnected.



