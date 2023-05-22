# Lab Report 3

## Researching Commands

I will be looking into the `grep` command and what kind of options are able to be used with it.

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

This was the output:

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

Again, this command outputs lines that don't match with the inputted string "i". This is useful if someone is curious how often the letter i is not used in the lines.

## `grep -n`
---

The first example I used was `grep -n "i" */*/*/*.txt`

This was the output:

```
technical/government/Alcohol_Problems/DraftRecom-PDF.txt:408:settings?
technical/government/Alcohol_Problems/DraftRecom-PDF.txt:409:Soderstrom suggested that the term "practitioner" in this
technical/government/Alcohol_Problems/DraftRecom-PDF.txt:410:recommendation needs to be clarified because it can mean anyone who
technical/government/Alcohol_Problems/DraftRecom-PDF.txt:411:takes care of a patient, including RNs, MDs, therapists, and
technical/government/Alcohol_Problems/DraftRecom-PDF.txt:413:Bernstein noted that alcohol-dependent patients clearly need
technical/government/Alcohol_Problems/DraftRecom-PDF.txt:414:specialized treatment and that some patients with hazardous
technical/government/Alcohol_Problems/DraftRecom-PDF.txt:415:drinking need out-patient counseling. He said if access to that
technical/government/Alcohol_Problems/DraftRecom-PDF.txt:416:counseling is not available, screening and interventions are less
technical/government/Alcohol_Problems/DraftRecom-PDF.txt:417:likely to happen in the ED. He called for research on barriers
technical/government/Alcohol_Problems/DraftRecom-PDF.txt:418:emergency physicians face in getting further care for ED patients
```

This command shows the line number of the line that includes the inputted string. This will be helpful if someone is trying to locate where a certain mention of the inputted string is.

The second example I used was `grep -n "Gutman" */*/*/*.txt` 

This was the output:

```
technical/government/Alcohol_Problems/Session2-PDF.txt:632:67. Williams J, Chinnis A, Gutman D. Health promotion practices
```

Again, this command shows the line number where the string appears. In this case it was 632. This is helpful when locating a mention of the string you inputted.

## `grep -i`
---

In the first example, I used the command `grep -i "HOWEVER" */*/*/*.txt `.

This is the output:

```
technical/government/About_LSC/CONFIG_STANDARDS.txt:or participation in each state. However, LSC continues to encourage
technical/government/About_LSC/LegalServCorp_v_VelazquezDissent.txt:experience, however, that these restrictions did not exhaust the
technical/government/About_LSC/LegalServCorp_v_VelazquezDissent.txt:on litigation, however, is unique, and it contains a proviso
technical/government/About_LSC/LegalServCorp_v_VelazquezDissent.txt:professional responsibility'"). The lawyers may, however, and
technical/government/About_LSC/LegalServCorp_v_VelazquezDissent.txt:"Petitioners contend, however, that most Title X cli
technical/government/About_LSC/LegalServCorp_v_VelazquezOpinion.txt:existing law. §1639.4. Under LSC's interpretation, however,
technical/government/About_LSC/LegalServCorp_v_VelazquezOpinion.txt:later cases, however, we have explained Rust on this understanding.
technical/government/About_LSC/LegalServCorp_v_VelazquezOpinion.txt:applies to subsidies for private speech in every instance, however.
technical/government/About_LSC/LegalServCorp_v_VelazquezOpinion.txt:government's message in the litigation. The LSC lawyer, however,
technical/government/About_LSC/LegalServCorp_v_VelazquezOpinion.txt:bar. Under §504(a)(16), however, cases would be presented by LSC
```
What this command does is find all the instances of the inputted string regardless of capital letters or lowercase. This is helpful when you are just looking for a word and not the word specifically when it is in capitals or all lowercase.

In this second example I used the command `grep -i "fda" */*/*/*.txt`. 

This is the output:

