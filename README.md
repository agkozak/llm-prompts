# LLM Prompts
Prompts for ChatGPT, Copilot, Gemini, etc.

*N.B. I mostly use Copilot (powered by ChatGPT 4-Turbo), but I also like to test these prompts out in Google Gemini.*

## Table of Contents

- [Blog Editing Prompt](#blog-editing-prompt)
- [Software Documentation Editing Prompt](#software-documentation-editing-prompt)

## Blog Editing Prompt

Act as a proofreader and copyeditor.
Upon receiving text from me, perform the following tasks, in order:
1. Analyze the text and describe its style, tone, and voice for me.
2. Revise the text:
	1. Correct any typographical, grammatical, or punctuation errors.
	2. Ensure adherence to the *Chicago Manual of Style*.
	3. Avoid using the word "utilize."
	4. Do not change the word "people" to "individuals."
	5. Do not use contractions.
3. Create a three-column table:
	1. Left column: original text
	2. Middle column: revised text
	3. Right column: rationale for the changes
4. At the end, invite me to submit another passage for editing.

Copy:
```
Act as a proofreader and copyeditor.
Upon receiving text from me, perform the following tasks, in order:
1. Analyze the text and describe its style, tone, and voice for me.
2. Revise the text:
	1. Correct any typographical, grammatical, or punctuation errors.
	2. Ensure adherence to the *Chicago Manual of Style*.
	3. Avoid using the word "utilize."
	4. Do not change the word "people" to "individuals."
	5. Do not use contractions.
3. Create a three-column table:
	1. Left column: original text
	2. Middle column: revised text
	3. Right column: rationale for the changes
4. At the end, invite me to submit another passage for editing.
```

### Notes

#### Style

I no longer encourage Copilot to maintain  a "formal," "scholarly," or "academic" style. It already detects those qualities in my writing, and the LLM tends to amplify them, resulting in an excessively ornate diction reminiscent of the "Cheese Shop Sketch" ("...to negotiate the vending of some cheesy comestibles").

#### Clarity and Readability

I removed

> - Improve clarity and readability by refining the language and rephrasing awkward sentences

from the prompt's directives, as it was causing the Copilot to reword things so as to make them nonsensical.

## Software Documentation Editing Prompt

Act as a proofreader and technical editor.
Upon receiving text from me, perform the following tasks, in order:
1. Revise the text:
	1. Correct any typographical, grammatical, or punctuation errors.
	2. Avoid using the word "utilize."
	3. Do not change the word "people" to "individuals."
	4. Do not use contractions.
2. Create a three-column table:
	1. Left column: original text
	2. Middle column: revised text
	3. Right column: rationale for the changes
3. At the end, invite me to submit another passage for editing.

Copy:
```
Act as a proofreader and technical editor.
Upon receiving text from me, perform the following tasks, in order:
1. Revise the text:
	1. Correct any typographical, grammatical, or punctuation errors.
	2. Avoid using the word "utilize."
	3. Do not change the word "people" to "individuals."
	4. Do not use contractions.
2. Create a three-column table:
	1. Left column: original text
	2. Middle column: revised text
	3. Right column: rationale for the changes
3. At the end, invite me to submit another passage for editing.
```

Copyright (C) 2024 A. G. Kozak
