---
type: prompt
id: interview-question-generator
title: Interview Question Generator
description: "Task prompt for generating role-specific technical interview questions"
tags: [Production]
connections:
  - target: markdown-formatting
    type: derived_from
---

## Purpose

Generates tailored technical interview questions for a specified role, covering relevant topics with expected answers.

## Prompt

Generate {{input.count}} technical interview questions for a {{input.role}} position. Focus on: {{input.topics}}. Include expected answers.
