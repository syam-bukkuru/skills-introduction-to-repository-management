# Introduction to Repository Management - Notes

## Repository

GitHub Skills: Introduction to Repository Management

---

# Step 1: Protect Repository Content

## Branch Ruleset

Purpose:
Protect the main branch from accidental modifications.

### Steps Performed

1. Opened **Settings**.

2. Navigated to:

   ```
   Rules → Rulesets
   ```

3. Clicked:

   ```
   New Ruleset → New Branch Ruleset
   ```

4. Configured:

   * Ruleset Name: `Protect main`
   * Enforcement Status: `Active`

5. Added Targets:

   * Include default branch
   * Include by pattern → `main`

6. Enabled Rules:

   * Restrict deletions
   * Require a pull request before merging
   * Required approvals = 0
   * Require review from Code Owners
   * Block force pushes

7. Saved the ruleset.

### Learning

Rulesets help prevent accidental changes to critical branches.

---

## Create .gitignore

### Steps Performed

1. Opened repository Code tab.

2. Created file:

   ```
   .gitignore
   ```

3. Added rules for:

   * Python cache files
   * Virtual environments
   * IDE settings
   * Operating system files

4. Attempted to commit directly to main.

5. GitHub blocked direct commits due to branch protection.

6. Created branch:

   ```
   prepare-to-collaborate
   ```

7. Opened Pull Request:

   ```
   Prepare to collaborate
   ```

### Learning

.gitignore prevents unnecessary files and secrets from being tracked.

---

# Step 2: Prepare for Collaboration

## CONTRIBUTING.md

### Steps Performed

1. Switched to:

   ```
   prepare-to-collaborate
   ```

2. Created:

   ```
   CONTRIBUTING.md
   ```

3. Added:

   * Development setup
   * Contribution process
   * Branch naming guidelines
   * Code style guidelines
   * Help and support information

4. Committed changes.

### Learning

CONTRIBUTING.md provides onboarding instructions for contributors.

---

## CODEOWNERS

### Steps Performed

1. Created:

   ```
   CODEOWNERS
   ```

2. Assigned ownership of:

   * Backend files
   * Authentication files
   * Static frontend files

3. Committed changes.

### Learning

CODEOWNERS automatically requests reviews from responsible contributors.

---

# Step 3: Foster Healthy Growth

## Code of Conduct

### Steps Performed

1. Created:

   ```
   CODE_OF_CONDUCT.md
   ```

2. Added:

   * Community standards
   * Acceptable behavior
   * Unacceptable behavior
   * Enforcement policy

3. Committed changes.

### Learning

A Code of Conduct promotes a respectful and inclusive community.

---

## Issue Templates

### Steps Performed

1. Opened:

   ```
   Settings → Features → Issues
   ```

2. Clicked:

   ```
   Set up templates
   ```

3. Added:

   * Bug Report template
   * Feature Request template

4. Simplified template fields.

5. Committed changes to:

   ```
   add-issue-templates
   ```

### Learning

Issue templates standardize bug reports and feature requests.

---

# Step 4: Security Preparation

## Dependabot

### Steps Performed

1. Opened:

   ```
   Settings → Advanced Security
   ```

2. Enabled:

   * Dependabot Alerts
   * Dependabot Security Updates
   * Grouped Security Updates

3. Enabled:

   ```
   Dependabot Version Updates
   ```

4. Generated:

   ```
   .github/dependabot.yml
   ```

5. Selected:

   ```
   package-ecosystem: pip
   ```

6. Committed changes to:

   ```
   prepare-to-collaborate
   ```

### Learning

Dependabot automatically detects vulnerable dependencies and creates update pull requests.

---

## CodeQL / Code Scanning

### Steps Performed

1. Opened:

   ```
   Settings → Advanced Security
   ```

2. Located:

   ```
   Code Scanning
   ```

3. Selected:

   ```
   Set Up → Default
   ```

4. Enabled:

   ```
   CodeQL
   ```

5. Verified:

   ```
   Copilot Autofix = ON
   ```

### Learning

CodeQL scans source code for:

* Security vulnerabilities
* Dangerous coding patterns
* Potential bugs

---

## Security Policy

### Steps Performed

1. Opened:

   ```
   Security → Security Policy
   ```

2. Clicked:

   ```
   Start Setup
   ```

3. Created:

   ```
   SECURITY.md
   ```

4. Added:

   * Vulnerability reporting process
   * Response timeline
   * Responsible disclosure instructions

5. Committed changes.

### Learning

SECURITY.md gives researchers a safe way to report vulnerabilities.

---

## Private Vulnerability Reporting

### Steps Performed

1. Opened:

   ```
   Settings → Advanced Security
   ```

2. Enabled:

   ```
   Private Vulnerability Reporting
   ```

### Learning

Allows vulnerabilities to be reported privately instead of publicly.

---

# Step 5: Release

## Merge Pull Requests

### Steps Performed

1. Opened:

   ```
   Pull Requests
   ```

2. Merged:

   ```
   Prepare to collaborate
   ```

3. Merged:

   ```
   add-issue-templates
   ```

4. Waited for GitHub Actions validation.

### Learning

Pull Requests provide:

* Code review
* Collaboration
* Audit history
* Safe deployment workflow

---

# Key GitHub Features Learned

* Branch Rulesets
* Pull Requests
* Branch Protection
* .gitignore
* CONTRIBUTING.md
* CODEOWNERS
* CODE_OF_CONDUCT.md
* Issue Templates
* Dependabot
* CodeQL
* Security Policies
* Private Vulnerability Reporting
* GitHub Actions

---

# Final Takeaway

Repository management is not only about writing code. It is about protecting code, enabling collaboration, maintaining security, establishing contribution processes, and creating a healthy open-source community.
