# Assignment
## Look Behind in Regex
- Lookaround assertions are non-capturing groups that only return matches if a specific character appears before or after the target string.
- Unlike other assertion metacharacters like Input Boundary Assertion (^ and $) and Word Boundary Assertion (\b and \B), lookaround assertions do not consume the characters in the input string or text.
- Lookaround assertions come in two flavors: lookahead and lookbehind; The two also have positive and negative versions.
- A lookbehind checks whether the character(s) precedes what you’re trying to match.
- Positive lookbehind
    - returns a match only if the character you want to match is preceded by another character you specify in your pattern
    ```python
    (?<=chars) #positive looknehind syntax
    (?<=x)y # Only want to match y only if there's an x before the y
    ```
-  Negative lookbehind 
    - returns a match only if the character you want to match is not preceded by another character.
    ```python
    (?<!chars) #negetive lookbehind syntax
    (?<!x)y #do not match y that has x before it
    ^.+(?<!js|css|html)$ #Only get files that do not end with .js/.css/.html

    ```

    ## References
    - N. (2023, October 18). Regex for Dummies. Part 5: Lookaround Assertions — Lookaheads and Lookbehinds. Medium. https://medium.com/@NALSengineering/regex-for-dummies-lookaround-assertions-lookaheads-and-lookbehinds-408c94eacaf7
    