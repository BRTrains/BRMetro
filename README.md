# BRMetro

A BRBuild project containing the tram and metro vehicles imported from the former BRMetro prototype.

## Build

```bash
uv venv --python 3.14 .venv
uv pip install --python .venv/bin/python pillow pyyaml nml
BRBUILD_DIR=/path/to/BRBuild .venv/bin/python build.py --log
```

`BRBuild.yaml` enables the BRBuild documentation manifest. A successful build writes `docs/generated/manifest.json` for BRdocs consumers.

## Layout

- `BRBuild.yaml` — BRBuild project manifest
- `build.py` — project-local BRBuild launcher
- `src/grf/GRF.yaml` — GRF metadata and parameters
- `src/vehicles/` — imported BRMetro vehicle candidates
- `docs/generated/` — BRBuild-generated BRdocs manifest

BRBuild and BRTrains3 are the format and track-type references. The legacy source is preserved at `/home/jon/BRmetro_old`.

