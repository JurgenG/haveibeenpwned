# haveibeenpwned
Python script to verify multiple email addresses for pwnage

usage:
  -h, --help     show this help message and exit
  -a ADDRESS     Single email address to be checked
  -f FILENAME    File to be checked with one email addresses per line
  -o OUTPUTFILE  File to store the infected addresses, the last affected date and the full HaveIBeenPwned JSON reply

This tool respects the rate limit (HTTP 429) and adjusts accordingly.
Output is in color to show the differences between breached and not breached.

Example output:

[i] info@example.com has not been breached.

[!] lastfm@example.com has been breached!

[!] Rate limit exceeded, server instructed us to retry after 2 seconds
    Refer to acceptable use of API: https://haveibeenpwned.com/API/v2#AcceptableUse

[i] example@example.com has not been breached.

EOF:w
