# Veyra Development Hub

A documentation-only workspace for coordinating Veyra development across ChatGPT, the regular Claude app, and the regular Gemini app.

> **Safety boundary:** This repository is for project documentation and review notes. Do not commit source code unless you intentionally choose to, and never commit `.env`, API keys, access tokens, passwords, private logs containing secrets, or personal data. This starter pack does not modify your existing Veyra project or configure API billing.

## Start here

1. Read `Veyra_Development_Handoff(1).md` first. It is copied from the handoff supplied for this setup and kept as the baseline.
2. Read `02_Current_State.md` for the current investigation and constraints.
3. Use `03_Task_Board.md` to select one task at a time.
4. Before changing code, record the proposed change and expected test in `04_Decisions_and_Rules.md` or a review note.
5. After an authorized code change, run the relevant test and update `02_Current_State.md`.

## Suggested GitHub setup

Create a **private** repository named `Veyra-Development-Hub` on GitHub. For the simplest setup, create it empty (do not add a README or license because this folder already contains them), then from PowerShell in this extracted folder run:

```powershell
git init
git add .
git commit -m "Initialize Veyra development hub"
git branch -M main
git remote add origin https://github.com/YOUR-GITHUB-USERNAME/Veyra-Development-Hub.git
git push -u origin main
```

Replace `YOUR-GITHUB-USERNAME` with your GitHub username. GitHub may prompt you to authenticate. Never paste an access token into a chat or save it in this repository.

If Git is not installed, you can instead create the private repository on GitHub and upload these documentation files using GitHub's web interface. Keep this hub separate from the actual `veyra` source-code repository unless you deliberately decide otherwise.

## Collaboration routine

- Give each assistant the same `01_Project_Bible.md`, `02_Current_State.md`, `04_Decisions_and_Rules.md`, and the specific source file(s) relevant to the task.
- Ask each assistant to review independently and return findings with severity, evidence, and suggested tests.
- Save responses separately under `05_AI_Reviews/` so reviewers do not bias each other prematurely.
- Compare results in `06_Handoff_and_Prompts/REVIEW_COMPARISON_TEMPLATE.md`.
- Do not treat an AI suggestion as an accepted change until you decide to implement it.

## Important limitation

A GitHub repository is a shared document store, not an automatic bridge between the regular ChatGPT, Claude, and Gemini apps. Unless a supported connector or project feature is configured separately, you must provide the relevant files or links in each app. This setup intentionally uses no integrations or API calls.
