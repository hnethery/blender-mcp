## 2025-02-27 - Blender Addon UI Inputs
**Learning:** Blender UI inputs should be disabled using `row.enabled = condition` when the underlying process (e.g., server) is active to prevent invalid state changes.
**Action:** Use `row.enabled` or `layout.enabled` for settings that require a restart.

## 2025-02-27 - External Links in Blender
**Learning:** External links in the Blender addon UI are implemented using the `wm.url_open` operator.
**Action:** Use `row.operator("wm.url_open", text="", icon="URL").url = "..."` for help links.
