# Quickstart

## Install
1. Install Python 3.11+
2. `pip install -r requirements.txt`
3. Run: `python main.py`

## Export
- Brush Builder  pick PNG tip  exports `.gbr` + `.meta.json`
- Palette Wizard → pick image → exports `.gpl` + `.meta.json`

## Pack & Validate
- Tools  **Pack Builder** (GUI)  
- Or CLI:
python tools\pack_builder.py --types all
python tools\validate_pack.py packs<printed-zip>


## Maintenance
- Tools  **Maintenance Tools**  Backfill sidecars / Make previews  
- Tools  **Update Checker**  open latest release page
