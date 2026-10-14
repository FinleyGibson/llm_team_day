# LLM Team Day

## Run the notebooks

The project uses Python 3.12 and [uv](https://docs.astral.sh/uv/). From the
repository root, create and sync the project environment with the locked
dependencies:

```bash
uv sync
```

Start JupyterLab with that environment:

```bash
uv run jupyter lab notebooks
```

Open a notebook from the `notebooks` directory and use its Python 3 kernel.
In VS Code, select the interpreter at `.venv/bin/python` as the notebook
kernel.

Some notebooks download tokenizers or models from Hugging Face the first time
their relevant cells run, so those cells need network access. In
`04_practical_prompting.ipynb`, setting `HUGGINGFACE_API_KEY` is optional; the
notebook can use a local model without it.
