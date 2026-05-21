## src/FormCollection.cs (part 2/3)

### `StrokeLength(Stroke st)` (L3624-L3641)
- **Does:** Computes the length of a stroke in pixels.
- **Params:** `st: Stroke`.
- **Returns:** `double`.

### `MeasureStroke(Stroke st)` (L3644-L3695)
- **Does:** Formats measurement text for a stroke.
- **Params:** `st: Stroke`.
- **Returns:** `string`.

### `MeasureAllStrokes(Strokes sts1, Strokes sts2, Stroke Hovered, bool LengthOnly = false)` (L3697-L3728)
- **Does:** Computes measurement text for selected/hovered strokes.
- **Params:** `sts1: Strokes`, `sts2: Strokes`, `Hovered: Stroke`, `LengthOnly: bool`.
- **Returns:** `string`.

### `ActivateStrokesInput(bool active)` (L3730-L3754)
- **Does:** Enables or disables stroke input and selection on the InkOverlay.
- **Params:** `active: bool`.
- **Returns:** `void`.

### `ToTransparent()` (L3756-L3761)
- **Does:** Sets the toolbar background to transparent.
- **Params:** None.
- **Returns:** `void`.

### `ToTopMost()` (L3763-L3767)
- **Does:** Brings the toolbar form to top-most.
- **Params:** None.
- **Returns:** `void`.

### `ToThrough()` (L3769-L3777)
- **Does:** Enables click-through mode for the toolbar window.
- **Params:** None.
- **Returns:** `void`.

### `ToUnThrough()` (L3779-L3790)
- **Does:** Disables click-through mode for the toolbar window.
- **Params:** None.
- **Returns:** `void`.

### `EnterEraserMode(bool enter)` (L3792-L3820)
- **Does:** Switches cursor and ink collector settings for erasing mode.
- **Params:** `enter: bool`.
- **Returns:** `void`.

### `SelectTool(int tool, int filled = -1)` (L3823-L4181)
- **Does:** Updates selected tool/fill state and refreshes toolbar visuals.
- **Params:** `tool: int`, `filled: int`.
- **Returns:** `void`.

### `SelectPen(int pen)` (L4183-L4441)
- **Does:** Changes the active pen, adjusts UI icons, and updates drawing attributes.
- **Params:** `pen: int`.
- **Returns:** `void`.

### `RetreatAndExit(bool Quick = false)` (L4443-L4481)
- **Does:** Handles exit animation/cleanup when leaving ink mode.
- **Params:** `Quick: bool`.
- **Returns:** `void`.

### `btDock_Click(object sender, EventArgs e)` (L4483-L4522)
- **Does:** Toggles docking when the dock button is clicked.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `btWindowMode_Click2(object sender, EventArgs e)` (L4524-L4553)
- **Does:** Toggles window mode selection state.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `btPointer_Click(object sender, EventArgs e)` (L4556-L4595)
- **Does:** Enters or exits pointer mode when the pointer button is clicked.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `AddPointerSnaps()` (L4597-L4615)
- **Does:** Captures pointer-mode snapshots based on key state.
- **Params:** None.
- **Returns:** `void`.

### `StartStopPickUpColor(int Active)` (L4617-L4664)
- **Does:** Starts, applies, or cancels color picker mode.
- **Params:** `Active: int` — 1=start, 2=apply, 0=cancel.
- **Returns:** `void`.

### `btPenWidth_Click(object sender, EventArgs e)` (L4666-L4703)
- **Does:** Handles pen width button clicks and opens width control.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `StartSnapshot(bool Continue)` (L4705-L4734)
- **Does:** Starts snapshot capture mode with optional continuation.
- **Params:** `Continue: bool`.
- **Returns:** `void`.

