# 🤖 Copilot Prompt List (Dataverse + Power Automate Project)

This file contains all prompts used with Microsoft Copilot while building:

- The Dataverse Table (`Prompt_Task`)
- The Power Automate Flow (`Daily Prompt from Task_Prompt`)
- Supporting logic such as email content, status updates, and recurrence setup

---

## 🟦 1. Dataverse Table Creation Prompts

**Prompt Example:**
> “Create a Dataverse table named *Prompt_Task* that will store daily tasks with columns: TaskName, Status, OwnerEmail, Date, Notes.”

**Follow-up prompts:**
- “Add a Status column with options Pending, Completed, Notified.”
- “Make OwnerEmail a text field.”
- “Add a Date column for scheduling the task.”
- “Add a multiline text Notes column.”

---

## 🟪 2. Power Automate Flow Generation Prompts

**Initial prompt:**
> “Create a Power Automate flow that runs daily and reads rows from the Prompt_Task Dataverse table.”

**Enhancement prompts:**
- “Add a recurrence trigger at 8:00 every morning.”
- “List rows from the Prompt_Task table.”
- “Add a Compose action to build the email body using fields from Dataverse.”
- “Send an email using OwnerEmail from the row.”
- “Update the row after sending email and set Status to Notified.”

---

## 🟧 3. Logic / Optimization Prompts

- “Add a filter so only rows where Status = ‘Pending’ are processed.”
- “Format the email in HTML with line breaks.”
- “Use dynamic content for TaskName and Notes.”
- “Update the Date field after task is processed.”

---

## 🟨 4. Export & Packaging Prompts

- “How do I export my flow and Dataverse table into a solution?”
- “Show me how to add existing flow into a solution.”
- “Explain how to upload everything to GitHub with folder structure.”

---

## ✅ Summary

These prompts allowed building the entire automation with minimal manual editing.  
Together, they document a reproducible low‑code solution powered by Copilot.