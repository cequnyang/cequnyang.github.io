# cequnyang.github.io

Resume site built from a single data source.

## Structure

- `index.html`: main resume page
- `resume/`: regular PDF wrapper page
- `ats/`: ATS HTML page and ATS PDF wrapper page
- `assets/`: shared static assets and generated PDFs
- `data/resume.json`: single resume content and build configuration source
- `tools/build_resume.py`: generator for HTML and PDF outputs

## Build

```powershell
python tools/build_resume.py
```

PDF export automatically looks for a Chromium-family browser on Windows, macOS,
and Linux. If discovery fails on a machine, set `build.pdf_export.browser_path`
in `data/resume.json` to the browser executable path.
