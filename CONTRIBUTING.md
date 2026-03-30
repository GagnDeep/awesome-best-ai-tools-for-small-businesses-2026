# Contributing to Best AI Tools for Small Businesses 2026

Thank you for your interest in contributing! This project thrives on community knowledge. Please take a moment to read this guide before submitting.

## Quick Links

- [Code of Conduct](#code-of-conduct)
- [How to Contribute](#how-to-contribute)
- [Tool Addition Criteria](#tool-addition-criteria)
- [Style Guide](#style-guide)
- [Link Verification](#link-verification)
- [Pull Request Checklist](#pull-request-checklist)

---

## Code of Conduct

By participating in this project, you agree to maintain a respectful, constructive environment. We don't tolerate harassment, spam, or promotional marketing disguised as contributions. Keep discussions focused on helping small businesses discover genuinely useful AI tools.

---

## How to Contribute

### Adding a New Tool

1. **Fork the repository** — click the "Fork" button on GitHub.
2. **Clone your fork locally:**
   ```bash
   git clone https://github.com/YOUR_USERNAME/awesome-best-ai-tools-for-small-businesses-2026.git
   cd awesome-best-ai-tools-for-small-businesses-2026
   ```
3. **Create a feature branch:**
   ```bash
   git checkout -b add/TOOL-NAME
   ```
4. **Add your tool** to the appropriate category in `README.md` (alphabetically within the section).
5. **Commit and push:**
   ```bash
   git commit -m "Add TOOL NAME in CATEGORY"
   git push origin add/TOOL-NAME
   ```
6. **Open a Pull Request** against the `main` branch with a clear description.

### Fixing a Broken Link

1. Fork and branch: `fix/broken-link-TOOL-NAME`
2. Update the URL in `README.md`
3. Verify the new URL works (see [Link Verification](#link-verification))
4. Submit a PR with the subject: `Fix: broken link for TOOL NAME`

### Improving Descriptions

Descriptions that are inaccurate, too short (under 80 words), or too long (over 150 words) should be corrected. Please include a brief note explaining what was wrong with the original description.

---

## Tool Addition Criteria

A tool qualifies for this list if ALL of the following are true:

| Criterion | Requirement |
|-----------|-------------|
| **Relevance** | Must solve a specific small business problem (not general-purpose or developer-only) |
| **AI-Powered** | Must have genuine AI/ML features (not just a web interface) |
| **Free Tier** | Must have a free plan, free trial, or affordable entry-level pricing (< $50/mo) |
| **SMB Focus** | Must be usable and marketed to businesses of 1–50 people |
| **Active Status** | Must be actively maintained (no abandoned repos, no deprecated services) |
| **Working URL** | Must have a publicly accessible, non-paywalled website or GitHub repo |

**Tools that do NOT qualify:**
- ❌ General-purpose dev tools (VS Code, GitHub, Docker) without specific SMB use cases
- ❌ Generic automation platforms (n8n, Zapier) unless your PR specifies a concrete SMB use case
- ❌ General calendar/scheduling tools unless specifically for business appointments
- ❌ Enterprise-only tools with no accessible pricing or trial
- ❌ Tools without AI features (we are specifically an *AI* tools list)
- ❌ Duplicate tools already listed in the same or another category

---

## Style Guide

### Formatting

Tool entries must follow this exact structure:

```markdown
### Tool Name

**Website:** [https://example.com](https://example.com)

**Tags:** `category` `subcategory` `feature`

Description text between 80 and 150 words. Start with what the tool does,
then who it's for, then notable features, then pricing info. End with a
sentence on what makes it stand out. No newline between the URL and tags.
```

### URL Format

- Always use the **main website URL** (not a login page, not a pricing page)
- Link text should be just the domain: `[https://example.com](https://example.com)`
- If a tool has a notable GitHub repo in addition to a website, include both

### Tags

Use 3–6 lowercase tags. Format: `category` `subcategory` `feature`

### Descriptions

- **Minimum 80 words** — less than 80 words means the entry lacks sufficient detail
- **Maximum 150 words** — more than 150 words makes the list hard to scan
- Write in present tense: "helps" not "helped", "provides" not "provided"
- No marketing fluff ("revolutionary", "game-changing", "best-in-class")
- Include specific pricing or free tier details when notable

---

## Link Verification

Before submitting a PR, **verify your links work**:

```bash
# Option 1: Check a single URL with curl
curl -sI https://example.com | head -n 1

# Option 2: Check multiple URLs with a loop
for url in "https://tool1.com" "https://tool2.com"; do
  status=$(curl -sI "$url" | head -n 1)
  echo "$url -> $status"
done
```

Look for `HTTP/2 200` or `HTTP/1.1 200 OK`. Avoid URLs that redirect excessively or return 4xx/5xx errors.

---

## Pull Request Checklist

Before submitting your PR, confirm:

- [ ] My tool meets all criteria in [Tool Addition Criteria](#tool-addition-criteria)
- [ ] My entry follows the [Style Guide](#style-guide) exactly
- [ ] All links return HTTP 200
- [ ] The description is between 80–150 words
- [ ] I've placed the tool in the correct category
- [ ] I've placed the tool alphabetically within that category
- [ ] I've added relevant tags (3–6, lowercase)
- [ ] I've added only one tool per PR (makes review easier)
- [ ] I've included a clear PR title: `Add [TOOL NAME] in [CATEGORY]`

---

## Reporting Issues

Found something wrong but don't have time to contribute a fix? Open an issue:

- **Broken link:** Use tag `broken-link`, include tool name and current URL
- **Outdated info:** Use tag `outdated`, describe what's wrong
- **Wrong category:** Use tag `categorization`, explain why
- **New suggestion:** Use tag `suggestion`, fill out the tool criteria table

---

## Recognition

Contributors will be acknowledged in the README's contributor graph. By submitting a contribution, you agree to your name and PR being visible in the project history.

---

*Thank you for helping small businesses discover the best AI tools!*
