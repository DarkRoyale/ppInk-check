## src/Hotkey.cs

### `Hotkey.IsValidKey(Keys key)` (L17-L26)
- **Does:** Validates that a key is not a pure modifier key.
- **Params:** `key: Keys`.
- **Returns:** `bool`.

### `Hotkey.ToString()` (L28-L44)
- **Does:** Formats the hotkey using localized key names.
- **Params:** None.
- **Returns:** `string`.

### `Hotkey.ToStringInvariant()` (L45-L61)
- **Does:** Formats the hotkey with invariant key names (Ctrl/Alt/Shift/Win).
- **Params:** None.
- **Returns:** `string`.

### `Hotkey.Parse(string para)` (L63-L98)
- **Does:** Parses a hotkey string into modifiers and key code.
- **Params:** `para: string`.
- **Returns:** `bool`.

### `Hotkey.ModifierMatch(bool control, bool alt, bool shift, bool win)` (L100-L103)
- **Does:** Checks if modifiers match exact state.
- **Params:** `control: bool`, `alt: bool`, `shift: bool`, `win: bool`.
- **Returns:** `bool`.

### `Hotkey.ModifierMatch(bool control, int alt, bool shift, bool win)` (L105-L111)
- **Does:** Checks modifier match with tri-state alt handling.
- **Params:** `control: bool`, `alt: int`, `shift: bool`, `win: bool`.
- **Returns:** `bool`.

### `Hotkey.ConflictWith(Hotkey hotkey)` (L113-L125)
- **Does:** Determines if another hotkey conflicts with this one.
- **Params:** `hotkey: Hotkey`.
- **Returns:** `bool`.

## src/HotkeyInputBox.cs

### `HotkeyInputBox()` (L53-L58)
- **Does:** Initializes the hotkey input textbox control.
- **Params:** None.
- **Returns:** Constructor.

### `UpdateText()` (L60-L63)
- **Does:** Updates textbox display using the current hotkey.
- **Params:** None.
- **Returns:** `void`.

### `SetBackColor()` (L65-L73)
- **Does:** Updates background color based on waiting/conflict state.
- **Params:** None.
- **Returns:** `void`.

### `OnPreviewKeyDown(PreviewKeyDownEventArgs e)` (L75-L138)
- **Does:** Captures key combos to set hotkeys and update UI feedback.
- **Params:** `e: PreviewKeyDownEventArgs`.
- **Returns:** `void`.

### `OnKeyUp(KeyEventArgs e)` (L140-L170)
- **Does:** Finalizes hotkey input and resets waiting state on key release.
- **Params:** `e: KeyEventArgs`.
- **Returns:** `void`.
