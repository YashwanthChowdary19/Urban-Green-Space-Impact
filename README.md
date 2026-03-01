# Team Instructions to Work on Urban-Green-Space-Impact Repository (GitHub)

Follow the below steps carefully to contribute to the project.

---

## Step 1: Accept the Invitation

- Open your email and accept the invitation from GitHub.
- Or go to GitHub → Your repositories → Open **Urban-Green-Space-Impact**

Repository link:  
https://github.com/YashwanthChowdary19/Urban-Green-Space-Impact.git

---

## Step 2: Clone the Repository

Open Git Bash or Command Prompt and run:

```bash
git clone https://github.com/YashwanthChowdary19/Urban-Green-Space-Impact.git
cd Urban-Green-Space-Impact
```

---

## Step 3: Create Your Own Branch (IMPORTANT)

Do NOT work on main branch.

Create a branch using your name:

```bash
git checkout -b yourname_branch
```

Example:

```bash
git checkout -b ravi_branch
```

---

## Step 4: Do Your Assigned Work

Add or modify files such as:

- Python files (.py)
- Jupyter notebooks (.ipynb)
- Dataset files
- Documentation files

---

## Step 5: Check Changes

```bash
git status
```

---

## Step 6: Add Files

```bash
git add .
```

---

## Step 7: Commit Changes

```bash
git commit -m "Your work description"
```

Examples:

```bash
git commit -m "Added preprocessing code"
git commit -m "Added feature engineering"
git commit -m "Added model training"
```

---

## Step 8: Push Your Branch

```bash
git push origin yourname_branch
```

Example:

```bash
git push origin ravi_branch
```

---

## Step 9: Create Pull Request

- Go to GitHub repository
- Click **Compare & pull request**
- Click **Create Pull Request**
- Add description
- Submit Pull Request

---

## Step 10: Pull Latest Changes Before Starting New Work

```bash
git checkout main
git pull origin main
git checkout yourname_branch
git merge main
```

---

## Important Rules

- Always create your own branch
- Never push directly to main branch
- Always commit your own work
- Always create Pull Request
- Always pull latest changes before starting work

---

## Example Full Workflow

```bash
git clone https://github.com/YashwanthChowdary19/Urban-Green-Space-Impact.git
cd Urban-Green-Space-Impact
git checkout -b yourname_branch
# Do your work
git add .
git commit -m "Added my contribution"
git push origin yourname_branch
```