### `btSnap_Click(object sender, EventArgs e)` (L4736-L4779)
- **Does:** Handles snapshot button click behavior.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ExitSnapping(bool cancel)` (L4781-L4802)
- **Does:** Exits snapshot mode, optionally canceling.
- **Params:** `cancel: bool`.
- **Returns:** `void`.

### `btStop_Click(object sender, EventArgs e)` (L4804-L4813)
- **Does:** Stops inking and exits drawing mode.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `gpPenWidth_MouseDown(object sender, MouseEventArgs e)` (L4860-L4863)
- **Does:** Starts pen width drag interaction.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `gpPenWidth_MouseMove(object sender, MouseEventArgs e)` (L4865-L4877)
- **Does:** Updates pen width during drag.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `gpPenWidth_MouseUp(object sender, MouseEventArgs e)` (L4879-L4894)
- **Does:** Finishes pen width drag interaction.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `pboxPenWidthIndicator_MouseDown(object sender, MouseEventArgs e)` (L4896-L4899)
- **Does:** Begins dragging pen width indicator.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `pboxPenWidthIndicator_MouseMove(object sender, MouseEventArgs e)` (L4901-L4914)
- **Does:** Updates pen width indicator during drag.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `pboxPenWidthIndicator_MouseUp(object sender, MouseEventArgs e)` (L4916-L4924)
- **Does:** Ends drag operation for the pen width indicator.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `SetPenTipCursor()` (L4926-L4993)
- **Does:** Sets the cursor to a pen tip image based on state.
- **Params:** None.
- **Returns:** `void`.

### `KeyCodeState(SnapInPointerKeys k)` (L5041-L5053)
- **Does:** Checks modifier key state for pointer snapshots.
- **Params:** `k: SnapInPointerKeys`.
- **Returns:** `bool`.

### `tiSlide_Tick(object sender, EventArgs e)` (L5056-L6079)
- **Does:** Handles toolbar animation and UI updates over time.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `recomputePensSet(int firstPen = -1, int currentPen = -1)` (L6081-L6116)
- **Does:** Rebuilds pen button icons based on current pen set.
- **Params:** `firstPen: int`, `currentPen: int`.
- **Returns:** `void`.

### `PenWidth_Change(int n)` (L6118-L6128)
- **Does:** Adjusts pen width by a delta.
- **Params:** `n: int`.
- **Returns:** `void`.

### `IsInsideVisibleScreen(int x, int y)` (L6130-L6146)
- **Does:** Tests whether coordinates fall within visible screens.
- **Params:** `x: int`, `y: int`.
- **Returns:** `bool`.

### `gpButtons_MouseDown(object sender, MouseEventArgs e)` (L6151-L6162)
- **Does:** Handles mouse down on toolbar buttons (dragging/selection).
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `gpButtons_MouseMove(object sender, MouseEventArgs e)` (L6164-L6171)
- **Does:** Handles toolbar button mouse move for drag operations.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `gpButtons_MouseUp(object sender, MouseEventArgs e)` (L6173-L6176)
- **Does:** Handles toolbar button mouse up events.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `btInkVisible_Click(object sender, EventArgs e)` (L6178-L6187)
- **Does:** Toggles ink visibility when the visibility button is clicked.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `AddBackGround(int A, int B, int C, int D)` (L6189-L6198)
- **Does:** Adds a background stroke region.
- **Params:** `A, B, C, D: int`.
- **Returns:** `Stroke`.

### `SelectCleanBackground()` (L6200-L6250)
- **Does:** Chooses a background stroke and clears/creates as needed.
- **Params:** None.
- **Returns:** `int`.

### `FadingToggle(int pen)` (L6252-L6268)
- **Does:** Toggles fading property for a pen.
- **Params:** `pen: int`.
- **Returns:** `void`.

### `btClear_Click(object sender, EventArgs e)` (L6270-L6319)
- **Does:** Clears strokes or selection based on state.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `btUndo_Click(object sender, EventArgs e)` (L6321-L6339)
- **Does:** Executes undo behavior when undo button is clicked.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `SelectNextLineStyle(object sender)` (L6341-L6362)
- **Does:** Cycles to the next enabled line style for the current pen.
- **Params:** `sender: object`.
- **Returns:** `void`.

### `btColor_LongClick(object sender)` (L6364-L6403)
- **Does:** Handles long-click color edits for pens.
- **Params:** `sender: object`.
- **Returns:** `void`.

### `btColor_Click(object sender, EventArgs e)` (L6405-L6444)
- **Does:** Handles pen color button click actions.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ExtraPensBtn_Click(object sender, EventArgs e)` (L6448-L6458)
- **Does:** Toggles the extra pen set display.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `btVideo_Click(object sender, EventArgs e)` (L6460-L6495)
- **Does:** Toggles video recording state or UI.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `VideoRecordStart()` (L6497-L6523)
- **Does:** Starts OBS-based video recording.
- **Params:** None.
- **Returns:** `void`.

### `VideoRecordStartFFmpeg(Rectangle rect)` (L6524-L6562)
- **Does:** Starts FFmpeg video recording for a specified rectangle.
- **Params:** `rect: Rectangle`.
- **Returns:** `void`.

### `VideoRecordStop()` (L6713-L6734)
- **Does:** Stops video recording and resets UI.
- **Params:** None.
- **Returns:** `void`.

### `VideoRecordPause()` (L6746-L6756)
- **Does:** Pauses active video recording.
- **Params:** None.
- **Returns:** `void`.

### `VideoRecordResume()` (L6758-L6761)
- **Does:** Resumes paused video recording.
- **Params:** None.
- **Returns:** `void`.

### `btClear_RightToLeftChanged(object sender, EventArgs e)` (L6776-L6787)
- **Does:** Handles clear button RTL state changes.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `SetTagNumber(string init = "")` (L6789-L6830)
- **Does:** Sets or resets the numbering tag counter.
- **Params:** `init: string`.
- **Returns:** `void`.
