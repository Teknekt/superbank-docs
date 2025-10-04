# Sidecar Schema (v1.0)

Sidecars live next to exported assets as `*.meta.json`. They carry author, license, version and per-asset details SuperBank uses when:

- building packs
- generating release notes
- validating resources

> **Naming**
> Sidecar filename: `<original-filename>.<ext>.meta.json`
> Example: `sb_dry-edge_v1.0.0_512px.gbr.meta.json`

---

## Common fields (all types)

These appear in **every** sidecar:

```json
{
  "schema_version": "1.0",
  "asset_version": "1.0.0",
  "type": "brush|palette",
  "name": "Human Name",
  "set": "Collection/Set name",
  "tags": ["optional", "tags"],
  "author": { "name": "Your Name", "url": "" },
  "license": { "id": "CC0-1.0", "url": "https://creativecommons.org/publicdomain/zero/1.0/" },
  "created_at": "2025-10-03T12:00:00Z"
}
{
  "type": "brush",
  "size": { "width": 512, "height": 512, "px": 512 },
  "spacing": 25,
  "bytes": 1
}
{
  "type": "palette",
  "columns": 8,
  "color_count": 32
}
{
  "schema_version": "1.0",
  "asset_version": "1.2.0",
  "type": "brush",
  "name": "Dry Edge",
  "set": "InkSketch",
  "tags": ["dry", "edge", "ink"],
  "author": { "name": "Teknekt", "url": "" },
  "license": { "id": "CC0-1.0", "url": "https://creativecommons.org/publicdomain/zero/1.0/" },
  "created_at": "2025-10-03T10:00:00Z",
  "size": { "width": 512, "height": 512, "px": 512 },
  "spacing": 25,
  "bytes": 1
}
{
  "schema_version": "1.0",
  "asset_version": "1.0.0",
  "type": "palette",
  "name": "InkSketch Basic",
  "set": "InkSketch",
  "tags": ["ink", "primary"],
  "author": { "name": "Teknekt", "url": "" },
  "license": { "id": "CC0-1.0", "url": "https://creativecommons.org/publicdomain/zero/1.0/" },
  "created_at": "2025-10-03T10:00:00Z",
  "columns": 8,
  "color_count": 32
}
```
