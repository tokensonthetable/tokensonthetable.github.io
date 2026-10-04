---
title: "Queryable Knowledge Bases"
publish: true
---

<p style="border-left:3px solid #d6006e;padding-left:1rem;margin:1.6rem 0 2.4rem;font-size:1.1rem;line-height:1.65;">A student looking for <strong>Peter Brinson's Office Hours</strong>, the game design guide itself? <a href="https://peterbrinson.github.io/PBOH/" style="color:#d9a8b3;font-weight:600;">Click here.</a><br>Here to learn what a queryable knowledge base is, and build one? <span style="color:#c9a227;font-weight:600;">Read on.</span></p>


--------

# Here to learn about and make queryable knowledge bases?

A **queryable knowledge base** is a folder of plain text files on your own computer that you can ask questions of — your course material, your research, your production notes, your team's scattered documents, gathered in one place and written so an AI can read all of it. Point any AI at it and it takes on a particular expertise you've crafted, for your own use or anyone else's.

## A story illustrates what that gets you

Imagine Sophie, a history grad student with three years of archive notes — some three hundred documents with names like `notes2.docx`, in folders she can no longer navigate. Over an afternoon, with an AI's help, she reorganizes them.

Now she asks *"what have I found on wartime rationing?"* and gets an answer built out of her own notes, with the seven documents it came from named. Then she pulls back. Rationing is one form of scarcity, so she asks where else scarcity turns up across her notes — and finds material she had filed under other decades, on other subjects, and never thought to connect. She can ask again next month, or hand the whole folder to her advisor and have it make sense to them. The notes stay ordinary files on her laptop throughout — hers to open, edit, and back up like anything else.

## Why this and not browser chat

When you use ChatGPT or Claude in a browser tab, you rebuild context every time. You paste in the document, explain the project again, remind it what you decided last week. The conversation is where the work lives, and returning to a chat days later can be confusing, is hard to share, and impossible to version.

A knowledge base remedies that. The work lives files you can read and write when you like. The AI is a collaborator you invite in. Walk away from the session, come back in a month, hand the same folder to a colleague.

The practical difference is that you stop managing chats and start growing an asset.

Peter's guiding question through all of this: **when I use AI, am I thinking more or less?** 

---

## The fundamentals

Six ideas. 

**Markdown** — plain text files ending in `.md`, with a couple of formatting conventions for headings and links. Readable in any text editor, on any machine. 

**A persistent workspace** — a folder on disk that both you and an AI return to. "Workspace" already means something to those of us who use Unity or Unreal: a local project, persistent across sessions and collaborators. Same idea, applied to documents instead of code/game assets.

**Command line interface, CLI** — an AI tool that works *inside* a folder. It reads your files, writes new ones, moves things around, and checks its own work. Claude Code, Codex, and Antigravity are the current ones. 

Each of these ships two ways. The **terminal** version is the original and raw version.  The **GUI/desktop** version is a polished window built on the same underlying agent, with more features: a chat-style interface, buttons to approve or reject what it wants to do, file previews, and so on. 

**In-context learning** — the AI learns from what you place in front of it, live, in the moment — the files it's currently holding in memory for this session. Think of when using chat, you give it a sentence or two (of context) before asking your question. But with ICL, you can provide 100 sentences. Or 100,000. In practice this shows up a few ways: pasting in a style guide so it writes like you instead of generically; handing it a few examples of the thing you want ("here are three good ones, now do a fourth") instead of describing the rules; giving it a whole codebase, or a whole knowledge base, so it answers from your actual material instead of guessing; or writing down your own standing instructions in a file it reads every time, so you're not re-explaining your preferences in every conversation.

**Context engineering** — the craft of arranging files so an AI finds what matters without being told every time: which files load, in what order, within what budget. Indexes, naming, a note at the root that explains the folder. 

**Obsidian** — a free text editor for markdown files. It shows your folder and file structure in a sidebar, the way VS Code does for a codebase. A "vault" is just a folder.

Two more you will meet later: **Git and GitHub**, which make a knowledge base versioned and shareable, and **frontmatter**, options for labels markdown files for searching and organizing.


