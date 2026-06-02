# Documentation Automation Projects

## Why I Built These

Manual documentation work doesn't scale. When your knowledge base has 
700+ articles maintained by different people, you can't rely on 
ctrl+F and gut instinct. These two projects helped me and my team work 
smarter, and both started with a simple question:

> "Can we automate this instead?"

---

## Project 1: Rebranding Terminology Audit

### The Problem
Our product was being rebranded. One legacy product term needed 
to be found and flagged across 900+ public Help Center articles.

Doing this manually meant opening each article, reading it, and 
checking if the old name appeared in the title, body, or as a 
reference. For one person, that could mean days of manual review.

### What I Did
I used AI-assisted code generation to develop a Python workflow that:
- Retrieved publicly available Help Center articles
- Searched for the old brand name in three places: article title, 
  body text, and internal references
- Generated a CSV listing every article where the term appeared

### The Result
The workflow identified more than 100 affected articles within 
minutes, significantly reducing manual review effort during the 
rebranding initiative. I could immediately see which articles 
needed updating and prioritize accordingly.

### A Note on Ethics
No confidential data was used. The workflow only accessed publicly 
available articles. I shared prompts with the AI, not company data.

---

## Project 2: Internal Knowledge Base Audit for AI Chatbot Readiness

### The Problem
Our internal knowledge base, 800 articles written by multiple 
contributors, was being connected to an AI support chatbot.

For a chatbot to give accurate answers, the articles feeding it 
need to be clean, current, and the right length. But we had a 
visibility problem:

- Who owns which article?
- Which articles are too long or too short?
- Which ones are outdated and should be retired?

Zendesk does not generate this report natively. My manager needed 
the data, and needed it fast.

### What I Did
I used AI-assisted code generation to develop a Python workflow that 
connected to the Zendesk API and pulled metadata for every article 
in our internal knowledge base:

- Article title
- Owner name
- Word count
- Last updated date

The output was a structured Excel report the team could sort, 
filter, and act on immediately.

### The Result
The report gave us full visibility for the first time. The team used 
it to:
- Retire outdated articles that were confusing the chatbot
- Identify articles that needed to be shortened for better retrieval
- Assign edit access to the right people
- Prioritize content cleanup before the chatbot went live

### A Note on Ethics
I used AI only to generate the code, not to process any article 
content. No company data was shared with any external AI tool. The 
workflow ran locally using our own API credentials.

---

## What These Projects Showed Me

Good documentation is not just about writing clearly. It is about 
understanding the systems your content lives in and finding ways to 
make those systems work better.

Both projects started with a documentation problem. Both ended with 
a tool that made the whole team more effective.

That is the kind of documentation problem-solving work I enjoy most.
