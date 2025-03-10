# Resume Enhancement with RAG Logic

## Overview

This project implements a Retrieval-Augmented Generation (RAG) approach using Claude 3.7 to enhance a personal resume by aligning it with a given job description. The model extracts relevant keywords and updates specific resume sections based on predefined instructions.

## Features

Reads the job description and personal resume from PDF files.

Extracts relevant keywords from the job description using Claude 3.7.

Uses a resume.json file to determine which sections of the resume need updating.

Iterates through each section and updates it using AI-driven text refinement.

Generates a new cover letter that aligns with the job description.

Uses a secrets.json file to store the Anthropic API key securely

## Dependencies

Ensure you have the following libraries installed before running the notebook:
pip install pypdf anthropic json

## Steps

Load PDFs: Extract text from the job description and resume.

Extract Keywords: Call Claude 3.7 to retrieve key terms from the job description.

Read resume.json: Identify sections to update and their specific instructions.

Iterate and Update: Process each section, sending requests to Claude 3.7 to refine the text.

Generate Cover Letter: Craft a tailored cover letter based on the updated resume.

## Usage

Run the Jupyter Notebook (main.ipynb) and ensure the necessary files (resume.json, secrets.json, PDFs) are in the project directory.


## Security Considerations

The API key for Claude 3.7 is stored in secrets.json. Do not share this file.

Ensure the job description and resume files are correctly formatted to avoid parsing errors.

## Future Enhancements

Add support for multiple job descriptions.

Improve AI prompt engineering for better alignment with job roles.

Introduce an interactive UI for resume customization.

## Author

Gerardo Tapia
