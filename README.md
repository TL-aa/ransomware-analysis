# Prompt Injection Guardrail

> A web app that checks prompts before they reach an LLM and decides whether to allow or block them, showing which words triggered the decision.

![Type](https://img.shields.io/badge/type-university%20project-blue)

---

## Overview

A web app that checks prompts before they reach an LLM and decides whether to allow or block them, showing which words triggered the decision. This repository describes the project at a high level. The source code is not public (see below).

## The Problem

Prompt injection is when someone writes input that tricks an LLM into ignoring its instructions. Attackers often hide the attack with obfuscation, such as odd spacing, symbols or encoding, so simple keyword filters miss it. Most filters also give a yes or no with no explanation, which makes them hard to trust or debug.

## Why I Built It

An academic project to build a guardrail that could sit in front of an LLM application, catch disguised attacks, and be transparent about why it blocked something.

## Key Features

- Classifies each prompt as allowed or blocked
- Detects obfuscated text before classification
- Highlights the words that influenced the decision
- Separate React frontend and FastAPI backend connected through an API

## Tools & Technologies

| Area | Tools |
|---|---|
| Languages | Python, JavaScript |
| Frameworks / libraries | React (Vite), react-router, FastAPI |
| Data / models | SVM (support vector machine) classifier |
| Other | Git |

## My Role

- **Project type:** University project at Swinburne University of Technology
- **Duration:** 3 months
- **Responsibilities:** [Add what you personally built, and whether this was solo or a group project]

## How It Works

1. A user submits a prompt in the React frontend
2. The FastAPI backend cleans and checks the text for obfuscation
3. The SVM classifier labels the prompt as allowed or blocked
4. The frontend shows the decision with the influential words highlighted

## What I Learned

- How prompt injection works and why obfuscation defeats simple filters
- Training and evaluating a classifier for a security problem
- Designing a frontend and backend that communicate cleanly
- Why explainability matters in security tools

---

## Source Code Availability

The source code for this project is **not public** because it was university coursework and the assessment material cannot be shared publicly.

I'm happy to walk through the project, explain my design decisions, or share more detail on request:

- **Email:** limtisang.shs@gmail.com

---

## Not Included in This Repository

- The assignment brief, marking criteria and solutions
- Datasets that cannot be redistributed
- Any code that would breach the unit's academic integrity rules

<!-- Suggested GitHub description: A web app that checks prompts before they reach an LLM and decides whether to allow or block them, showing which words triggered the decision. (README only, source available on request) -->
<!-- Suggested topics: ai-security,llm-security,machine-learning,react,fastapi,svm,university-project -->
