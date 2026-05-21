## src/FormOptions.cs (part 1/2)

### `FormOptions(Root root)` (L37-L108)
- **Does:** Constructs the options dialog and binds to the Root settings.
- **Params:** `root: Root`.
- **Returns:** Constructor.

### `FormOptions_Load(object sender, EventArgs e)` (L110-L409)
- **Does:** Populates controls with current configuration and initializes UI state.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `FormOptions_Shown(object sender, EventArgs e)` (L411-L414)
- **Does:** Runs logic after the dialog is shown.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `FormOptions_LocalReload()` (L416-L616)
- **Does:** Reloads localized strings into the UI.
- **Params:** None.
- **Returns:** `void`.

### `comboPensAlpha_TextChanged(object sender, EventArgs e)` (L618-L634)
- **Does:** Updates pen alpha when the alpha combo changes.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `comboPensWidth_TextChanged(object sender, EventArgs e)` (L636-L652)
- **Does:** Updates pen width when the width combo changes.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `comboPensFading_Changed(object sender, EventArgs e)` (L654-L668)
- **Does:** Updates pen fading settings.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `pboxFont_Click(object sender, EventArgs e)` (L670-L686)
- **Does:** Opens the font picker for text tools.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `pboxPens_Click(object sender, EventArgs e)` (L688-L703)
- **Does:** Opens pen configuration dialog.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `cbPens_CheckedChanged(object sender, EventArgs e)` (L705-L710)
- **Does:** Enables/disables pen set configuration.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `FormOptions_FormClosing(object sender, FormClosingEventArgs e)` (L712-L731)
- **Does:** Saves/validates on close and persists settings.
- **Params:** `sender: object`, `e: FormClosingEventArgs`.
- **Returns:** `void`.

### `cbWidthEnabled_CheckedChanged(object sender, EventArgs e)` (L733-L737)
- **Does:** Toggles pen width panel enablement.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `cbEraserEnabled_CheckedChanged(object sender, EventArgs e)` (L739-L742)
- **Does:** Toggles eraser tool enablement.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `cbPointerEnabled_CheckedChanged(object sender, EventArgs e)` (L744-L747)
- **Does:** Toggles pointer tool enablement.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `cbSnapEnabled_CheckedChanged(object sender, EventArgs e)` (L749-L752)
- **Does:** Toggles snapshot feature enablement.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `cbUndoEnabled_CheckedChanged(object sender, EventArgs e)` (L754-L757)
- **Does:** Toggles undo feature enablement.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `cbClearEnabled_CheckedChanged(object sender, EventArgs e)` (L759-L762)
- **Does:** Toggles clear feature enablement.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `cbPanEnabled_CheckedChanged(object sender, EventArgs e)` (L764-L767)
- **Does:** Toggles pan tool enablement.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `cbInkVisibleEnabled_CheckedChanged(object sender, EventArgs e)` (L769-L772)
- **Does:** Toggles ink visibility tool enablement.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `cbWhiteIcon_CheckedChanged(object sender, EventArgs e)` (L774-L778)
- **Does:** Switches between white and red tray icon.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `btSnapPath_Click(object sender, EventArgs e)` (L780-L794)
- **Does:** Opens snapshot path picker dialog.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `tbSnapPath_ModifiedChanged(object sender, EventArgs e)` (L796-L802)
- **Does:** Tracks snapshot path edits.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `timer1_Tick(object sender, EventArgs e)` (L804-L830)
- **Does:** Periodic timer to refresh UI state.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `comboBox1_SelectedIndexChanged(object sender, EventArgs e)` (L832-L835)
- **Does:** Updates settings when a combo box changes.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `cbAllowDragging_CheckedChanged(object sender, EventArgs e)` (L837-L840)
- **Does:** Toggles toolbar dragging option.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `cbToolsEnabled_CheckedChanged(object sender, EventArgs e)` (L842-L845)
- **Does:** Toggles tools enablement.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `SaveWindowPosBtn_Click(object sender, EventArgs e)` (L847-L851)
- **Does:** Saves window position settings.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `SaveConfigBtn_Click(object sender, EventArgs e)` (L853-L875)
- **Does:** Persists configuration to disk.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `Float_Validating(object sender, CancelEventArgs e)` (L877-L888)
- **Does:** Validates float input fields.
- **Params:** `sender: object`, `e: CancelEventArgs`.
- **Returns:** `void`.

