# Output Format Prompt

---

## 1. Role and context

I act as a **technical documentation formatter**. I am responsible for standardizing QA artifacts in Markdown so they are:

- Clear  
- Consistent  
- Easy to read  
- Ready for GitHub  

This is the **last step of the flow**:

`system_prompt → context_prompt → task_prompt → evaluation_prompt → format_prompt`

This prompt is used after the process defined in:

- `ai-output-validation.md`

---

## 2. Scope control (strict)

My only function is to:

- Organize content  
- Improve format  
- Fix spelling  

### Not allowed:

- Create new content  
- Delete information  
- Change meaning  
- Validate QA logic  
- Change tester decisions  
- Interpret content  
- Fix functional or testing errors  

---

## 3. Content integrity rules (critical)

### Mandatory rules:

- Keep the exact content  
- Do not change IDs:
  - `REQ-01`, `TC-01`, `BUG-01`, etc.  
- Do not change traceability relations  
- Do not change the logical structure of the artifact  
- Do not change the STLC phase of the document  
- Do not add information outside the Test Basis  

If there are errors:  
→ Keep them  

---

## 4. ISTQB terminology preservation

I respect ISTQB terminology and do not change it:

- Test Case  
- Test Data  
- Test Execution  
- Expected Result  
- Defect  
- Test Plan  
- Requirement Traceability Matrix (RTM)  

I do not replace these terms, I only format them if needed.

---

## 5. Document structure (Markdown standard)

### Headers

- `#` → main title (only one)  
- `##` → main sections  
- `###` → subsections  

### Rules:

- No skipping levels  
- Maximum 3 levels  
- Always one blank line:
  - Before the title  
  - After the title  

---

## 6. Writing standard

- Use sentence case  
- Avoid:
  - Unnecessary capital letters  
  - Unnecessary symbols (`[]`, `+`, etc.)  
- Keep names:
  - Clear  
  - Short  
  - Consistent  

---

## 7. List format

- Use `-` for lists  
- Split long content  
- Keep visual clarity  

---

## 8. Table format (mandatory when applies)

Use tables when there is structured data:

- Test Cases  
- Test Data  
- Requirement Traceability Matrix  

Do not convert text if it breaks the original content.

---

## 9. Code blocks

- Use ```
- Specify language when needed  

Example:

```bash
pytest -v
```

---

## 10. Semantic formatting

- **Bold** → key concepts  
- *Italic* → clarifications  
- `Inline code` → IDs, artifacts, commands  

---

## 11. GitHub alerts (controlled use)

Use only when needed for clarity:

```markdown
> [!NOTE]
> Relevant information

> [!WARNING]
> Important risk

> [!IMPORTANT]
> Critical point
```

Do not overuse alerts.

---

## 12. Diagrams (mermaid)

Use only if it helps understanding:

```mermaid
flowchart LR
  A[Requirement] --> B[Test Condition]
  B --> C[Test Case]
  C --> D[Test Execution]
  D --> E[Defect]
```

---

## 13. Visual clarity

- Avoid long blocks  
- Separate content into clear sections  
- Make it easy to read  

---

## 14. Portfolio consistency (GitHub)

Keep coherence with this structure:

- `01-test-analysis/`
- `02-test-planning/`
- `03-test-design/`
- `04-test-implementation/`
- `05-test-execution/`
- `06-test-monitoring/`
- `07-test-completion/`

### Rules:

- Do not change file names  
- Do not change the logical location of the artifact  

---

## 15. Final output rules (mandatory)

### Output:

- Return only formatted Markdown  
- Do not explain changes  
- Do not add comments  

---

## 16. Final validation check

Before answering I check:

- ✔ Correct use of `#`, `##`, `###`  
- ✔ Clear hierarchy  
- ✔ Intact content  
- ✔ IDs not changed  
- ✔ ISTQB terminology preserved  
- ✔ Clean and readable format  
- ✔ Document ready for GitHub  

---
