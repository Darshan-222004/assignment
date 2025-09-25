
---

## 📄 Final `PROMPTS.md`
```markdown
# LLM Mapping – Prompt / Stub

For this assignment, I used a **stub resolver** instead of a live LLM API.  
The stub inspects target text (e.g., "Full name field") and matches it with DOM inventory (labels, placeholders, IDs, options).

---

## Stub Example
Input → `target_text: "Full name field"`  
DOM Inventory → `[ {id:"full_name", label:"Full name"} ]`  
Stub Output → `#full_name`

Console log shows:
