# Day 1: Full-Stack Web Development Learnings

## 1. Version Control: Git & GitHub

### What is Git?
**Git** is a free, open-source **Distributed Version Control System (DVCS)** designed to track changes in source code during software development.
- **Tracks History**: Records every modification made over time, allowing you to revert files or projects to previous states.
- **Branching & Merging**: Lets developers work on isolated feature branches without disturbing the main codebase.
- **Works Offline**: Stores the entire repository history locally on your machine—no internet connection is needed for commits or branch switching.

---

### What is GitHub?
**GitHub** is a cloud-based hosting platform built around Git that enables developers to store, manage, share, and collaborate on code repositories.
- **Cloud Backup**: Serves as a centralized remote host for your Git repositories.
- **Collaboration**: Provides team collaboration tools like Pull Requests (PRs), code reviews, issues, and discussions.
- **Ecosystem**: Integrates with continuous integration and continuous delivery (CI/CD) pipelines (GitHub Actions), project boards, and web hosting (GitHub Pages).

---

### Key Differences Between Git and GitHub

| Feature | Git | GitHub |
| :--- | :--- | :--- |
| **Definition** | Version control software / CLI tool | Cloud-based hosting platform for Git repositories |
| **Location** | Runs locally on your machine | Hosted in the cloud |
| **Internet Access** | Works completely offline | Requires internet to access and sync |
| **Primary Purpose** | Tracks code history and versioning | Facilitates backup, code sharing, and team collaboration |
| **Interface** | Command Line Interface (CLI) & desktop GUI clients | Web interface, GitHub Desktop, GitHub CLI (`gh`) |
| **Maintenance** | Open-source community project | Proprietary platform owned by Microsoft |

---

### Essential Git Commands

Here is the standard workflow of basic Git commands:

#### 1. Configuration (`git config`)
Sets your identity for all commits you create.
```bash
# Set your name and email globally
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

# View your current configurations
git config --list
```

#### 2. Cloning a Repository (`git clone`)
Downloads an existing remote repository from GitHub onto your local machine.
```bash
git clone https://github.com/username/repository-name.git
```

#### 3. Staging Changes (`git add`)
Adds modified or newly created files to the staging area to prepare them for a commit.
```bash
# Stage a specific file
git add index.html

# Stage all modified and untracked files in the current folder
git add .
```

#### 4. Committing Changes (`git commit`)
Saves a snapshot of your staged changes to your local Git history with an explanatory message.
```bash
git commit -m "Add Day 1 HTML structure and Git notes"
```

#### 5. Pushing Changes (`git push`)
Uploads your local commits to the remote repository (such as GitHub).
```bash
git push origin main
```

#### 6. Pulling Changes (`git pull`)
Fetches and merges recent changes from the remote repository into your local branch.
```bash
git pull origin main
```

> **Typical Day-to-Day Workflow**:
> `git pull` &rarr; Make edits &rarr; `git add .` &rarr; `git commit -m "..."` &rarr; `git push`

---

## 2. Web Fundamentals: HTML

### What is HTML?
**HTML** stands for **HyperText Markup Language**. It is the standard language used to create and structure content on the World Wide Web.
- **HyperText**: Text containing hyperlinks to other text or web pages.
- **Markup**: Uses tags (`<tag>...</tag>`) to label pieces of content such as headings, paragraphs, images, and tables.
- **The Core Web Triad**: HTML provides the **structure/skeleton**, CSS provides the **styling/appearance**, and JavaScript provides the **behavior/interactivity**.

---

### HTML Document Skeleton

Every standard HTML5 document follows this foundational structure:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Day 1 Learnings</title>
  </head>
  <body>
    <h1>Welcome to Day 1</h1>
    <p>This is visible in the browser window.</p>
  </body>
</html>
```

#### Structural Tags:
- `<!DOCTYPE html>`: Informs the browser that this is an HTML5 document.
- `<html>`: The root container element that encloses all other HTML elements.
- `<head>`: Holds document metadata, page title, character set definitions, and links to stylesheets/scripts (not directly visible in the viewport).
- `<title>`: Defines the title displayed on the browser tab and search engine results.
- `<body>`: Contains all visible page content (headings, paragraphs, images, buttons, lists, etc.).

---

### Commonly Used HTML Tags

#### 1. Headings & Paragraphs
- `<h1>` to `<h6>`: Heading tags, where `<h1>` represents the highest importance/largest size and `<h6>` the smallest.
- `<p>`: Paragraph tag used to group sentences and blocks of text.

```html
<h1>Main Topic Heading</h1>
<h2>Section Subheading</h2>
<p>This is a paragraph of text explaining the core concepts.</p>
```

#### 2. Text Formatting Tags
Tags used to apply styling or semantic emphasis to text:
- `<b>`: Formats text in **bold** (purely visual presentation).
- `<strong>`: Formats text in **bold** with semantic importance (read with emphasis by screen readers).
- `<i>`: Formats text in *italics* (stylistic).
- `<em>`: Formats text in *italics* with semantic emphasis.
- `<u>`: <u>Underlines</u> text.
- `<mark>`: <mark>Highlights</mark> text with a background color.
- `<small>`: Renders text in a smaller font (useful for disclaimers or copyright notices).
- `<del>`: Renders text with a strikethrough (represents deleted content).
- `<sub>`: Subscript text (e.g., H<sub>2</sub>O).
- `<sup>`: Superscript text (e.g., E = mc<sup>2</sup>).

```html
<p>Remember to <strong>commit frequently</strong> and write <em>clear</em> messages.</p>
<p>Water formula: H<sub>2</sub>O | Math exponent: 10<sup>2</sup> = 100</p>
```

#### 3. Lists
HTML offers two primary list types to organize content:

- **Unordered List (`<ul>`)**: Bulleted list.
  ```html
  <ul>
    <li>Git</li>
    <li>GitHub</li>
    <li>HTML</li>
  </ul>
  ```

- **Ordered List (`<ol>`)**: Numbered list.
  ```html
  <ol>
    <li>Install Git</li>
    <li>Configure username and email</li>
    <li>Clone the repository</li>
  </ol>
  ```

- **List Item (`<li>`)**: Used inside both `<ul>` and `<ol>` to define each individual list item.

---

### Day 1 Summary Checklist
- [x] Understood Git (VCS) vs GitHub (Cloud Host)
- [x] Configured Git credentials (`git config`)
- [x] Used key Git commands (`git clone`, `git add`, `git commit`, `git push`, `git pull`)
- [x] Created basic HTML structure (`<!DOCTYPE html>`, `<html>`, `<head>`, `<body>`)
- [x] Structured text with headings, paragraphs, text formatting, and lists (`<ul>`, `<ol>`, `<li>`)
