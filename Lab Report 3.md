# Lab Report 3

## Researching Commands

I will be looking into the `grep` command and what kind of options are able to be used.

## `grep -v`
---
My first example I used `grep -v "ABA" */*/*/*.txt` to search through the directories.


This was the output:

```
technical/government/About_LSC/conference_highlights.txt:
technical/government/About_LSC/conference_highlights.txt:
technical/government/About_LSC/conference_highlights.txt:•
technical/government/About_LSC/conference_highlights.txt:Set high expectations for staff;
technical/government/About_LSC/conference_highlights.txt:
technical/government/About_LSC/conference_highlights.txt:
technical/government/About_LSC/conference_highlights.txt:•
technical/government/About_LSC/conference_highlights.txt:Delegate appropriate management functions so that the
technical/government/About_LSC/conference_highlights.txt:Executive Director can be a visible leader among staff and the
technical/government/About_LSC/conference_highlights.txt:greater equal justice community;
```

Here, what it is doing is outputting the lines that **DON'T** match with the inputed strings. This is useful if you're trying to see what lines don't include a certain string that you want every line 
