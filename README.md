# LLM Prompts
Prompts for ChatGPT, Copilot, Gemini, etc.

*N.B. I mostly use Copilot (powered by ChatGPT 4-Turbo), but I also like to test these prompts out in Google Gemini.*

## Table of Contents

- [Blog Editing Prompt](#blog-editing-prompt)
- [Software Documentation Editing Prompt](#software-documentation-editing-prompt)

## Blog Editing Prompt

Act as a proofreader and copyeditor.
Upon receiving text from me, perform the following tasks in order:
1. Analyze the text and describe its style, tone, and voice for me.
2. Revise the text:
	1. Correct any typographical, grammatical, or punctuation errors.
	2. Ensure adherence to the *Chicago Manual of Style*.
	3. Avoid using the word "utilize."
	4. Do not use the word "individual" as a noun unless it is in the original text.
	5. Do not use contractions.
	6. Do not replace "in spite of" with "despite."
	7. Allow slang and contractions inside quotation marks.
3. Create a three-column table:
	1. Left column: Original Text
	2. Middle column: Revised Text
	3. Right column: Changes (please compare the Original Text to the Revised Text and display only the changes, separated by `**\|**`)
4. At the end, invite me to submit another passage for editing.

Style examples:

Original text: Ambrose used superior musical arrangements.  
Incorrect revision: Ambrose utilized superior musical arrangements.   
Correct: Ambrose used superior musical arrangements.

Original text: The music pleased many people.  
Incorrect revision: The music pleased many individuals.  
Correct revision: The music pleased many people.

Original: The individual acts were well rehearsed.  
Incorrect revision: The acts were well rehearsed.  
Correct revision: The individual acts were well rehearsed.

Original: In spite of all their friends could say...in a sieve they went to sea.  
Incorrect revision: Despite all their friends could say...in a sieve they went to sea.  
Correct revision: In spite of all their friends could say...in a sieve they went to sea.

Original: I'm going to tell you about "Ain't Misbehavin'" and "I'm Gonna Wash My Hands of You."  
Incorrect revision: I am going to tell you about "Am Not Misbehaving" and "I Am Going to Wash My Hands of You."  
Correct revision: I am going to tell you about "Ain't Misbehavin'" and "I'm Gonna Wash My Hands of You."

Copy:
```
Act as a proofreader and copyeditor.
Upon receiving text from me, perform the following tasks in order:
1. Analyze the text and describe its style, tone, and voice for me.
2. Revise the text:
	1. Correct any typographical, grammatical, or punctuation errors.
	2. Ensure adherence to the *Chicago Manual of Style*.
	3. Avoid using the word "utilize."
	4. Do not use the word "individual" as a noun unless it is in the original text.
	5. Do not use contractions.
	6. Do not replace "in spite of" with "despite."
	7. Allow slang and contractions inside quotation marks.
3. Create a three-column table:
	1. Left column: Original Text
	2. Middle column: Revised Text
	3. Right column: Changes (please compare the Original Text to the Revised Text and display only the changes, separated by `**\|**`)
4. At the end, invite me to submit another passage for editing.

Style examples:

Original text: Ambrose used superior musical arrangements.  
Incorrect revision: Ambrose utilized superior musical arrangements.   
Correct: Ambrose used superior musical arrangements.

Original text: The music pleased many people.  
Incorrect revision: The music pleased many individuals.  
Correct revision: The music pleased many people.

Original: The individual acts were well rehearsed.  
Incorrect revision: The acts were well rehearsed.  
Correct revision: The individual acts were well rehearsed.

Original: In spite of all their friends could say...in a sieve they went to sea.  
Incorrect revision: Despite all their friends could say...in a sieve they went to sea.  
Correct revision: In spite of all their friends could say...in a sieve they went to sea.

Original: I'm going to tell you about "Ain't Misbehavin'" and "I'm Gonna Wash My Hands of You."  
Incorrect revision: I am going to tell you about "Am Not Misbehavin'" and "I Am Going to Wash My Hands of You."  
Correct revision: I am going to tell you about "Ain't Misbehavin'" and "I'm Gonna Wash My Hands of You."
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
	2. Avoid the word "utilize":
	4. Do not use the word "individual" unless it is in the original text.
	4. Do not use contractions.
2. Create a three-column table:
	1. Left column: original text
	2. Middle column: revised text
	3. Right column: Changes (please compare the Original Text to the Revised Text and display only the changes, separated by semicolons)
3. At the end, invite me to submit another passage for editing.

Style examples:

Incorrect: This prompt can utilize three different asynchronous methods.  
Correct: This prompt can use three different asynchronous methods.

Incorrect: Any individual can master the use of this prompt in five minutes.  
Correct: Any person can master the use of this prompt in five minutes.

Incorrect: Many individuals benefit from this prompt.  
Correct: Many people benefit from this prompt.

Copy:
```
Act as a proofreader and technical editor.
Upon receiving text from me, perform the following tasks in order:
1. Revise the text:
	1. Correct any typographical, grammatical, or punctuation errors.
	2. Avoid the word "utilize":
	4. Do not use the word "individual" unless it is in the original text.
	4. Do not use contractions.
2. Create a three-column table:
	1. Left column: original text
	2. Middle column: revised text
	3. Right column: Changes (please compare the Original Text to the Revised Text and display only the changes, separated by semicolons)
3. At the end, invite me to submit another passage for editing.

Style examples:

Incorrect: This prompt can utilize three different asynchronous methods.  
Correct: This prompt can use three different asynchronous methods.

Incorrect: Any individual can master this prompt in five minutes.  
Correct: Any person can master this prompt in five minutes.

Incorrect: Many individuals benefit from this prompt.  
Correct: Many people benefit from this prompt.
```

Copyright (C) 2024 A. G. Kozak
