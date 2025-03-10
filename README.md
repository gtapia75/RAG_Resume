Resume Enhancement with RAG Logic

Overview

This project implements a Retrieval-Augmented Generation (RAG) approach using Claude 3.7 to enhance a personal resume by aligning it with a given job description. The model extracts relevant keywords and updates specific resume sections based on predefined instructions.

Features

Reads the job description and personal resume from PDF files.

Extracts relevant keywords from the job description using Claude 3.7.

Uses a resume.json file to determine which sections of the resume need updating.

Iterates through each section and updates it using AI-driven text refinement.

Generates a new cover letter that aligns with the job description.

Uses a secrets.json file to store the Anthropic API key securely
