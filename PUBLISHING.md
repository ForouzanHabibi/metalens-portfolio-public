# Publish this clean folder using VS Code

**Important:** Use a **new empty GitHub repository** (for example,
`metalens-portfolio-public`). Do **not** copy the `.git` folder from your old
repository, do not `git push --force` to the old repository, and do not upload
any file from `research_scripts/`.

1. Extract the ZIP and open **the extracted `metalens-portfolio-public` folder**
   using **File → Open Folder** in VS Code.
2. Open **Terminal → New Terminal** and run the Quick start commands in README.
3. Sign into GitHub in your browser and create a **new empty repository** named
   `metalens-portfolio-public`. Do not add a README or license on GitHub.
4. From the VS Code terminal **inside this new folder**, run:

```powershell
git init
git branch -M main
git add .
git status
git commit -m "Publish independent synthetic metalens demo"
git remote add origin https://github.com/ForouzanHabibi/metalens-portfolio-public.git
git push -u origin main
```

5. In GitHub, verify the README and figures display and check that `research_scripts`
   **does not exist**. Keep the **old repository Private** until you decide how to
   handle its history.

**If `git commit` asks for your identity**, configure it locally:

```powershell
git config user.name "Forouzan Habibighahfarokhi"
git config user.email "your-email-address"
```

Then rerun the `git commit` and `git push` commands. You may instead use
**Source Control → Publish Branch** in VS Code after creating the new repository,
but verify the destination before confirming.

A new repository starts with **fresh history**; deleting files in an older
repository does not erase their old commits. Publishing a new clean repository
cannot revoke any copies previously downloaded by others.

This example intentionally provides **no open-source license**: public visibility
lets people view the portfolio but does not automatically grant them the legal
right to reuse the code. If you want others to reuse it, choose a license later.
