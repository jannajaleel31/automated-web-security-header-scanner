# Automated Web Security Header Scanner

## Project description
This project is a beginner-friendly Python tool that checks a single authorized website for HTTPS usage and the presence of six common HTTP security headers. It displays findings and can save a JSON report.

## Technologies used
- Python 3.9 or later
- Jupyter Notebook (`.ipynb`)
- Requests library
- JSON (Python standard library)

## Files
- `JannaJaleel_AutomatedWebScanner.ipynb` — complete notebook code and explanation
- `requirements.txt` — Python dependency list
- `JannaJaleel_ProjectReport.docx` — project documentation

## Setup on Windows
1. Install Python from https://www.python.org/downloads/
2. Install Jupyter Notebook, if not already installed:
   ```powershell
   py -m pip install notebook
   ```
3. Open Command Prompt or PowerShell in this folder.
4. Install dependencies:
   ```powershell
   py -m pip install -r requirements.txt
   ```
5. Launch Jupyter Notebook:
   ```powershell
   py -m notebook
   ```
6. Open `JannaJaleel_AutomatedWebScanner.ipynb` in the browser and run cells from top to bottom.
7. Set `TARGET_URL` to a website you own or are explicitly authorized to test.
8. Review results and keep the generated `report.json` as supporting evidence if requested.

## Safety and scope
Only scan websites you own or have explicit permission to assess. The notebook sends a single HTTP GET request per run. It does not exploit vulnerabilities, brute-force, crawl, or modify the target. A missing header is not proof of a vulnerability, and header presence does not guarantee a website is secure.

## Dataset
No dataset is required. The project analyzes HTTP response headers returned by the authorized website during execution.

## References
- MDN HTTP headers: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers
- OWASP Secure Headers Project: https://owasp.org/www-project-secure-headers/
- Requests documentation: https://requests.readthedocs.io/
