# Lab Report 3 - The grep Command

## Using the grep command with the -i command line option

-i allows us to ignore the case of the matching string when we use grep.

This is useful as sometimes we might want to look at all occurences of the given string,
independent of the case.

Examples of commands and their output has been shown below.

```
Command - grep -i "one" ./technical/government/About_LSC/Comments_on_semiannual.txt

Output - Ten programs were chosen for visits in 2001. One visit was
conducted in April; one is scheduled for May; two are scheduled for
June; two are scheduled for July; and one is scheduled for
at least one statewide activity that will promote positive, lasting
ideal telephone intake, advice, and referral systems. LSC and its
accepting comments to draft characteristics of a telephone intake
one program to another. LSC's internal procedures for clearing
Grantees Issued With Questioned Costs For the Six Month Period
```

```
Command - grep -i "rna" ./technical/biomed/rr166.txt 

Output - RNA synthesis in several cell types, including fibroblasts
twice, and the supernatants were pooled and cultured in
supernatant was aspirated and fresh media containing 30
min of incubation the supernatant was collected and saved
were used for RNA and protein extractions, respectively.
described [ 23 ] . Briefly, deuterium-labeled internal
1α were added to the supernatants with
internal standards had been added.
Cell pellets were lyzed and RNA extracted using the
instructions. RNA was quantified by determining light
MOPS/formaldehyde gel. The RNA was denatured prior to
loading by incubating the RNA at 65°C for 10 min in a
bromophenol blue, 0.025% xylene cyanol. The RNA was
showed minimal COX-2 mRNA in unstimulated cells and
significant upregulation of COX-2 mRNA expression when
upregulates COX-2 protein and mRNA expression to a similar
2 , decreases procollagen I and III mRNA
```

## Using the grep command with the -n command line option

-n allows us to see the line numbers against the output of grep. 

This is useful as sometimes we might want to locate where in the file
the occurence of the matching string is.

Examples of commands and their output has been shown below.

```
Command -  grep -n "impact" ./technical/government/Post_Rate_Comm/WolakSpeech_usps.txt

Output - 63:3) What is the impact of home computing technology on postal
```

```
Command - grep -n "dead" ./technical/911report/chapter-1.txt       
                 
Output - 190:    Callers reported that a passenger had been stabbed and that two people were lying on 
the floor of the cabin, injured or dead-possibly the captain and first officer. One caller reported that a flight attendant had been killed.
```

## Using the grep command with the -w command line option

-w allows us to match the exact word we are providing as the matching string

Examples of commands and their output has been shown below.

```
Command - grep -w "normal" ./technical/biomed/1468-6708-3-1.txt

Output - classifies normal weight (without reference to age) as a
subgroup to the 'normal' group. The effect size is the
with BMI from 18.5 to 20 would be considered 'normal' by
compared with normal group). Underweight men also had lower
the normal group, in part because of low sample size. Men
classified as normal, overweight or obese all had about the
women and men. Women who were normal or overweight averaged
normal group. The relationship of BMI to YHL for men is
women than for men in the normal and overweight groups, but
to the normal BMI group. The effect sizes are shown in
4.50 YHL compared to 4.92 for normal women, and the common
treatment to help underweight women achieve normal weight
underweight to normal. YHL and YOL have similar effect
to normal yielded small, non-significant effect sizes, with
would be needed. For comparing obese to normal, only YHL
to that of their normal weight peers could be performed
make obese women comparable to normal women could be
from those of normal weight, suggesting that these two
being obese to being normal would likely show changes in
normal-weight peers (presumably by addressing the
differences between the overweight and normal weight
```

```
Command - grep -w "one" ./technical/government/About_LSC/Comments_on_semiannual.txt

Output - conducted in April; one is scheduled for May; two are scheduled for
June; two are scheduled for July; and one is scheduled for
at least one statewide activity that will promote positive, lasting
one program to another. LSC's internal procedures for clearing
```


## Using the grep command with the -c command line option

Examples of commands and their output has been shown below.

```
Command - grep -c "alcohol" ./technical/government/Alcohol_Problems/DraftRecom-PDF.txt

Output - 53
```

```
Command - grep -c "kill" ./technical/911report/chapter-1.txt

Output - 9
```
