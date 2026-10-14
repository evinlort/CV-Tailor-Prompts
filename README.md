# Create a CV for one job

Use these prompts to make a CV for a job you want. Start with a job link and your saved skills and CV files. The result is a CV PDF for that job.

There are two steps:

1. **Check the job fit.** Compare the job with your real skills. Save the result as a Fit Audit file.
2. **Create the CV.** Start with `General_CV.md` as your base CV. Use the audit to choose changes. Add relevant facts from `Master_Skills.md`. Save and check the new CV as a PDF.

Start here, then choose one way to work:

- [Before you start](#before-you-start)
- [Choose a model and effort](#choose-a-model-and-effort)
- [ChatGPT or Claude](#use-chatgpt-or-claude)
- [Codex or Claude Code](#use-codex-or-claude-code)

## Before you start

Have these ready:

- `Master_Skills.md`: your skills, work, projects, and results.
- `General_CV.md`: your base CV. The app will use it as the starting point for each tailored CV.
- A link to one job, from LinkedIn, a company website, or a job board.

This guide starts after you have made the two files. If you do not have them, use [Create-Master-Skills-and-General-CV-Markdowns.md](Create-Master-Skills-and-General-CV-Markdowns.md) first.

Keep your personal files in a private folder. Do not add them to this prompt repository.

### Check the skills filename

Use `Master_Skills.md` for both the job fit check and CV creation. Keep the spelling and capital letters exactly as shown. Use the same file in both projects.

### Set your name and languages

Make a private copy of [MASTER_PROMPT_CV_Tailoring_From_Fit_Audit.md](MASTER_PROMPT_CV_Tailoring_From_Fit_Audit.md). Open it in a text editor.

At the top:

1. Replace `USERNAME` in `CANDIDATE_FULL_NAME` with your full name. It must match your CV.
2. Change `LANGUAGES_LINE` to your real languages and levels. The saved line is an example, not your personal data.
3. Keep `CV_LANGUAGE: "English"` if you want an English CV.
4. Save the file with the same filename.

Use this edited copy in the steps below.

### How the files work together

Start with `General_CV.md`. Keep your correct name, contact details, work history, dates, and education. Change the summary, skills, and work descriptions to fit the job. Use `Master_Skills.md` for more facts about your real work. Use the Fit Audit to decide which facts matter for this job.

Save the tailored CV as a new file. Keep `General_CV.md` for the next job.

## Choose a model and effort

Effort means how much time the model spends thinking. More effort can help with hard checks, but takes longer and uses more of your limit.

These are suggested starting points for this workflow, checked on **14 October 2026**. They are not results from a CV model test. Your account may show different choices.

| Tool | Suggested model | Effort |
| --- | --- | --- |
| ChatGPT, in Chat mode | An available model with thinking and file tools. | Start with the default; increase thinking time for the audit and final CV checks if offered. |
| ChatGPT, in Work mode | GPT-6.1 Sol | Medium; use High if the files are long or facts disagree. |
| Claude | Sonnet 5.5 | High for the audit and final CV checks. |
| Codex | GPT-6.1 Sol | High for reading files, making the PDF, and checking it. |
| Claude Code | Sonnet 5.5 | High for the same steps. |

In ChatGPT Chat mode, use the model picker if your account offers one. Choose a model with thinking and file tools, and adjust its thinking time if that control is available. Model names and controls vary by account; the Work settings below do not necessarily apply. Use Chat for questions, comparing the job with your experience, and revising CV text. For creating and checking the finished PDF, switch to Work. See [Chat and Work guidance](https://learn.chatgpt.com/docs/use-chatgpt).

In ChatGPT Work, open the model control below the message box. Use **Advanced** if needed. GPT-6.1 Sol is available in Work and Codex, not ordinary Chat mode. In Codex CLI, use `/model` to choose the model and effort. See the [OpenAI model guide](https://learn.chatgpt.com/docs/models).

In Claude, click the model name near the send button, then choose **Effort**. Sonnet 5.5 already has thinking on. See [Claude model and effort settings](https://support.claude.com/en/articles/8664678-change-the-model-effort-and-thinking-settings).

In Claude Code, use `/model` and `/effort high`. See [Claude Code model settings](https://code.claude.com/docs/en/model-config).

If these models are missing, use an available model with thinking and file tools. For a harder case, try Astra in ChatGPT Work or Codex, or Opus in Claude. Start with its default effort. A stronger model still needs correct source files.

## Use ChatGPT or Claude

Set up two projects once. Then use a new chat in each project for each job.

Once the project instructions and required files are in place, send **only the job URL** in a new **CV FIT AUDIT** chat, or attach **only the full Fit Audit document** in a new **CV TAILOR** chat. No extra prompt text is required. The example messages below are optional.

### 1. Create the audit project

In your chosen app, create a private project called **CV FIT AUDIT**.

| App | Where to put instructions | Where to add files |
| --- | --- | --- |
| ChatGPT | Open the project settings and add project instructions. | Add files to the project sources. |
| Claude | Open the project and choose **Set project instructions**. | Add files to **Project knowledge**. |

For help, see [ChatGPT projects](https://learn.chatgpt.com/docs/projects) or [Claude projects](https://support.claude.com/en/articles/9519177-how-can-i-create-and-manage-projects).

Copy all the text from [CV-FIT-AUDIT-Project-Instructions.md](CV-FIT-AUDIT-Project-Instructions.md) into the project instructions.

Add these three files to the project:

- [CV_Fit_Audit_Protocol.md](CV_Fit_Audit_Protocol.md)
- Your `Master_Skills.md`
- Your `General_CV.md`

The instruction text goes in the settings. The three files go in the file area.

### 2. Send the job link

Start a new chat inside **CV FIT AUDIT**. Choose the model and effort above. Allow web access if the app asks for it.

Send only the job URL to start the audit. If you prefer a fuller message, use this optional example and replace `[JOB LINK]` with the real link:

```text
Check my fit for this job: [JOB LINK]

Read the project instructions, CV_Fit_Audit_Protocol.md,
Master_Skills.md, and General_CV.md in full.
If a required file is missing or cannot be read, stop and tell me.
Use simple English for your questions and report.
Ask no more than three questions at a time.
Use only facts from my files and my answers about my experience.
Create the full Fit Audit, with the CV Builder Prompt.
Do not create the final CV yet.
```

If the app cannot open the job link, open it yourself. Copy the full job text into the chat. Include the company, job title, tasks, and requirements. Keep the original link in your message.

Answer any questions with real facts. Say “I do not know” when needed.

### 3. Read and save the audit

Check the report. It should explain:

- How your skills match the job.
- What your general CV already shows.
- What a new CV can show more clearly.
- Which job requirements you do not meet, or still need to check.
- What the CV writer should change, in the **CV Builder Prompt**.

Scores are rough estimates. They are not results from the employer's hiring software, often called an ATS.

If the report says **HOLD**, read the reason. Answer the missing questions or choose another job before you continue.

Save the whole report as:

```text
Company_Position_CV_Fit_Audit_YYYY-MM-DD.md
```

Use the real company, job title, and date. If there is no download button, copy the full report into a text file and save it with `.md` at the end.

### 4. Create the CV project

Create a second private project called **CV TAILOR**.

Copy all the text from [CV_TAILOR-Project-Instructions.md](CV_TAILOR-Project-Instructions.md) into its project instructions.

Add these files to the project:

- Your edited `MASTER_PROMPT_CV_Tailoring_From_Fit_Audit.md`
- Your `Master_Skills.md`
- Your `General_CV.md`

Use a mode that can create files and run code to check a PDF. [ChatGPT Work can create PDFs](https://learn.chatgpt.com/docs/web). In Claude, enable file creation and code execution if your account offers them.

### 5. Ask for the CV PDF

Start a new chat inside **CV TAILOR**. Attach the full audit from step 3. Do not attach only its summary.

The full Fit Audit attachment is enough to start tailoring; no accompanying message is required. If you prefer, add this optional message:

```text
Use General_CV.md as the base CV. Tailor it for the job
in the attached Fit Audit.

Read the project instructions, the full master prompt,
Master_Skills.md, General_CV.md, and the attached audit.
If a required file is missing or cannot be read, stop and tell me.

Use the audit for the job details and suggested changes.
Keep the correct personal details and work history from General_CV.md.
Use Master_Skills.md to add relevant, supported facts.
Save the tailored CV as a new file. Do not change General_CV.md.
Use the tailoring master prompt for the final output: a real PDF.
If the audit asks for Markdown, follow the PDF rule for this step.

Use my configured name and language line.
Write the CV in natural, professional English.
Use simple English for your questions and short report.
Ask no more than three questions at a time.
Do not invent skills, work, or results.

Check the facts, job fit, PDF text, every page, and PDF metadata.
Give me the PDF and say which checks you completed.
If a tool is missing, say which check you could not do.
```

The final filename follows this pattern:

```text
Your_Name_Company_Position_CV.pdf
```

If the app cannot make or check the PDF, continue in Codex or Claude Code with the same files. A text draft alone does not finish this workflow.

### 6. Check the PDF before you send it

Download and open the PDF.

PDF metadata is the file's saved information, such as its title and author.

- Check your name, contact details, dates, job titles, and languages.
- Read each work claim. Make sure you can explain it in an interview.
- Check every page for cut text, strange spaces, or empty pages.
- Try to select and copy the text. Check that it stays in the right order.
- Read the app's check report. The PDF `Author` and `Creator` fields should show your name.

Ask for fixes if needed. The app must check the changed PDF again. Send the CV only when you have read it.

For the next job, keep both projects. Start a new audit chat with the new link. Then start a new CV chat with the new audit.

## Use Codex or Claude Code

Use this path if you want the agent to read and write files on your computer. You need Codex or Claude Code installed and signed in.

### 1. Prepare a private folder

Create a folder outside this repository. Copy the files into this layout:

```text
cv-work/
  audit/
    CV-FIT-AUDIT-Project-Instructions.md
    CV_Fit_Audit_Protocol.md
    Master_Skills.md
    General_CV.md
  tailor/
    CV_TAILOR-Project-Instructions.md
    MASTER_PROMPT_CV_Tailoring_From_Fit_Audit.md
    Master_Skills.md
    General_CV.md
  output/
```

Use the same candidate facts in both folders. Set your name and languages in the master prompt, as shown above.

### 2. Open the agent

Open a terminal in `cv-work`. Run one command:

```bash
codex
```

Or:

```bash
claude
```

Choose the model and effort from the table above. In the Codex app, you can open the folder and start a local task instead.

The agent needs to read these folders, write to `output/`, and use tools to make and check a PDF. It also needs the job text or access to the job page.

### 3. Run the audit

Replace `[JOB LINK]`, then send:

```text
Check my fit for this job: [JOB LINK]

Read and follow audit/CV-FIT-AUDIT-Project-Instructions.md
and audit/CV_Fit_Audit_Protocol.md.
For this local task, use the files in audit/ as Project Sources.
Read audit/Master_Skills.md and audit/General_CV.md in full.
If a required file cannot be read, stop and name it.
If you cannot read the exact job page, ask me for its full text.
Use simple English. Ask no more than three questions at a time.
Link each important claim to the job text, my files, or my answers.
Do not invent facts or change my source files.

Save the complete audit, including the CV Builder Prompt, as
output/Company_Position_CV_Fit_Audit_YYYY-MM-DD.md.
Use the real company, position, and date in the filename.
Stop after the audit. Do not create the CV yet.
```

Answer the questions. Open the saved audit and check it as in step 3 of the chat guide. Resolve any **HOLD** before the CV step.

### 4. Create and check the PDF

Start a new agent session in the same `cv-work` folder. Replace `[AUDIT FILE]` below with the exact saved filename:

```text
Use tailor/General_CV.md as the base CV. Tailor it for the job
in output/[AUDIT FILE].

Read and follow tailor/CV_TAILOR-Project-Instructions.md
and tailor/MASTER_PROMPT_CV_Tailoring_From_Fit_Audit.md.
For this local task, use the files in tailor/ as Project Sources.
Read tailor/General_CV.md, tailor/Master_Skills.md,
and the full audit. Stop if a required file cannot be read.
Keep the correct personal details and work history from General_CV.md.
Use Master_Skills.md to add relevant, supported facts.
Use the audit for the job details and suggested changes.
Save the tailored CV as a new file. Do not change General_CV.md.
Use the tailoring master prompt's PDF output rule,
even if the audit asks for Markdown.

Use my configured name and language line.
Do not invent facts or change my source files.
Ask no more than three questions at a time.
Use simple English for questions and the final report.
Write the CV in natural, professional English.

Save the real CV PDF in output/ with the required filename.
Check every claim against my files and confirmed answers.
Check the CV against this job's audit.
Extract the saved PDF text and check its reading order.
Render and inspect every page. Read back the PDF metadata.
Fix errors and repeat the affected checks.

Give me the final file path and a short check report.
Include the actual Author and Creator values.
If a tool is missing, explain what is needed.
Never say a check passed unless you ran it.
```

Open the PDF and follow the checks in step 6 of the chat guide. Keep the audit and PDF together for that job.
