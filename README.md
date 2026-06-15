# resume

My personal Resume written in LaTeX. The template is form https://github.com/latex-ninja/hipster-cv

## Requirements Setup

    sudo apt install texlive-latex-recommended texlive-xetex texlive-fonts-extra texlive-lang-cjk latexmk fonts-noto-cjk -y

- In VSCode, install the `LaTeX Workshop` extension.
- The document uses `fontspec` and `xeCJK` (for Chinese characters), which require **XeLaTeX** — build with `latexmk -xelatex` or use the provided `.vscode/settings.json` and `hipster-cv/.latexmkrc`.

## Usage

**Command line:**

```bash
cd hipster-cv
latexmk -xelatex resume_Gstoettner_J_2026.tex
```

The PDF is written to `hipster-cv/resume_Gstoettner_J_2026.pdf`.

To clean build artifacts:

```bash
latexmk -C resume_Gstoettner_J_2026.tex
```

**VS Code:**

Open the workspace, then open `hipster-cv/resume_Gstoettner_J_2026.tex` and press `Ctrl+Alt+B` to build via LaTeX Workshop. The included `.vscode/settings.json` automatically configures LaTeX Workshop to use `xelatex`.

[Resume pdf](https://github.com/JosefGst/resume/blob/main/hipster-cv/resume_Gstoettner_J_2025.pdf)