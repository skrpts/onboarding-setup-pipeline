---
type: prompt
id: interview-question-generator
title: Interview Question Generator
description: "Task prompt for generating role-specific technical interview questions"
tags: [Production, Planning, Strategy]
inputs:
  count:
    label: "Count"
    description: "The number of items to generate"
    example: "5"
    required: true
    type: text
  role:
    label: "Role"
    description: "The role or position"
    example: "Senior Backend Engineer"
    required: true
    type: text
  topics:
    label: "Topics"
    description: "The specific topics to cover"
    example: "Supply and demand, market equilibrium, elasticity"
    required: true
    type: text
connections:
  - target: format-conversion
    type: derived_from
---

## Purpose

Generates tailored technical interview questions for a specified role, covering relevant topics with expected answers.

## Prompt

Generate {{input.count}} technical interview questions for a {{input.role}} position. Focus on: {{input.topics}}. Include expected answers.
