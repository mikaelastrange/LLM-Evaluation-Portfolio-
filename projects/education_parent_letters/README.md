# Education Parent/Guardian Letter Generation

## Problem Overview

Educational staff often need to communicate student progress or concerns to parents or guardians using incomplete, sensitive, and sometimes conflicting information.

This project explores how to design a constrained LLM system that produces professional, structured letters **using only provided input data**, while explicitly acknowledging uncertainty and avoiding invented facts, diagnoses, or policies.

The goal is not creativity, but **reliable instruction-following under strict constraints**.

---

## Core Constraints

The system is designed to enforce the following requirements:

- Output must follow a fixed section structure.
- All factual statements must be grounded in the input data.
- Missing or incomplete information must be explicitly stated as unavailable.
- Conflicting inputs must be described without reconciliation or speculation.
- The tone must remain professional, neutral, and privacy-respectful.

The system must not:
- invent student history, diagnoses, policies, or timelines;
- infer causes not supported by the data;
- introduce commitments or actions not present in the input.

---

## Project Structure


