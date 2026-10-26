# MicroPy: Towards Training Transformers as a Universal Computer

This is the official codebase for **Towards Training Transformers as a Universal Computer** (Findings of EMNLP 2026).

**Ruize Xu · Chenxiao Yang · Yanhong Li · David McAllester**

MicroPy is a small, Turing-complete language for studying learned program execution. A decoder-only Transformer learns atomic evaluation steps through next-token prediction. Together with PENCIL, these steps form program-level chain-of-thought: completed execution history is removed while returned values and effects are retained.

**Materials:** [Project page](https://micropy.org/) · [Paper](https://micropy.org/assets/paper.pdf) · [Slides](https://micropy.org/assets/slides.pdf) · [PENCIL](https://github.com/chr26195/PENCIL)

## Release status

This initial release contains the standalone **MicroPy reference-interpreter notebook**. Training code, data-generation pipelines, datasets, and model checkpoints are not included in this release.

## Installation

Use Python 3 with Jupyter Notebook or JupyterLab:

```bash
python -m pip install notebook
```

The notebook itself uses only the Python standard library.

## Run the notebook

Open [`MicroPy3.ipynb`](MicroPy3.ipynb) and run its cells in order:

```bash
jupyter notebook MicroPy3.ipynb
```

The notebook introduces the interpreter, PENCIL context reduction, and examples of object reads and writes, function calls, branching, bit copying and flipping, binary addition, and multiplication. It runs the reference interpreter; it does not load a trained Transformer.

Saved execution outputs have been cleared to keep the notebook compact. Running the examples prints their execution traces.

## Citation

If you find this work useful, please cite:

```bibtex
@inproceedings{xu2026micropy,
  title     = {Towards Training Transformers as a Universal Computer},
  author    = {Xu, Ruize and Yang, Chenxiao and Li, Yanhong and McAllester, David},
  booktitle = {Findings of the Association for Computational Linguistics: EMNLP 2026},
  year      = {2026},
  url       = {https://micropy.org/}
}
```

## Acknowledgements

This work builds on [PENCIL: Long Thoughts with Short Memory](https://github.com/chr26195/PENCIL), which also inspired the structure of this repository.
