# static-analysis-emirhan-rauf
Static analysis report for mkdocs-with-confluence
# Static Code Analysis Report – mkdocs-with-confluence

**Prepared by:
*Emirhan CAGLAR – SD2 
*Rauf Egemen Imamoglu - SD2
**Date:** May 26, 2025



##  Project Overview

This repository includes a static code analysis report for the [mkdocs-with-confluence](https://github.com/pawelsikora/mkdocs-with-confluence) project, a Python plugin that syncs MkDocs-generated documentation with Atlassian Confluence.

The analysis focuses on identifying code quality issues, style violations, and potential security risks using three popular static analysis tools.

---

## Tools Used

- [`pylint`](https://pylint.pycqa.org/) – for code quality and structure checking  
- [`flake8`](https://flake8.pycqa.org/) – for PEP8 style guide enforcement  
- [`bandit`](https://bandit.readthedocs.io/) – for identifying security vulnerabilities


##  Files

| File | Description |

| `Static_Code_Analysis_Report.docx` | Full analysis report with examples and recommendations |
| `flake8_output.txt` | Output from flake8 tool |
| `pylint_output.txt` | Output from pylint tool |
| `bandit_output.txt` | Output from bandit tool |


## Summary of Findings

- **pylint:** Missing docstrings, long lines, unused variables, complex functions  
- **flake8:** Mostly E501 (line too long), and one E261 (missing space before inline comment)  
- **bandit:** One high-risk issue — use of SHA1 hash algorithm

---

##  Recommendations

- Fix line length issues and spacing problems  
- Add missing docstrings  
- Use `with` statement for file handling  
- Replace insecure hashing algorithms (e.g., use SHA-256 instead of SHA1)

---

##  Contribution Suggestion

If these issues are fixed, a pull request can be submitted to the original open-source repository. This would demonstrate proper coding standards and community involvement.


##  Original Project

🔗 https://github.com/pawelsikora/mkdocs-with-confluence

