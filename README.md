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

**Expected Output Sections:**

1. Requirement Summary
2. Functional Requirements
3. Agile User Story
4. Acceptance Criteria
5. Test Scenarios
6. Assumptions and Clarifications

The generated output should be reviewed by a Business Analyst before being used as a final business specification.

## Dataset

The project includes eight sample hotel business requirements covering:

* Booking
* Payment
* Housekeeping
* Reporting
* Customer management

The sample dataset is used to demonstrate requirement processing and AI-assisted documentation.

## Setup and Execution

This project was developed for Google Colab.

1. Open the notebook in Google Colab.
2. Install the required Python dependencies.
3. Configure a Gemini API key in Colab Secrets using the name `GEMINI_API_KEY`.
4. Ensure the key has access to the selected Gemini model.
5. Run the notebook cells in order.
6. Enter a business requirement when prompted.
7. Review the generated analysis and exported CSV files.

### Dependencies

* `google-genai`
* `pandas`

The original notebook also pins certain package versions. Use the dependency versions documented in the notebook if compatibility issues arise.

## Security

Do not hard-code or commit API keys, credentials, or other secrets. Store the Gemini API key securely using Colab Secrets or an appropriate environment-variable-based configuration.

## Limitations

* AI-generated documentation may contain inaccuracies and requires human validation.
* Acceptance criteria and test scenarios depend on the clarity and completeness of the input requirement.
* Business rules, edge cases, and non-functional requirements may need further stakeholder clarification.
* The current implementation demonstrates a command-line workflow in Colab rather than a deployed web application.

## Future Enhancements

* Build a Streamlit interface for interactive requirement analysis.
* Add export options for BRD and FRD documents.
* Support batch uploads of requirements from CSV or Excel.
* Add requirement traceability between business requirements, user stories, and test cases.
* Introduce validation checks and human review before approving generated documentation.

## Author

Developed as a portfolio project to explore the practical application of Generative AI in Business Analysis and requirements engineering.
