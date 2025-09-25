# Guided Overlay Demo – Assignment

This is a single-page demo where a user can upload a JSON file (`steps-recorded.json`) and see step-by-step guidance overlaid on the form. The overlay shows the current step, highlights the correct element, and lets you move through the flow with Next/Prev/Reset buttons.  

## How to Run
```bash
npx http-server ./public -p 8080 --cors
# then open http://localhost:8080/task.html
