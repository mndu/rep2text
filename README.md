# Rep2Text — NeurIPS 2026 project page

A lightweight static project website for **Rep2Text: Decoding Full Text from a Single LLM Token Representation**, using the same visual style as the SAEExplainer page. The top navigation and conference badge are omitted, following the author's preferred layout.

- Website: https://mndu.github.io/rep2text/
- Website repository: https://github.com/mndu/rep2text
- Paper preprint: https://arxiv.org/abs/2511.06571

## Local preview

From this directory, run `python3 -m http.server 8000`, then open http://localhost:8000. There is no build step or package dependency.

## Maintenance

- `index.html`: paper content, authors, metrics, links, and BibTeX.
- `style.css`: shared visual style from the SAEExplainer site.
- `paper.css`: layout adjustments for this paper's figures and tables.
- `script.js`: citation copying with a manual-copy fallback.
- `assets/`: figures cropped from the supplied PDF, plus the site favicon.
- `rep2text.pdf`: the supplied paper, unchanged.

GitHub Pages publishes the `main` branch from `/ (root)`. Commit and push updates to redeploy.

## Source and editorial notes

The supplied `rep2text.pdf` is the source of the abstract, author order, method descriptions, figures, and experimental values. NeurIPS 2026 acceptance is stated by the author and on the supplied PDF.

- The PDF labels both Cisco Research and Wake Forest University with affiliation 3, while Fan Yang has superscript 4. The website uses 4 for Wake Forest University to match Fan Yang's superscript and institutional email; the original PDF is preserved.
- The main table reproduces the mean ROUGE and BERTScore values of all eight configurations in Table 1. Standard deviations and additional metrics are available in the paper.
- The analysis figures are Figures 4 and 5. The original/reconstructed text example comes from Table 3 and is explicitly identified as a selected example.
- The clinical results use the Mistral-7B-v0.1 section of Table 2. The summary follows the tabulated values and retains the paper's caveat about imperfect recovery of critical details.
- The citation omits unconfirmed volume and page details. Update these when official proceedings metadata is available.
- No official research-code URL was found in the supplied PDF or checked public sources, so the page does not present the website repository as research code.

Visual style adapted from the original SAEExplainer website in the parent directory, which drew on the centered layouts of Ctrl-X and DisCoScene project pages. No third-party template code was copied.
