---
title: "Prompt engineering in .NET"
description: "Learn basic GPT prompt engineering for .NET."
author: catbutler
ms.author: [your Microsoft alias or a team alias]
ms.service: [the approved service name]
ms.topic: concept-article #Don't change.
ms.date: [mm/dd/yyyy]

#customer intent: As a .NET developer, I want to understand GPT prompt engineering so that I can build more efficient and effective AI chat apps.

---

# Basic prompt engineering in .NET

This article explains basic GPT prompt engineering in .NET, including the simple Completions API and the more advanced Chat Completions API. 

GPT models from OpenAI are prompt-based: they respond to user input text (a prompt) with the most likely series of words to follow (a completion). For example, in response to the prompt "The president who served the shortest term was " these models might output the completion "Pedro Lascurain". 

But what if the app is supposed to help US History students? Pedro Lascurain's 45-minute term is the shortest term for any president, but he served Mexico&mdash;the students are probably looking for "William Henry Harrsion". Clearly, your app could be more helpful if you gave it some context. That's the basic idea of prompt engineering: including extra context in your app to help it produce better completions. You can do this by giving the model instructions and examples.

You can use prompt engineering with the Completion API and the Chat Completion APIs, but there are differences in the way they support instructions and examples. The Completions API supports the GPT-3 and GPT-35 models, which have no specific format rules for prompt engineering. The Chat Completion API supports the GPT-35-Turbo and GPT-4 models, which require that prompt engineering follows a specific chat-like format. 

## Instructions

Use an instruction to tell the model how to respond. You can clarify an instruction by including primary content (a text string to process using the instruction), supporting content (text strings referenced by the instruction), and cues (text strings to use to parse and format completions). 

- You are helping students learn about US history. Unless they specifically ask about other countries, only talk about the US.

## Examples 

Use an example to show the model how to respond. An example includes a prompt paired with a partial completion (zero-shot) or a full completion (one-shot). You can improve several examples with full completions (few-shot). The model uses examples to generalize what to include in completions. 

[Describe a main idea.]

<!-- Required: Main ideas - H2

Use one or more H2 sections to describe the main ideas
of the concept.

Follow each H2 heading with a sentence about how
the section contributes to the whole. Then, describe 
the concept's critical features as you define what it is.

-->

## Related content

- [Prompt engineering techniques](https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/advanced-prompt-engineering)
- [Related article title](link.md)
- [Related article title](link.md)

<!-- Optional: Related content - H2

Consider including a "Related content" H2 section that 
lists links to 1 to 3 articles the user might find helpful.

-->

<!--

Remove all comments except the customer intent
before you sign off or merge to the main branch.

-->

