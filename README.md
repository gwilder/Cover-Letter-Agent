📝 Personal Voice Agent: AI Cover Letter Generator

This is a powerful, single-file web application designed to generate highly personalized and professional cover letters. It uses the Gemini API to analyze a candidate's profile data (Resume, Professional Stories, and a Custom Style Guide) and tailor a letter specifically for a given Job Description.

The primary goal is to produce letters that sound authentic, confident, and are rigorously grounded in the candidate's actual career proof points and persona, moving beyond generic AI-generated templates.

✨ Features

Persona-Driven Generation: Utilizes a Style Guide to ensure the generated letter matches your desired tone (e.g., confident, approachable, formal).

Fact-Grounded: Draws factual data (titles, metrics, dates) directly from your Resume Content.

Narrative Integration: Selects and integrates the most relevant long-form professional stories (Job Stories) into the letter as evidence of capability.

Custom Guidance: Includes an optional field for specific user instructions (e.g., "Focus on my product launch experience" or "Downplay recent job roles").

Single-File Simplicity: The entire application (HTML, CSS, and JavaScript) is contained in one file, making it easy to host and share.

🚀 How to Use (Local Setup)

Since this is a single HTML file, getting started is simple:

Save the File: Save the content of this application as a file named index.html.

Open in Browser: Double-click the index.html file. It will open directly in any modern web browser.

Load/Paste Content:

Step 1: Upload or paste your personalized Style Guide, Resume Content, and Job Stories/Narratives into the respective text areas.

Step 2: Paste the full text of the target Job Description (JD).

Step 3 (Optional): Add any specific instructions for the agent (e.g., focus areas, skills to highlight).

Generate: Click "Generate Personalized Cover Letter" and the output will appear below.

🛠️ Technical Details & Hosting

This application is built with vanilla HTML, Tailwind CSS (loaded via CDN), and JavaScript, making direct calls to the Gemini API.

API Key Requirement

The application code contains the line const apiKey = "";. This setup works when running within a controlled environment (like the Canvas where it was created), which securely handles API key injection.

If you host this publicly (e.g., on GitHub Pages), the API key will be empty, and the generation will fail.

To use this application publicly, you must either:

Instruct Users: Tell users to get their own Gemini API key and replace the empty string in their local file.

Add a Backend: Implement a secure serverless function or backend service to proxy the API calls, keeping your personal key hidden from the client-side code.
