# html-source-from-email
Extracting the HTML source code of an HTML email from Apple Mail is not just copy &amp; paste. The copied code needs to be cleaned of special characters first.

This repository is providing instructions on how to clean copied HTML code from an email in Apple Mail into clean HTML code.

# Steps to perform
1. View the emails' raw source by selecting View --> Message --> Raw Source
2. Copy the HTML part of the raw source
3. Delete all occurences of "=09"
4. Delete all occurences of "3D" - case-sensitive
5. Delete all occurences of the regexp "=\n\s+"

Then manually correct any remaining code issues. Look for occurences of "=" characters followed by a line break especially.

Done, you should have clean HTML code of your email now.
