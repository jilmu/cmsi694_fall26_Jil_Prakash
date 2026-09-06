# cmsi694_fall26_Jil_Prakash
Visa_Path

# VisaPath

**A multi-agent AI system for answering specific visa and immigration questions, grounded in official government data.**

> Status: Early-stage / planning. This repo currently holds the idea and initial approach — implementation hasn't started yet.

## The Problem

Generic AI chatbots are often used to answer visa and immigration questions, but they rely on general training knowledge that can be outdated, incomplete, or simply wrong. Immigration rules change frequently and the stakes for getting an answer wrong are high. There's a need for a tool that answers narrow, specific visa questions using current, verifiable government sources instead of guesswork.

## The Idea

VisaPath will be a multi-agent AI system where distinct agents each handle one part of the problem instead of a single model trying to do everything:

- **Retrieval agent** — pulls relevant, current information from scraped official government immigration sources
- **Interpretation agent** — parses the user's specific situation (visa type, country, circumstances) to figure out what's actually being asked
- **Composition/verification agent** — drafts the answer and checks it against the retrieved source material before returning it

The goal is an answer that's traceable back to an actual government source, not something the model generated from memory.

## Planned Tech Stack

- **FastAPI** — API layer
- **LangGraph** — multi-agent orchestration
- **Celery** — async task processing
- **Docker Compose** — containerized deployment

*(Subject to change as the design develops.)*

## Who This Is For

People navigating visa and immigration processes who need fast, trustworthy answers to specific questions — without relying on generic chatbots or expensive/slow professional consultations.

## Goals / Success Criteria

- Answers are grounded in current, scraped government data — not model priors
- The system reliably handles a defined set of specific visa question types
- End-to-end demonstrable: a user asks a question, gets a sourced answer

## Current Status

- [x] Idea defined
- [x] Initial approach sketched out
- [ ] Architecture design
- [ ] Scraping pipeline
- [ ] Agent implementation
- [ ] Evaluation against test questions

## Roadmap

This project is being developed as part of a course project. More detail will be added here as the design and implementation progress.