### `DefaultFontBtn_Click(object sender, EventArgs e)` (L890-L901)
- **Does:** Opens default font selector.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `TagFontBtn_Click(object sender, EventArgs e)` (L903-L914)
- **Does:** Opens tag font selector.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ArrHdAperture_Validated(object sender, EventArgs e)` (L917-L920)
- **Does:** Validates arrow head aperture input.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ArrHdLength_Validated(object sender, EventArgs e)` (L922-L925)
- **Does:** Validates arrow head length input.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ShowFloatingWinCb_Click(object sender, EventArgs e)` (L927-L951)
- **Does:** Toggles floating window visibility.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `Magnet_TB_Validated(object sender, EventArgs e)` (L953-L962)
- **Does:** Validates magnet radius settings.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `DefArrStartCb_CheckedChanged(object sender, EventArgs e)` (L964-L967)
- **Does:** Toggles default arrow start behavior.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `OpenIntoSnapCb_CheckedChanged(object sender, EventArgs e)` (L969-L972)
- **Does:** Toggles opening directly into snapshot mode.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `WidthAtPenSelCb_CheckedChanged(object sender, EventArgs e)` (L974-L977)
- **Does:** Toggles apply-width-on-selection option.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ToolBarHeight_Validated(object sender, EventArgs e)` (L979-L982)
- **Does:** Validates toolbar height input.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ValidateOnEnter(object sender, KeyPressEventArgs e)` (L984-L992)
- **Does:** Commits validation when Enter is pressed.
- **Params:** `sender: object`, `e: KeyPressEventArgs`.
- **Returns:** `void`.

### `BoardAtOpenCombo_SelectedIndexChanged(object sender, EventArgs e)` (L994-L997)
- **Does:** Updates board-at-open selection.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `BoardCustColorPnl_Click(object sender, EventArgs e)` (L999-L1018)
- **Does:** Picks custom board background color.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `WsUrlTxt_TextChanged(object sender, EventArgs e)` (L1020-L1023)
- **Does:** Updates OBS WebSocket URL.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `WsPwdTxt_TextChanged(object sender, EventArgs e)` (L1025-L1028)
- **Does:** Updates OBS WebSocket password.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `FfmpegCmdTxt_TextChanged(object sender, EventArgs e)` (L1030-L1033)
- **Does:** Updates FFmpeg command template.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `VideoOption_Changed(object sender, EventArgs e)` (L1035-L1042)
- **Does:** Updates video recording options.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ToolbarDwg_Click(object sender, EventArgs e)` (L1044-L1066)
- **Does:** Toggles toolbar background selection.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `AltTabActivateCb_CheckedChanged(object sender, EventArgs e)` (L1068-L1071)
- **Does:** Toggles Alt-Tab activation behavior.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ClipartsSelBtn_Click(object sender, EventArgs e)` (L1073-L1092)
- **Does:** Opens clipart selection dialog.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ClipBtn_Click(object sender, EventArgs e)` (L1094-L1112)
- **Does:** Opens clipart button configuration.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `cbLoadSaveEnabled_CheckedChanged(object sender, EventArgs e)` (L1114-L1117)
- **Does:** Toggles stroke load/save enablement.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ToolbarOrientationBtn_Click(object sender, EventArgs e)` (L1119-L1125)
- **Does:** Rotates toolbar orientation.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `FadingTimeEd_Validating(object sender, CancelEventArgs e)` (L1127-L1147)
- **Does:** Validates fading time input.
- **Params:** `sender: object`, `e: CancelEventArgs`.
- **Returns:** `void`.

### `ZoomWidthEd_Validating(object sender, CancelEventArgs e)` (L1149-L1155)
- **Does:** Validates zoom width input.
- **Params:** `sender: object`, `e: CancelEventArgs`.
- **Returns:** `void`.

### `ZoomHeightEd_Validating(object sender, CancelEventArgs e)` (L1157-L1163)
- **Does:** Validates zoom height input.
- **Params:** `sender: object`, `e: CancelEventArgs`.
- **Returns:** `void`.