```
technical/government/Env_Prot_Agen/atx1-6.txt:practices related to toxicity testing, see: FDA, 1978; USEPA, 1975;
technical/government/Env_Prot_Agen/ctf1-6.txt:see FDA, (1978); USEPA, (1979d), USEPA (1980b), USEPA (1980c), and
technical/government/Env_Prot_Agen/ctm4-10.txt:see FDA (1978); USEPA (1979d); USEPA (1980b); USEPA (1980c); USEPA
technical/government/Gen_Account_Office/ai00134.txt:than fitting new technology to outofdate processes, Owens Corning
technical/government/Gen_Account_Office/og96038.txt:by the Food and Drug Administration (FDA) and published in the
technical/government/Gen_Account_Office/og96038.txt:has been revised based on comments the FDA received and now also
technical/government/Gen_Account_Office/og96038.txt:tobacco products to individuals under the age of 18. FDA considers
technical/government/Gen_Account_Office/og96038.txt:FDA estimates the overall compliance costs of the rule to be
technical/government/Gen_Account_Office/og96038.txt:one-time costs and $78 million in annual costs), FDA ($3 to $5
technical/government/Gen_Account_Office/og96038.txt:FDA recognizes that it could not quantify every regulatory cost
```

In this example, it searches for the string "fda" regardless of captial or lowercase letters. It is helpful to just search for the word regardless of capitials.

## `grep -c`
---

In the first example I used `grep -c "food" */*/*/*.txt`.

This is the output:

```
technical/government/About_LSC/CONFIG_STANDARDS.txt:0
technical/government/About_LSC/Comments_on_semiannual.txt:0
technical/government/About_LSC/LegalServCorp_v_VelazquezDissent.txt:0
technical/government/About_LSC/LegalServCorp_v_VelazquezOpinion.txt:0
technical/government/About_LSC/LegalServCorp_v_VelazquezSyllabus.txt:0
technical/government/About_LSC/ODonnell_et_al_v_LSCdecision.txt:0
technical/government/About_LSC/ONTARIO_LEGAL_AID_SERIES.txt:0
technical/government/About_LSC/Progress_report.txt:0
technical/government/About_LSC/Protocol_Regarding_Access.txt:0
technical/government/About_LSC/Special_report_to_congress.txt:0
```

Here, what the command does is output how many lines of the given string there is in the file. This is useful when you don't want to count the lines yourself or don't want all the lines printed.

In the second example, I used the command `grep -c "by" */*/*/*.txt`.

This is the output:

```
technical/government/About_LSC/CONFIG_STANDARDS.txt:3
technical/government/About_LSC/Comments_on_semiannual.txt:18
technical/government/About_LSC/LegalServCorp_v_VelazquezDissent.txt:28
technical/government/About_LSC/LegalServCorp_v_VelazquezOpinion.txt:32
technical/government/About_LSC/LegalServCorp_v_VelazquezSyllabus.txt:9
technical/government/About_LSC/ODonnell_et_al_v_LSCdecision.txt:11
technical/government/About_LSC/ONTARIO_LEGAL_AID_SERIES.txt:22
technical/government/About_LSC/Progress_report.txt:40
technical/government/About_LSC/Protocol_Regarding_Access.txt:22
```

In this example, it also prints out how many lines in the file match the given string. This is useful for when you don't want all the matching lines taking over your terminal.

## Sources:
---
All of these commands were found through the AI [ChatGPT](https://chat.openai.com/).

Input used: can you give me some command line argument options for grep?

Output: 

```
Certainly! grep is a powerful command-line tool used for searching text patterns within files. Here are some commonly used command-line argument options for grep:

Basic Usage: grep [pattern] [file]

Searches for the specified [pattern] within the [file].
Case Insensitivity: grep -i [pattern] [file]

Ignores case when searching for the [pattern].
Recursive Search: grep -r [pattern] [directory]

Recursively searches for the [pattern] within the specified [directory] and its subdirectories.
Invert Match: grep -v [pattern] [file]

Displays lines that do not match the [pattern].
Match Whole Word: grep -w [pattern] [file]

Matches the [pattern] as a whole word, rather than as part of a word.
Print Line Numbers: grep -n [pattern] [file]

Displays the line numbers along with the matched lines.
Count Matches: grep -c [pattern] [file]

Prints only the count of matching lines, without displaying the actual lines.
Multiple Patterns: grep -e [pattern1] -e [pattern2] [file]

Searches for multiple patterns within the [file].
Include/Exclude Files: grep --include=*.[ext] [pattern] [directory]

Searches only in files with a specific extension ([ext]) within the [directory].
Recursive Exclude: grep --exclude-dir=[dir] [pattern] [directory]

Excludes a specific directory ([dir]) from recursive searches.
These are just a few examples of the many options available with grep. You can explore more by referring to the grep manual page (man grep) or by using the grep --help command to see a brief summary of available options.
```

What I changed was that I only chose 4 commands and I replaced everything with the files I will be using.
