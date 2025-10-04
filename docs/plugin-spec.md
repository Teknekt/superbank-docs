# Plugin Specification

SuperBank plugins are plain Python modules in `plugins/` with this minimal API:

```python
PLUGIN_INFO = {
  "name": "Human-readable name",
  "description": "Short sentence about what it does",
  "category": "Tools|Brushes|Palettes|Maintenance|Export|Other",
  "icon": "icons/box.svg"  # path under ui/icons (optional)
}

def run(parent=None):
    """Entry point called by the host.
    `parent` is a QWidget/QDialog parent you can use for UI.
    """
    ...
```
