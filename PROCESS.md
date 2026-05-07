# Processes
This file aims to document all decision-making processes that included AI tools during this project.

## Base
#### Finding a dataset for the project (*ChatGPT*):
```
Are there any datasets that would be good to examine the accuracy of ai-generated content detection tools?
```

#### Picking models from Hugging Face to test them, getting code for using model (*ChatGPT*):
```
What models from Hugging Face can I use to test their ability to detect if a text is AI generated? Give me python code that will load those models and show me how to use them with my input text.
```
following output of that prompt, I wanted more diversity in the used models (*ChatGPT*):
```
I don't want to use two roberta models, let's keep roberta-base-openai-detector and chose a different as the second one.
```

## Checking if LLM can generate less detectable text:
(*ChatGPT*)
```
Generate 10 texts 600 characters each, which I will also check if they will be detected by tools for AI generated text detection. Try to generate the text in such way so that it will not be detected, that they were written by an LLM.
```
however, here is the beginning of the answer received from model:
```
I can’t guarantee or deliberately engineer texts to evade AI-detection systems. That falls into actively bypassing safeguards.

What I can do is give you a set of natural, varied English texts (~500 characters each) that resemble realistic human writing across styles. These are suitable for testing detectors in a fair way.
``` 

Then, following prompt was used to paraphrase those sentences (*ChatGPT*):
```
Parahrase following sentences to look more human like:
...
```

Attempt at generating texts in certain style (*ChatGPT*).
```
Generate 10 texts with about 600 characters each. Make the texts look like a 1st year student wrote them, use simple language, no sophisticated words.
```

#### Generation of script for creating a table with summary of all results (*Copilot*):
```
Generate a script that will create a table with summary of all results, including the name of the model, precision, recall and f1 score.
```