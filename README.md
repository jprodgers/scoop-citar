# scoop-citar

A [Scoop](https://scoop.sh) bucket for [CITAR](https://github.com/jprodgers/CITAR) — a
Civilization V-style 4X game for benchmarking language models.

```powershell
scoop bucket add citar https://github.com/jprodgers/scoop-citar
scoop install citar
citar setup
```

`citar setup` looks for LM Studio, Ollama and other OpenAI-compatible servers already running on
your machine, and tells you what to install if it finds none. Then `citar` on its own starts
playing — it opens your browser.

This installs the portable build, so nothing is written outside Scoop's own directory. Your games
and settings live in `%LOCALAPPDATA%\CITAR` and are **not** removed when you uninstall CITAR.

Prefer a normal installer? There is one on the
[releases page](https://github.com/jprodgers/CITAR/releases/latest).

## This repository is generated

`bucket/citar.json` is copied from
[`packaging/scoop/citar.json`](https://github.com/jprodgers/CITAR/tree/main/packaging/scoop) in the
CITAR repository, with the version and hash filled in by `scripts/release_checksums.py` at each
release. Edit it there, not here.

Problems with the manifest belong in
[CITAR's issue tracker](https://github.com/jprodgers/CITAR/issues).

## Licence

MPL-2.0, the same as CITAR. See [LICENSE](LICENSE).
