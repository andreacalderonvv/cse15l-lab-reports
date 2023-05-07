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

Here, what it is doing is outputting the lines that **DON'T** match with the inputted string, in this case "ABA". This is useful if you're trying to see what lines don't include a certain string that you want every line to include.

In this second example I used `grep -v "i" */*/*/*.txt` to search.

this was the output:

```
technical/government/Gen_Account_Office/og96026.txt:at the agency.
technical/government/Gen_Account_Office/og96026.txt:Fed. Reg. 13543.
technical/government/Gen_Account_Office/og96026.txt:Page 4 GAO/OGC-96-26
technical/government/Gen_Account_Office/og96026.txt:follows:
technical/government/Gen_Account_Office/og96026.txt:all major hazards, the consequences of each of these hazards, the
technical/government/Gen_Account_Office/og96026.txt:been, for large, complex sources, documents of a l,000 pages or
technical/government/Gen_Account_Office/og96026.txt:more."
technical/government/Gen_Account_Office/og96026.txt:of substances on January 31, 1994 (59 Fed. Reg. 4478).
technical/government/Gen_Account_Office/og96026.txt:under
technical/government/Gen_Account_Office/og96026.txt:Page 5 GAO/OGC-96-26
```

Again, this command outputs lines that don't match with the inputted string "i". This is useful if someone is curious how often the letter i is not used 
