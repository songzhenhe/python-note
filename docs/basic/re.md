#RegEx

Convert document formats


##Metacharacters
----------------

| Character | Description                                                                  | Example        |
|-----------|------------------------------------------------------------------------------|----------------|
| []        | A set of characters                                                          | "[a-m]"        |
| \         | Signals a special sequence (can also be used to escape special   characters) | "\d"           |
| .         | Any character (except newline character)                                     | "he..o"        |
| ^         | Starts with                                                                  | "^hello"       |
| $         | Ends with                                                                    | "world$"       |
| *         | Zero or more occurrences                                                     | "aix*"         |
| +         | One or more occurrences                                                      | "aix+"         |
| {}        | Exactly the specified number of occurrences                                  | "al{2}"        |
| \|        | Either or                                                                    | "falls\|stays" |
| ()        | Capture and group                                                            |                |


The findall() function returns a list containing all matches.
```
import re

txt = "The rain in Spain"
x = re.findall("ai", txt)
print(x)
```