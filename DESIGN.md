# Design

Preserve the incumbent Hugging Face viewer design for this extension. Reference authority is the existing `src/app/globals.css`, episode tabs, playback controls, and AGENTS.md; no replacement visual direction.

Use Source Sans 3 for controls and IBM Plex Mono for coordinate values. Retain semantic surface/text tokens, dark and light themes, and LeRobot orange for primary actions. New controls use solid opaque fills and existing 6px radii; no gradients, outlined buttons, decorative copy, Unicode arrows, or dot separators.

3D Replay remains the primary surface. Place Scene and Axes controls above the viewport. Open the scene editor alongside the viewport on wide displays and below it with a bounded scroll area on narrow displays. Use labeled native inputs, visible focus rings, keyboard-operable controls, inline import errors, and loading states. Hide complexity behind selection and native disclosure controls. Coordinate labels must name units; identify manually added context as user-authored.

World axes use the conventional red X, green Y, blue Z colors. Grid spacing is 0.1 meter. Keep animations tied to recorded motion only. Scene loading never changes the original dataset.
