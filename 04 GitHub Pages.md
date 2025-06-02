
# 🌐 Lab: Publish Your GitHub Profile README as a GitHub Pages Site

## 🕐 Duration: 30 minutes  
🎯 **Objective**: Learn how to deploy your GitHub profile README as a live GitHub Pages site, making your profile summary accessible on the web.

---

## 🧠 Learning Outcomes

By the end of this lab, students will be able to:

- Understand the difference between a GitHub Profile README and GitHub Pages
- Enable GitHub Pages for a profile repository
- Publish their profile README as a web page
- Access and share the public URL

---

## 🗂️ Lab Overview

| Duration | Type              | Tools              | Team Size      |
|----------|-------------------|--------------------|----------------|
| 0.5 hours  | Guided + Self-paced | GitHub Pages    | Individual  |

---

## 📘 What is a GitHub Profile README?

- A **profile README** appears at the top of your GitHub profile page.
- It's stored in a **special repository** named exactly as your GitHub username (e.g., `yourusername/yourusername`).
- GitHub Pages lets you also publish the **contents of this repo** as a **web page** at `https://yourusername.github.io/yourusername/`.

---

## 🛠️ Step 1: Ensure You Have a Profile README (10 mins)

1. Go to [https://github.com/yourusername/yourusername](https://github.com/yourusername/yourusername)
2. Make sure the repository contains a `README.md` with your profile content.
3. If not, follow the lab “Create Your GitHub Profile README” first.

---

## 🌍 Step 2: Enable GitHub Pages (10 mins)

1. In your `yourusername/yourusername` repository, go to **Settings**.
2. In the left menu, click **Pages**.
3. Under **Source**, choose:
   - **Branch**: `main`
   - **Folder**: `/ (root)`
4. Click **Save**.

📌 GitHub will now generate a site at:
```
https://yourusername.github.io/yourusername/
```
⚠️ This may take 1–5 minutes to go live.

---

## 🎨 Optional: Style the Page (Optional Bonus)

By default, README content is shown in raw markdown style. For a more styled appearance:

- Add a simple `index.html` file with your content inside HTML tags.
- Or use GitHub Pages with a Jekyll theme.

Example `index.html` snippet:
```html
<!DOCTYPE html>
<html>
<head><title>My GitHub Profile</title></head>
<body>
  <h1>Welcome to my Profile Page</h1>
  <p>This site complements my GitHub profile README!</p>
</body>
</html>
```

You can create this file in the same repo and GitHub Pages will serve it as your homepage.

---

## 🔗 Step 3: Share Your Profile Page (10 mins)

Once live, open your browser and visit:
```
https://yourusername.github.io/yourusername/
```

Share the link with your peers or instructor!

---

## 🧰 Resources

- [GitHub Pages Documentation](https://pages.github.com/)
- [GitHub Profile READMEs](https://docs.github.com/en/github/setting-up-and-managing-your-github-profile/customizing-your-profile/about-your-profile)

🙌 You’ve now made your professional profile globally accessible!
