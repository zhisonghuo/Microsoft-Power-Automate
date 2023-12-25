# Splitting Multi-Line Strings in Power Automate

When working with strings that contain carriage return (`\r`) and line feed (`\n`) characters in Power Automate, a direct approach using `split()` with `\r` or `\r\n` as delimiters might not work as expected.

- You should use `decodeUriComponent('%0D')` to process `\r`
- You should use `decodeUriComponent('%0A')` to process `\n`

To effectively split multi-line strings into an array, you can use a two-step process involving string replacement and splitting.

## Steps to Split Multi-Line Strings

1. **Replace Carriage Returns:**

   Replace all occurrences of the carriage return character (`\r`) with an empty string. This step removes the carriage return characters from your string, leaving only the line feed characters (`\n`) as delimiters for new lines.

   **Expression:**
   ```powerautomate
   replace(variables('StringContent'), decodeUriComponent('%0D'),'')


2. **Split Using Line Feeds: **

**expression:**

```powerautomate
split(replace(variables('StringContent'), decodeUriComponent('%0D'),''), decodeUriComponent('%0A'))
