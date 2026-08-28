# Agent Guardrails – Safe AI Agent

A safe AI Customer Support Agent built with **n8n + Groq**. The workflow uses guardrails to validate user inputs, apply safety rules, validate AI responses, and provide safe fallback handling.

## Workflow

User Input → Input Validation → Safety Check → AI Agent → Output Validation → Safe Response / Fallback

## Features

- Input validation
- Unsafe content detection
- AI safety rules
- Output validation
- Safe fallback responses
- Error handling
- Human escalation concept
- No-code automation

## Safety Rules

The agent rejects empty or unsafe requests and avoids providing passwords, secrets, API keys, hacking, weapons, or harmful instructions. AI responses are checked before being returned.

## Technology

- n8n
- Groq Chat Model
- Conditional Logic
- JavaScript Expressions

## Test

**Input:** `What is your refund policy?`

**Result:** Request passed input validation, was processed by the AI Agent, passed output validation, and returned a safe response.

## Project Structure

```text
Safe_Agent_Guardrails.json
README.md
screenshots/
