# Pack Profiles

Pack Profiles let you batch-build packs from a JSON file — either from the GUI or CLI.

## JSON format

`profiles/pack_profiles.json`:

```json
{
  "profiles": [
    {
      "name": "Local – All",
      "types": "all",
      "src_brushes": "exports/brushes",
      "src_palettes": "exports/palettes",
      "out": "packs",
      "set": "Local-Samples"
    }
  ]
}
```
