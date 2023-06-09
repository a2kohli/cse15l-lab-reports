# Lab Report 3 - The grep Command

## Using the grep command with the -i command line option

-i allows us to ignore the case of the matching string when we use grep.

This is useful as sometimes we might want to look at all occurences of the given string,
independent of the case. For instance, the starting word of a sentence always begins with a capital letter.
-i would allow us to match with that word even when the matching string is entirely in lowercase.

I found the information about this command line option at [freecodecamp](https://www.freecodecamp.org/news/grep-command-in-linux-usage-options-and-syntax-examples/#:~:text=Grep%20is%20a%20useful%20command,a%20powerful%20command%20to%20use.)

Examples of commands and their output have been shown below.

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

This is useful as sometimes we might want to locate where (which line) in the file
the occurence of the matching string is. For instance, if the file is a java file
and we are looking for the line throwing an error, we can type "error" as the matching
string and find the line number.

I found the information about this command line option at [freecodecamp](https://www.freecodecamp.org/news/grep-command-in-linux-usage-options-and-syntax-examples/#:~:text=Grep%20is%20a%20useful%20command,a%20powerful%20command%20to%20use.)

Examples of commands and their output have been shown below.

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

-w allows us to match the exact word we are providing as the matching string. 

This is useful when we want to look at where the EXACT string we are looking for occurs in the file.
For example, if the matching word is "one", then grep won't match with "everyone" or "anyone" in the file.

I found the information about this command line option at [freecodecamp](https://www.freecodecamp.org/news/grep-command-in-linux-usage-options-and-syntax-examples/#:~:text=Grep%20is%20a%20useful%20command,a%20powerful%20command%20to%20use.)

Examples of commands and their output have been shown below.

```
Command - grep -w "'normal'" ./technical/biomed/1468-6708-3-1.txt

Output - subgroup to the 'normal' group. The effect size is the
with BMI from 18.5 to 20 would be considered 'normal' by
```

```
Command - grep -w "one" ./technical/government/About_LSC/Comments_on_semiannual.txt

Output - conducted in April; one is scheduled for May; two are scheduled for
June; two are scheduled for July; and one is scheduled for
at least one statewide activity that will promote positive, lasting
one program to another. LSC's internal procedures for clearing
```


## Using the grep command with the -c command line option

-c allows us to count the number of times the matched string appears in the file.

This is useful when we want to count the number of times a particular string is repeated. For example,
if we are looking at a file with a DNA sequence, we can use this to find the number of cytosine bases.

I found the information about this command line option at [freecodecamp](https://www.freecodecamp.org/news/grep-command-in-linux-usage-options-and-syntax-examples/#:~:text=Grep%20is%20a%20useful%20command,a%20powerful%20command%20to%20use.)

Examples of commands and their output have been shown below.

```
Command - grep -c "alcohol" ./technical/government/Alcohol_Problems/DraftRecom-PDF.txt

Output - 53
```

```
Command - grep -c "kill" ./technical/911report/chapter-1.txt

Output - 9
```
