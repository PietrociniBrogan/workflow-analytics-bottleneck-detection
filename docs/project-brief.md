# Project Brief

## Project Name

Workflow Analytics and Bottleneck Detection Platform

## Objective

Build a portfolio project that ingests workflow event data, models how work moves through a multi-stage process, and identifies bottlenecks, delays, reopen patterns, backlog, and on-time completion performance.

## Business Problem

Organizations often have workflows that move through multiple stages, but leadership cannot easily answer:

- where work gets stuck
- how long each stage takes
- who is overloaded
- how often items are reopened
- which items miss expected completion targets

## MVP Scope

This first version will:

- ingest sample workflow data from CSV/JSON
- validate and normalize the data
- model workflows, events, owners, and findings/issues
- produce metrics for cycle time, backlog, reopen rate, and on-time completion

## Out of Scope

For version 1, this project will not include:

- a production UI
- real external system integrations
- complex auth implementation
- advanced forecasting/ML
- enterprise-scale infrastructure

## Core Entities

- workflows
- workflow_events
- owners
- issues_or_findings

## Initial Metrics

- workflow cycle time
- stage cycle time
- backlog count
- reopen rate
- on-time completion rate

## Constraints

- data will initially be synthetic but realistic
- project should be explainable in interviews
- work will be built incrementally over time
- project artifacts must be committed to GitHub regularly

## Success Criteria

- clean repo history
- documented schema and metrics
- working Python ingestion script
- meaningful SQL metrics
- portfolio-ready README and walkthrough
