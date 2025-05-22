![Header](https://github.com/k4itrun/.github/assets/103044629/92715974-a12e-4d2b-a8e9-bddcf227ba9f)

<!-- prettier-ignore -->
> [!NOTE] 
> **If you’re reading this, you’re already helping our community grow. Every contribution — big or small — matters. Please take a moment to review these guidelines for a smooth and rewarding experience.**

<!-- prettier-ignore-end -->

<details>
  <summary>📚 <strong>Table of Contents</strong></summary>
  <ol>
    <li><a href="#-getting-started"><strong>Getting Started</strong></a></li>
    <li><a href="#%EF%B8%8F-coding-standards"><strong>Coding Standards</strong></a></li>
    <li><a href="#-pull-request-checklist"><strong>Pull Request Checklist</strong></a></li>
  </ol>
</details>

---

## 🚀 Getting Started

Jumping into a **new project** can seem daunting, but our process is straightforward and welcoming to contributors of all backgrounds and experience levels.

### 1. 🍴 Fork and Clone

First, head over to the original repository on GitHub and hit that **Fork** button. Think of it like making your own copy of grandma’s secret cookie recipe — you get to experiment without messing up the original masterpiece.

![Forking repository on Github](https://github.com/k4itrun/.github/assets/103044629/59aca8e7-bf3f-49fc-8cc1-ceec2f97939a)

Then, clone your fork to your local machine to start cooking in your own kitchen:

```bash
git clone https://github.com/your-username/this-project.git
cd this-project
```

This pulls down all the project goodness right to your computer.

### 2. 🔗 Add Upstream Remote

Keep your fork up to date with the main project:

```bash
git remote add upstream https://github.com/billoneta/this-project.git
git remote show upstream
```

To sync later:

```bash
git pull upstream main
```

### 3. 🌿 Create a Feature or Fix Branch

<!-- prettier-ignore -->
> [!WARNING]
> **Never work directly on `main`!** Make a new branch for each contribution

<!-- prettier-ignore-end -->

Before you dive in, create a fresh branch. This is like getting a new notebook page so you don’t scribble all over the main story. Name it something clear and descriptive, like `feature/amazing-widget` or `bugfix/fix-login-issue`. This keeps things neat and tidy for you and everyone else:

```bash
git checkout -b feature/your-feature-name
```

Now you’re ready to start your changes without the fear of breaking the main storyline.

### 4. 🔥 Make Your Changes

Time to bring your ideas to life! Whether you're fixing bugs, adding new features, or improving existing ones — go ahead and implement your contribution. Keep things clean, readable, and in line with the project goals.

Quick tip: To avoid merge conflicts later, make sure to pull the latest changes from the original repository **before** starting your work:

```bash
git pull upstream main
```

> [!CAUTION]
> Keep the existing project structure intact and follow the **[Coding Standards](#%EF%B8%8F-coding-standards)** closely.

<!-- prettier-ignore -->
> [!IMPORTANT] 
> **Before submitting your work:**
>
> - **Check the project as many times as necessary and make sure that everything is working.**
> - **Documentation is updated for new features or major changes.**

<!-- prettier-ignore-end -->

### 5. 🚀 Push and Commit

Once your changes are ready and tested, push them to your forked repository:

```bash
git push origin feature/your-feature-name
```

> [!NOTE]
> Replace `feature/your-feature-name` with the name of your branch created earlier in **[step 3](#3--create-a-feature-or-fix-branch)**

### 6. 🧩 Open a Pull Request

Once your code is ready, **go to your forked repository on GitHub and click the "Compare & pull request" button** to open a Pull Request (PR) from your feature branch to the main repository.

Your Pull Request should be clear, descriptive, and follow the required structure. This helps maintainers review your work efficiently and increases the chances of your contribution being accepted.

For full details on what your PR should include, (see [Pull Request Checklist](#-pull-request-checklist)).

> [!CAUTION]
> Keep the existing project structure intact and follow the **[Coding Standards](#%EF%B8%8F-coding-standards)** closely.

<!-- prettier-ignore -->
> [!IMPORTANT] 
> **Before submitting your work:**
>
> - **Check the project as many times as necessary and make sure that everything is working.**
> - **Documentation is updated for new features or major changes.**

<!-- prettier-ignore-end -->

---

## ♻️ Coding Standards

Writing good code isn’t just about making it run — it’s about making it understandable, maintainable, and consistent. These standards help keep the project clean, readable, and easy to work with (even months later when you’ve forgotten what “final_final_finalFix2.js” was supposed to do).

### 1. ✍️ Use Clear, Meaningful Commit Messages

We adhere to the **[Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)** specification alongside **[Gitmoji](https://gitmoji.dev/)** guidelines to include **meaningful emojis** in every commit. This **standardized approach** keeps our commit history **clean, consistent,** and ready for **automation tasks** like generating **changelogs** and managing **versioning**.

> [!NOTE]
> Your commit messages should clearly describe what your changes do and why.
>
> **Examples:**
>
> ```bash
> ✨ feat: add search feature to user dashboard
> 🐛 fix: resolve crash on login with empty password
> 📝 docs: update README with new installation steps
> ```

<!-- prettier-ignore -->
> [!CAUTION] 
> **Avoid vague messages** like `update file` or `fix stuff`.

<!-- prettier-ignore-end -->

This helps reviewers (and your future self) understand the purpose behind each change without having to dig through the code.

### 2. 🧹 Maintain Code Consistency

- **Indentation, naming, and organization** should match the existing code.
- **Respect the project's chosen style**, even if it's not your preference.
- If unsure, **mimic the patterns** you see in similar files.

### 3. 👓 Focus on Readability

Code should be **easy to read and understand** without needing a decoder ring. Avoid **deeply nested logic**, **overly clever tricks**, or **cryptic variable names**.

If a new developer (or your **sleep-deprived teammate**) can’t understand your code within **30 seconds**, it needs **simplification**.

### 4. 🧭 Follow the existing project style

When unsure how to structure something, check how similar features are implemented elsewhere in the codebase. Consistency is more important than personal style.

> [!NOTE]
> If you think there’s a better way to do something, propose it in a pull request or discussion — but don’t introduce a new pattern just for fun.

### 4. 📝 Add Documentation Where Needed

If your code contains **non-obvious logic or important decisions**, add comments explaining "**why**" (not just "**what**").

**Update documentation files** (like README) if your changes affect usage or public APIs.

---

## ✅ Pull Request Checklist

Before submitting your pull request, please ensure you:

- [ ] **Describe your changes clearly** in the PR description.
- [ ] **Reference related issues** if applicable (e.g., "**Closes #123**").
- [ ] **Have tested your changes** and ensured existing tests pass.
- [ ] **Added new tests** for new features or bug fixes (if appropriate).
- [ ] **Updated documentation** as needed.
- [ ] **Kept the branch up-to-date** with the latest main branch (`git pull upstream main`).

### 📝 Example Pull Request Structure

#### ✨ Summary

A brief explanation of what this PR does and why.

#### 🧪 How to Test

Steps for maintainers or reviewers to test your changes.

#### 🔗 Related Issues

<!-- prettier-ignore -->
> [!NOTE]
> **Example:**  
> Closes [#42](https://www.youtube.com/shorts/OdEKu4WXs5c)

<!-- prettier-ignore-end -->

#### 💡 Additional Notes

Anything else reviewers should know.

---

## 📜 License

By contributing, you agree that your contributions will be licensed under the same license as the project (see the [LICENSE](LICENSE.md) file for details).

---

### ❤ Thank you for helping us improve this project!

Your time, ideas, and effort are valued here.  
If you have questions, open a discussion or reach out to the maintainers.
