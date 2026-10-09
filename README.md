# GEN-AI-BUSINESS-ANALYST-ASSISTANT
# AI Business Analyst Assistant

## Overview

The **AI Business Analyst Assistant** is a Generative AI project built using Python, Google's Gemini API, and Pandas. It helps streamline the business analysis process by transforming natural-language business requirements into structured BA documentation.

The project uses hotel management software scenarios to demonstrate how AI can support requirement analysis, functional requirement definition, Agile user story creation, acceptance criteria preparation, and test scenario generation.

## Business Problem

Business Analysts frequently spend time translating stakeholder requirements into clear, structured documentation for product, development, and QA teams. This project explores how Generative AI can assist with this process while explicitly identifying assumptions and missing information that may require clarification.

## Key Features

* **Requirement Summary:** Converts business requirements into concise summaries.
* **Functional Requirements:** Generates structured functional requirements from business needs.
* **Agile User Stories:** Creates user stories using the standard "As a / I want / So that" format.
* **Acceptance Criteria:** Generates acceptance criteria using the Given–When–Then format.
* **Test Scenarios:** Suggests basic scenarios for validating the requested functionality.
* **Assumption Identification:** Highlights assumptions and missing information that require stakeholder clarification.
* **Batch Analysis:** Processes a sample dataset containing eight hotel business requirements.
* **CSV Export:** Saves the original requirements and generated analysis for further review.

## Technology Stack

* Python
* Google Gemini API
* Google Gen AI SDK (`google-genai`)
* Pandas
* Google Colab
* Prompt Engineering
* CSV

## Project Workflow

1. Load the sample hotel business requirements into a Pandas DataFrame.
2. Select an individual requirement or enter a new requirement.
3. Construct a structured prompt using Business Analyst terminology.
4. Send the prompt to the Gemini API.
5. Generate requirement summaries, functional requirements, user stories, acceptance criteria, test scenarios, and assumptions.
6. Store the analysis alongside the original requirement.
7. Export the resulting dataset to CSV for review.

## Sample Use Case

**Input Requirement:**

Customers should be able to cancel their hotel bookings through the mobile application.





