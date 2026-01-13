# Palette's Journal

## 2025-05-18 - [Blender Panel Organization]
**Learning:** Grouping Blender addon properties in UI boxes using `layout.box()` drastically improves readability compared to a flat list. Adding icons to operators clarifies their function.
**Action:** Always use `layout.box()` for distinct feature sets in Blender panels and look for appropriate built-in icons.

## 2025-05-18 - [External Configuration Links]
**Learning:** Adding direct links (using `wm.url_open` operator with an icon) next to API key fields significantly reduces friction for users who need to find where to get their credentials.
**Action:** Whenever a user input requires external configuration (like an API key), always include a helper button linking directly to the provider's dashboard or settings page.
