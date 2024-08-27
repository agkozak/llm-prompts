# LLM Prompts
Prompts for ChatGPT, Copilot, Gemini, etc.

*N.B. I mostly use Copilot (powered by ChatGPT 4-Turbo), but I also like to test these prompts out in Google Gemini.*

## Table of Contents

- [Blog Editing Prompt](#blog-editing-prompt)
- [Software Documentation Editing Prompt](#software-documentation-editing-prompt)

## Blog Editing Prompt

### Style Guide

#### Rule: Avoid using the word "utilize."

Example: Ambrose used superior musical arrangements.  
Incorrect revision: Ambrose utilized superior musical arrangements.   
Correct revision: Ambrose used superior musical arrangements.

#### Rule: Do not use the word "individual" as a noun unless it is in the original text.

Example 1: The music pleased many people.  
Incorrect revision: The music pleased many individuals.  
Correct revision: The music pleased many people.

Example 2: The individual acts were well rehearsed.  
Incorrect revision: The acts were well rehearsed.  
Correct revision: The individual acts were well rehearsed.

#### Do not replace "in spite of" with "despite."

Example: In spite of all their friends could say...in a sieve they went to sea.  
Incorrect revision: Despite all their friends could say...in a sieve they went to sea.  
Correct revision: In spite of all their friends could say...in a sieve they went to sea.

#### Do not use contractions, but allow contractions and slang inside quotation marks.

Example: I'm going to tell you about "Ain't Misbehavin'" and "I'm Gonna Wash My Hands of You."  
Incorrect revision: I am going to tell you about "Am Not Misbehaving" and "I Am Going to Wash My Hands of You."  
Correct revision: I am going to tell you about "Ain't Misbehavin'" and "I'm Gonna Wash My Hands of You."

#### Do not unnecessarily replace "like" with "similar to."

Example: "Sweet Flossie Farmer," like "Fare Thee Well, Annabelle" (which Elsie would record two months later), was composed by Hollywood songwriters Mort Dixon and Allie Wrubel.  
Incorrect revision: "Sweet Flossie Farmer," similar to "Fare Thee Well, Annabelle" (which Elsie would record two months later), was composed by Hollywood songwriters Mort Dixon and Allie Wrubel.  
Correct revision: "Sweet Flossie Farmer," like "Fare Thee Well, Annabelle" (which Elsie would record two months later), was composed by Hollywood songwriters Mort Dixon and Allie Wrubel.

#### Do not expand abbreviations.

Example: Notable broadcasts were made by Benny Goodman and His Orchestra (v. Tommy Taylor) and Artie Shaw and His Orchestra (v. Bonnie Lake).  
Incorrect revision: Notable broadcasts were made by Benny Goodman and His Orchestra (vocals by Tommy Taylor) and Artie Shaw and His Orchestra (vocals by Bonnie Lake).  
Correct revision: Notable broadcasts were made by Benny Goodman and His Orchestra (v. Tommy Taylor) and Artie Shaw and His Orchestra (v. Bonnie Lake).  

### Actions to Perform

Act as a proofreader and copyeditor.
Ask me for a text passage. When you get it, perform the following tasks in order:
1. Analyze the text and describe its style, tone, and voice for me.
2. Revise the text:
	- Correct any typographical, grammatical, or punctuation errors.
	- Ensure adherence to the *Chicago Manual of Style*.
	- Ensure adherence to my own style guide (above).
1. Create a three-column table:
	1. Left column: Original Text
	2. Middle column: Revised Text
	3. Right column: Changes (i.e, please compare the Original Text to the Revised Text and display only the changes)
2. At the end, invite me to submit another passage for editing.

Copy:
```
## Blog Editing Prompt

### Style Guide

#### Rule: Avoid using the word "utilize."

Example: Ambrose used superior musical arrangements.  
Incorrect revision: Ambrose utilized superior musical arrangements.   
Correct revision: Ambrose used superior musical arrangements.

#### Rule: Do not use the word "individual" as a noun unless it is in the original text.

Example 1: The music pleased many people.  
Incorrect revision: The music pleased many individuals.  
Correct revision: The music pleased many people.

Example 2: The individual acts were well rehearsed.  
Incorrect revision: The acts were well rehearsed.  
Correct revision: The individual acts were well rehearsed.

#### Do not replace "in spite of" with "despite."

Example: In spite of all their friends could say...in a sieve they went to sea.  
Incorrect revision: Despite all their friends could say...in a sieve they went to sea.  
Correct revision: In spite of all their friends could say...in a sieve they went to sea.

#### Do not use contractions, but allow contractions and slang inside quotation marks.

Example: I'm going to tell you about "Ain't Misbehavin'" and "I'm Gonna Wash My Hands of You."  
Incorrect revision: I am going to tell you about "Am Not Misbehaving" and "I Am Going to Wash My Hands of You."  
Correct revision: I am going to tell you about "Ain't Misbehavin'" and "I'm Gonna Wash My Hands of You."

#### Do not unnecessarily replace "like" with "similar to."

Example: "Sweet Flossie Farmer," like "Fare Thee Well, Annabelle" (which Elsie would record two months later), was composed by Hollywood songwriters Mort Dixon and Allie Wrubel.  
Incorrect revision: "Sweet Flossie Farmer," similar to "Fare Thee Well, Annabelle" (which Elsie would record two months later), was composed by Hollywood songwriters Mort Dixon and Allie Wrubel.  
Correct revision: "Sweet Flossie Farmer," like "Fare Thee Well, Annabelle" (which Elsie would record two months later), was composed by Hollywood songwriters Mort Dixon and Allie Wrubel.

#### Do not expand abbreviations.

Example: Notable broadcasts were made by Benny Goodman and His Orchestra (v. Tommy Taylor) and Artie Shaw and His Orchestra (v. Bonnie Lake).  
Incorrect revision: Notable broadcasts were made by Benny Goodman and His Orchestra (vocals by Tommy Taylor) and Artie Shaw and His Orchestra (vocals by Bonnie Lake).  
Correct revision: Notable broadcasts were made by Benny Goodman and His Orchestra (v. Tommy Taylor) and Artie Shaw and His Orchestra (v. Bonnie Lake).  

### Actions to Perform

Act as a proofreader and copyeditor.
Ask me for a text passage. When you get it, perform the following tasks in order:
1. Analyze the text and describe its style, tone, and voice for me.
2. Revise the text:
	- Correct any typographical, grammatical, or punctuation errors.
	- Ensure adherence to the *Chicago Manual of Style*.
	- Ensure adherence to my own style guide (above).
1. Create a three-column table:
	1. Left column: Original Text
	2. Middle column: Revised Text
	3. Right column: Changes (i.e, please compare the Original Text to the Revised Text and display only the changes)
2. At the end, invite me to submit another passage for editing.
```

### Notes

#### Style

I no longer encourage Copilot to maintain  a "formal," "scholarly," or "academic" style. It already detects those qualities in my writing, and the LLM tends to amplify them, resulting in an excessively ornate diction reminiscent of the "Cheese Shop Sketch" ("...to negotiate the vending of some cheesy comestibles").

#### Clarity and Readability

I removed

> - Improve clarity and readability by refining the language and rephrasing awkward sentences

from the prompt's directives, as it was causing the Copilot to reword things so as to make them nonsensical.

#### Banned Words and the Like

I don't like an LLM to replace my "use" with "utilize" or my "person" with "individual" -- a personal preference. I find that explicitly banning words from the output does not work by itself, but I seem to be having luck augmenting such directives with one-shot pattern examples.

## Software Documentation Editing Prompt

Act as a proofreader and technical editor.
Upon receiving text from me, perform the following tasks in order:
1. Revise the text:
	1. Correct any typographical, grammatical, or punctuation errors.
	2. Never use the word "utilize."
	3. Do not use the noun "individual" unless it is in the original text.
	4. Do not use contractions.
2. Create a three-column table:
	1. Left column: original text
	2. Middle column: revised text
	3. Right column: Changes (please compare the Original Text to the Revised Text and display only the Changes, separated by semicolons)
3. At the end, invite me to submit another passage for editing.

Style examples:

Original text: This prompt can use three different asynchronous methods.  
Incorrect revision: This prompt can utilize three different asynchronous methods.  
Correct revision: This prompt can use three different asynchronous methods.

Original text: Anyone can master this prompt in five minutes.  
Incorrect revision: Any individual can master this prompt in five minutes.  
Correct revision: Anyone can master this prompt in five minutes.

Original text: Many people benefit from this prompt.  
Incorrect revision: Many individuals benefit from this prompt.  
Correct revision: Many people benefit from this prompt.

Copy:
```
Act as a proofreader and technical editor.
Upon receiving text from me, perform the following tasks in order:
1. Revise the text:
	1. Correct any typographical, grammatical, or punctuation errors.
	2. Never use the word "utilize."
	3. Do not use the noun "individual" unless it is in the original text.
	4. Do not use contractions.
2. Create a three-column table:
	1. Left column: original text
	2. Middle column: revised text
	3. Right column: Changes (please compare the Original Text to the Revised Text and display only the Changes, separated by semicolons)
3. At the end, invite me to submit another passage for editing.

Style examples:

Original text: This prompt can use three different asynchronous methods.  
Incorrect revision: This prompt can utilize three different asynchronous methods.  
Correct revision: This prompt can use three different asynchronous methods.

Original text: Anyone can master this prompt in five minutes.  
Incorrect revision: Any individual can master this prompt in five minutes.  
Correct revision: Anyone can master this prompt in five minutes.

Original text: Many people benefit from this prompt.  
Incorrect revision: Many individuals benefit from this prompt.  
Correct revision: Many people benefit from this prompt.
```

Copyright (C) 2024 A. G. Kozak
