---
slug: github-cover-letter-writing-overview
id: github-cover-letter-writing-overview
title: Cover Letter and Resume Made Easy with LaTeX
repo: justin-napolitano/cover-letter
githubUrl: https://github.com/justin-napolitano/cover-letter
generatedAt: '2025-11-24T17:13:18.341Z'
source: github-auto
summary: >-
  I created the **Cover Letter** project to simplify putting together
  professional resumes and cover letters using LaTeX. If you’ve ever wrestled
  with formatting in Word or Google Docs, you’ll understand the appeal of
  keeping it clean and straightforward.
tags: []
seoPrimaryKeyword: ''
seoSecondaryKeywords: []
seoOptimized: false
topicFamily: null
topicFamilyConfidence: null
kind: writing
entryLayout: writing
showInProjects: false
showInNotes: false
showInWriting: true
showInLogs: false
---

I created the **Cover Letter** project to simplify putting together professional resumes and cover letters using LaTeX. If you’ve ever wrestled with formatting in Word or Google Docs, you’ll understand the appeal of keeping it clean and straightforward. 

## What This Repo Is 

The **Cover Letter** GitHub repo offers a LaTeX template designed specifically for crafting resumes and accompanying cover letters. It’s for anyone who wants their application documents to look sharp without getting bogged down in the intricate details of LaTeX formatting. It allows you to focus on the content rather than wrestling with templates that add complexity. 

## Why It Exists 

I built this project out of frustration. After trying to find a decent LaTeX template online, I noticed most either required extensive tweaking or were overly complicated. My aim was simple: create a straightforward template that minimized setup while delivering professional results. This way, anyone—even those new to LaTeX—could produce solid application materials.

## Key Design Decisions 

1. **Simplicity First**: The project uses minimal setup, letting users dive right into creating their documents.
2. **Custom Commands**: I created LaTeX commands for common elements like headers and objectives. This reduces the boilerplate code you need to worry about.
3. **Compatibility**: Built on LaTeX2e, it works well with standard LaTeX typesetting engines, ensuring broad compatibility.
4. **Paired Templates**: The resume and cover letter templates complement each other, reinforcing a cohesive application package.

## Tech Stack

- **Primary Language**: TeX (specifically LaTeX2e)
- **PDF Generation**: Powered by pdfTeX / pdfLaTeX

## Getting Started

To get going with the template, you just need to have a LaTeX distribution like TeX Live or MiKTeX installed. Here’s how to set it up:

### Installation Steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/justin-napolitano/cover-letter.git
   cd cover-letter
   ```
2. Navigate to the `expressive-resume` directory where all the template files are stored.

### Usage Instructions:

1. Create a new `.tex` file in the `expressive-resume` folder.
2. Use the `ExpressiveResume` document class to get started:
   ```tex
   \documentclass{ExpressiveResume}
   \begin{document}
   % Your resume content here
   \end{document}
   ```
3. Add your header with the `\resumeheader` command:
   ```tex
   \resumeheader[
       firstname=John,
       lastname=Doe,
       email=john.doe@example.com,
       phone=123-456-7890,
       linkedin=johndoe,
       github=johndoe,
       city=San Francisco,
       state=CA
   ]
   ```
4. Optionally, include an objective statement:
   ```tex
   \objective{
       Seeking a software engineering position where I can apply my skills.
   }
   ```
5. Compile it using your preferred LaTeX engine like `pdflatex`.

## Project Structure 

Here's a glance at how the repo is structured:

```
cover-letter/
├── expressive-resume/    # Contains templates and related files
├── README.md             # This file
├── References.pdf        # Purpose unspecified 
├── texput.log            # LaTeX compilation log
```

## Tradeoffs 

Creating a simple template meant I had to make some tradeoffs. While the ease of use is excellent for newcomers, I realized that some advanced customization options were sacrificed in the pursuit of simplicity. If you want an intricate design detail, this might not be the right fit. However, I stand by the idea that most users want to focus on their content—and this template aligns with that philosophy.

## What’s Next?

I have some plans for the future. Here’s what I’m looking into:

- **More Documentation**: I want to add examples that showcase different usages. A practical guide would do wonders.
- **Expanded Features**: Adding sections like certifications or additional customization options would be helpful.
- **Sample Files**: I’d like to provide sample `.tex` files demonstrating cover letter usage, making it even easier to get started.
- **Automation**: I’m considering automation scripts or a Makefile to handle PDF compilation.
- **Better Error Handling**: LaTeX can be finicky, so improved error handling in the documentation would help simplify troubleshooting for users.

If you want to stay updated on this project or see what else I’m working on, you can catch me on social media. I share updates on Mastodon, Bluesky, and Twitter/X.

## Conclusion

The **Cover Letter** project makes the daunting task of creating resumes and cover letters as painless as possible. It’s straightforward, focused on user experience, and avoids unnecessary complexity. If you're tired of fighting with templates, give this one a shot. Let’s make job applications less stressful, one LaTeX document at a time.
