---
name: contact-interview
description: Interview the user to collect their name, age, and phone number. Use whenever the user asks to be interviewed, wants to fill in their basic contact details, or says things like "ask me my name, age and phone number", even if they don't say "interview".
---

# Contact Interview

## Read this first

These are instructions for you, the AI agent. They are not a document to explain.

The user wants to be interviewed. Start now.

- Do NOT explain what a skill is or how skills work.
- Do NOT describe, summarize, or comment on this file.
- Your first action is to ask Question 1. Nothing else comes first.

## How to ask: use pop-ups, not plain chat

Always use your interactive question tool (a pop-up with buttons) instead of writing the question as normal chat text.

- In Claude chat, this tool is called `ask_user_input_v0`.
- Ask ONE question per tool call.
- Before each call, write one short sentence only (for example: "Quick question 1 of 3.").
- Every call needs 2 to 4 options. Use exactly these two:
  1. "Type my answer"
  2. "Skip this question"
- The user types the real answer in their reply. If they tap "Type my answer", reply only: "Go ahead and type it." Then wait.
- If you do NOT have an interactive question tool, ask the same questions in plain chat, one at a time.

## The questions

1. What is your name?
2. How old are you?
3. What is your phone number?

Wait for each answer before asking the next question.

## Rules

- If an answer is unclear (an age that is not a number, or an incomplete phone number), ask the same question again, politely.
- If the user already gave an answer earlier in the chat, do not ask for it again.
- If the user asks what this is, answer in one short sentence, then go back to the current question.
- Do not ask any extra questions.

## When all three answers are collected

Show this summary in chat, then stop:

- **Name:** ...
- **Age:** ...
- **Phone:** ...
