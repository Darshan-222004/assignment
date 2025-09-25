# Guided Overlay Demo – Assignment

This is my submission for the Guided Overlay Demo assignment.  
The app lets a user upload a `steps-recorded.json` file, and shows step-by-step guidance with an overlay.  
If selectors are missing, a local LLM stub maps natural-language targets to DOM elements (labels, placeholders, text).  

To run:  
```bash
npx http-server ./public -p 8080 --cors
# open http://localhost:8080/task.html
