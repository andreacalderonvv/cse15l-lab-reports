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


