# RAG_Resume
The goal of this project is to help to update your resume doing the following:

** Extract the most relevant keywords from a specific Job Description
** Review the sections you want to update from your resume and rephrase them using the keywords from the JD

Some considerations of this project:
- This project is using Anthropic API to interact with Claude 3.7, so for that reason you will need to have a valid Anthropic account to be able to run this code.
- The API KEY is stored in the file called "secrets.json", once you create your Anthropic account you can generate your KEY and update this file
- You need to have the Job Description in a PDF format
- You need to create a JSON file with the sections you are interested to update from your resume, see the template called "personal_resume.json"
- You need to have your current resume as a PDF file in the same directory


Data Flow of this project
1.- The Notebook load the Antropic API as a environment variable
2.- The process reaed the Job Description file and the personal resume in PDF format
3.- Using a prompt and the Job Description, we are doing a first interaction with Claude to extract the Keywords
4.- Then we read the sections to update from the file "personal_resume.json", we will request to Claude to update section by section from this json
5.- Iterate from the different sections loaded in step 4 and request to Claude to update it using the keywords extracted
6.- In the personal_resume.json file include, as the last section, the request to create a cover letter too. This will usee keywords, the JD and the resume.
7.- All the responses will be printed and the you can copy and paste this information on your resume.

