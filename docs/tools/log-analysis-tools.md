# Log Analysis

## Command Line Log Analysis Tools
- `cut` extracts column(s) from a file or text stream. Columns must be delineated by a consistent character. 
  - `cut example.txt -d , -f 2` prints the second column from example.txt where a comma is used to separate each column.
- `sort` sorts the lines from a file or text stream.
  - `sort example.txt` prints the sorted output of the lines from example.txt.
  - `sort -n example.txt` uses numberical value to sort.
  - `sort -b example.txt` ignores blanks at the start of the line.
  - `sort -r example.txt` reverses the sorting order.
  - `-k` flag is useful for sorting databases.
- `uniq` prints the result of removing any duplicate lines from a file or text stream.
  - `uniq example.txt` prints the result of removing any duplicate lines from example.txt.
  - Usually use this after using `sort`; it only removes adjacent duplicate lines.
- `grep` "Global Regular Expression Print" searches for text that matches a specific pattern.
  - `grep match example.txt` prints lines that contain the text "match" in example.txt.
  - grep IP address:
    ```bash
    grep -E '[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}' example.txt
    ```
  - grep only valid IP address:
    ```bash
    grep -E '^((25[0-5]|2[0-4][0-9]|[1]?[1-9][0-9]?).){3}(25[0-5]|2[0-4][0-9]|[1]?[1-9]?[0-9])$' example.txt
    ```
    - `ping` to remove leading zeros.
- `wc` "Word Count" gets a line count (followed by a word count and a byte count) of a file or text stream.
  - `wc example.txt` prints the number of lines, words, bytes in example.txt.
  - `-l` flag to print number of lines only.
  - `-c` flag to print number of bytes only.
  - `-w` flag to print number of words only. A word is defined as a string of characters delimited by spaces, tabs, or newline characters.
- `awk` is a tool used to manipulate data. It can be used to extract specific columns from data.
  - `cat example.txt | awk '{print #2}'` prints the second column in example.txt.
- `tail` prints the last 10 lines of a file.
  - `tail example.txt` prints the last 10 lines of example.txt.
  - `tail -12 example.txt` prints the last 12 lines of example.txt.
- `head` prints the first 10 lines of a file.
  - `head example.txt` prints the first 10 lines of example.txt.
  - `head -7 example.txt` prints the first 7 lines of example.txt.

## SQLite
- [SQLite Browser](https://sqlitebrowser.org/dl/)
  - `sqlitebrowser` GUI.
- [`sqlite3 <file.sqlite>`](https://www.sqlite.org/cli.html)
  - `.tables` to see a list of tables.
  - `.index` to see index.
  - `.schema` to see a list of schema.
  - `.databases`
    
## Creating Programs to do Log Analysis
- `.json` File, Python analysis:
  - *Find unique IPs, unique signatures, most popular category, total bytes sent, category of non TCP traffic*
```python
import json
f = open('filename.json')
```


## Articles and Tutorials
- [CryptoKait: How to Approach a Wild Log](https://cryptokait.com/2021/02/10/command-line-log-analysis-for-the-win-1-3-how-to-approach-a-wild-log/)
- [CryptoKait: Walking Through "Leaping"](https://cryptokait.com/2021/02/15/command-line-log-analysis-for-the-win-2-3-walking-through-leaping/)
- [CryptoKait: Untangling a Web Access Log](https://cryptokait.com/2021/02/17/command-line-log-analysis-for-the-win-3-3-untangling-a-web-access-log/)



