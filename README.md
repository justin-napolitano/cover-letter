# Expressive Resume & Cover Letter LaTeX Template

This repository contains the Expressive Resume LaTeX template along with supporting files to create beautifully formatted resumes and cover letters with minimal LaTeX knowledge. The templates are designed to be easy to use, allowing you to focus on writing your content rather than wrestling with formatting code.

## Features

- Minimal setup: start writing your resume or cover letter without needing to scroll through hundreds of lines of formatting code.
- Custom LaTeX commands simplify adding common resume elements like headers, objectives, and contact info.
- Compatible with most LaTeX typesetting engines (written in LaTeX2e).
- Includes a paired cover letter template to complement your resume.

## Tech Stack

- Primary language: TeX (LaTeX2e)
- PDF generation via pdfTeX / pdfLaTeX

## Getting Started

### Prerequisites

- A LaTeX distribution installed (e.g., TeX Live, MiKTeX)
- A LaTeX editor or command line tools

### Installation

1. Clone this repository:

```bash
git clone https://github.com/justin-napolitano/cover-letter.git
cd cover-letter
```

2. Navigate to the `expressive-resume` directory where the template files are located.

### Usage

1. Create a new `.tex` file in the `expressive-resume` folder.
2. Use the `ExpressiveResume` document class:

```tex
\documentclass{ExpressiveResume}

\begin{document}

% Your resume content here

\end{document}
```

3. Add your resume header using the `\resumeheader` command with optional parameters:

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

4. Optionally add an objective statement:

```tex
\objective{
    Seeking a software engineering position where I can apply my skills.
}
```

5. Compile with your preferred LaTeX engine (e.g., `pdflatex`).

## Project Structure

```
cover-letter/
├── expressive-resume/       # LaTeX template files and README for expressive resume
│   └── README.md             # Documentation specific to the template
├── References.pdf           # Example or reference PDF
├── texput.log               # LaTeX compilation log file
```

## Future Work / Roadmap

- Add comprehensive example `.tex` files demonstrating cover letter usage.
- Improve documentation with more usage examples and troubleshooting tips.
- Develop automated build scripts for easier PDF generation.
- Expand customization options for different resume styles and layouts.

---

*Note: This repository currently lacks a detailed description and some files like `cover_page.tex` appear incomplete or cause compilation errors. Contributions to improve stability and documentation are welcome.*