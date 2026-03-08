---
type: workflow
id: onboarding-setup-pipeline
title: Onboarding Setup Pipeline
description: "Generates personalised onboarding materials and interview questions"
tags: [Production]
connections:
  - target: markdown-formatting
    type: uses
  - target: interview-question-generator
    type: uses
---

## Overview

This workflow generates personalised onboarding materials for new team members, including tailored interview questions and formatted documentation.

## Pipeline Stages

### Stage 1: Generate Questions

Invoke the **interview-question-generator** prompt to produce role-specific technical interview questions based on the position and required topics.

### Stage 2: Format Materials

Invoke the **markdown-formatting** skill to ensure all generated onboarding materials are clean, well-structured, and consistent with company documentation standards.

## Output

Personalised onboarding pack containing:

- Technical interview questions with expected answers
- Role-specific onboarding checklist
- Formatted documentation ready for distribution
