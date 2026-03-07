Use the project's bundled virtual environment (`.venv`) for every Python operation (commands, scripts, tools, linting, and type checking).

Use Plotly for notebook/data visualizations, and make figures presentation-ready by default.

Prefer paragraph-style notebook markdown over bullet-point lists unless a list is clearly necessary.

After any relevant code change, run the affected Jupyter code cell(s) and inspect the output. If the output is a graph or other visual plot, export it to a PNG and inspect the generated image.

After every Python-related change (including `.py` and `.ipynb` files), run:

- `task lint`
- `task typecheck`