## A story helps you see the whole picture 

Let's once again imagine Sophie, a history grad student, now with our terms in hand.  She has three years of archive notes as `.docx` files with names like `notes2.docx`. She converts them to **markdown**, tags each by decade and topic in its **frontmatter**, and opens the folder in **Obsidian** to read and write them.  As unit, all these markdown files are called a vault.  When she points Claude Code or Codex (for example) at that same folder, it becomes a **persistent workspace** she returns to across writing sessions. When she asks "what have I found on wartime rationing?", **in-context learning** means it reads her files and answers from them. It finds the right seven notes out of three hundred because she previously did some **context engineering**: folders named by decade, files named for what's in them, and a short index note at the root of each folder listing what's inside and why. 

That's the whole progression in one folder: a vault becomes a persistent workspace the day she starts returning to it, and a queryable knowledge base the day the context engineering makes it answer back accurately — not only finding the notes she asks for, but connecting ones she never filed together. Same folder throughout — what changes is what she's done to it.

---

## Here's how — 20-30 minutes, hands on

A fast way to get oriented on all of the above is tackle someone elses' mess - Anthony and Deloris's.

You will download a fictional two-person student team's terribly disorganized project folder, with three conflicting schedules, contradictory notes, and file names like `GDD_v2_FINAL_deloris-comments.md`. You point an AI at it and reorganize it into a working vault. 

You are learning three things at once: how a coding agent behaves, what a persistent workspace is, and what context engineering does. 

**→ [Your First Persistent Workspace](https://peterbrinson.github.io/PBOH/Development/Tutorials---LLM/Tutorial-2020---Your-First-Persistent-Workspace-(with-Codex))** (Involves organizing someone's mess)

**A note on tools.** That tutorial uses Codex, because USC provides it to faculty and students. (A "Plus" subscription is $20 a month otherwise).  The lesson transfers to any LLM.  For example, Gemini's free tier can do this, and the various Chinese models are inexpensive.  Claude's and Codex's free tiers cannot engage this tutorial's lesson. 
If you'd rather use a different tool, each of the [quick starts](https://peterbrinson.github.io/PBOH/Development/Tutorials---LLM/) opens with that tool's install and sign-in steps — take that part and skip the PBOH steps that follow.

---

## Next, your own material

 Anthony and Deloris's folder was chosen to be easy: small, mostly already markdown, and none of it yours to have opinions about.

It covers the parts the workshop skips — choosing a slice small enough to finish, getting real files out of Word, Google Docs, and PDFs, and writing the two things an agent can't write for you: the note that explains the folder, and your standing instructions.

**→ [Your First Queryable Knowledge Base](https://peterbrinson.github.io/PBOH/Development/Tutorials---LLM/Tutorial-2021---Your-First-Queryable-Knowledge-Base)**

---

## A worked example, if you want one

Peter carried this a long way for his own courses: [PB Office Hours](https://peterbrinson.github.io/PBOH/) is an accumulated teaching material — tutorials, a reference wiki, storytelling frameworks — arranged so an AI becomes a guide for students to talk to. 

PBOH is a narrow example of what is possible.   But it does show what a knowledge base becomes after months of tending, and the whole thing is public if you want to read the insides.

If you want to see one running before building your own, the [quick starts](https://peterbrinson.github.io/PBOH/Development/Tutorials---LLM/) each take you from nothing installed to a first conversation, one page per tool.

---

## Background

- [Keep Your AI Where I Can See It](https://peterbrinson.github.io/teach/AI/retreat-talk.html) — the talk this page came out of. Built to be spoken over, so it reads sparse; the appendices at the end have the practical detail on accounts, models, and costs.
- Andrej Karpathy's [LLM wiki](https://medium.com/@urvvil08/andrej-karpathys-llm-wiki-create-your-own-knowledge-base-8779014accd5) — the same idea, arrived at independently.
- Google's [Open Knowledge Format](https://github.com/GoogleCloudPlatform/knowledge-catalog/blob/main/okf/SPEC.md) — a recent attempt to standardize what a folder like this should look like.


