# Guided Overlay Demo – Assignment

## Overview
This is a minimal single-page demo where a user uploads a recorded-steps JSON and receives step-by-step guidance via an overlay.  
When selectors are missing, the flow resolves them using an LLM stub that maps natural-language targets to DOM elements (labels, placeholders, innerText, options).  

## How to Run
```bash
npx http-server ./public -p 8080 --cors
# then open http://localhost:8080/task.html
