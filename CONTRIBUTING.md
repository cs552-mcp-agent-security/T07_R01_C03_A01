# Contributing

Thanks for considering a contribution. Two small rules of thumb:

1. **One PR, one concern.** If you're tuning the optimizer and also fixing a typo
   in `README.md`, please open two PRs.
2. **Keep `main.py` minimal.** If a change needs more than ~15 lines of glue,
   move the logic into a helper inside `utils.py` or a new module under
   `models/`.

## Local development

```bash
pip install -r requirements.txt
pre-commit install
pytest tests/ -q
```

## Reporting issues

Please use the bug report template in `.github/ISSUE_TEMPLATE/`. Include the
PyTorch version and the exact command line that reproduces the problem.
