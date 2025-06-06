
# ⚙️ Lab: Automate with GitHub Actions – CI in 30 Minutes

## 🕐 Duration: 30 minutes  
🎯 **Objective**: Understand the basics of GitHub Actions and create a workflow that automatically runs when changes are pushed to a repository.

---

## 🧠 Learning Outcomes

By the end of this lab, students will be able to:

- Understand what GitHub Actions are and why they're used
- Create a basic GitHub Actions workflow
- Trigger an action on push to the `main` branch
- View workflow results in GitHub’s Actions tab

---

## 💡 Use Case: Auto-check Markdown on Push

**Scenario**:  
You're managing a documentation repo with `README.md` and want to run a markdown linter (or echo a test message) every time someone pushes changes. This helps ensure the markdown is structured correctly and reminds users of quality checks.

---

## 🧰 Requirements

- A GitHub account
- A repository with a `README.md` or markdown content

---

## 🗂️ Step-by-Step Instructions

### ✅ Step 1: Create a Repository or Use Existing (5 mins)

1. Create or open an existing repository on GitHub.
2. Ensure it has at least a `README.md` file.
3. Clone the repo using GitHub Desktop (optional).

---

### 🛠️ Step 2: Add a GitHub Actions Workflow (10 mins)

1. In your repo, create the following path and file:
   ```
   .github/workflows/markdown-check.yml
   ```

2. Add this starter workflow:
   ```yaml
   name: Markdown Check

   on:
     push:
       branches: [ main ]

   jobs:
     echo-test:
       runs-on: ubuntu-latest
       steps:
         - name: Checkout Code
           uses: actions/checkout@v3

         - name: Echo Confirmation
           run: echo "✅ Markdown check complete! README has been updated."
   ```

3. Commit the new workflow file to your repo.

📁 _This file lives inside the `.github/workflows` folder and defines what should happen on push events._

---

### 🚀 Step 3: Trigger the Workflow (5 mins)

1. Make a small change to `README.md` (e.g., add a line or fix a typo).
2. Commit and push the change to the `main` branch.

GitHub Actions will automatically run your workflow.

---

### 📊 Step 4: View Results (5 mins)

1. Go to your repository on GitHub.
2. Click on the **Actions** tab.
3. View the most recent workflow run.
4. Click into the run and check logs for the `✅ Markdown check complete!` message.

---

## 🧰 Bonus Challenge (Optional)

- Replace the `echo` step with a real markdown linter (like `markdownlint`).
- Explore pre-built Actions in the [GitHub Actions Marketplace](https://github.com/marketplace?type=actions).

---

## 📘 Resources

- [GitHub Actions Docs](https://docs.github.com/en/actions)
- [GitHub Actions Cheatsheet](https://github.com/actions/starter-workflows)
- [Explore Actions Marketplace](https://github.com/marketplace?type=actions)

🙌 You’ve just built and triggered your first GitHub Action!
