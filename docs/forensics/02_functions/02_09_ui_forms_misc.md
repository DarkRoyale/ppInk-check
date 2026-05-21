## src/ArrowSelDlg.cs

### `ArrowSelDlg(Root r)` (L21-L32)
- **Does:** Constructs the arrow selection dialog.
- **Params:** `r: Root`.
- **Returns:** Constructor.

### `Initialize(Stroke st = null)` (L34-L64)
- **Does:** Initializes arrow head/tail lists and UI state.
- **Params:** `st: Stroke`.
- **Returns:** `void`.

### `ArrowHead_Pnl_Click(object sender, EventArgs e)` (L66-L88)
- **Does:** Handles arrow head selection clicks.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ArrowTail_Pnl_Click(object sender, EventArgs e)` (L90-L113)
- **Does:** Handles arrow tail selection clicks.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `SaveBtn_Click(object sender, EventArgs e)` (L115-L144)
- **Does:** Saves arrow head/tail changes.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `NextBtn_Click(object sender, EventArgs e)` (L146-L150)
- **Does:** Moves to next arrow image.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `PrevBtn_Click(object sender, EventArgs e)` (L152-L156)
- **Does:** Moves to previous arrow image.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `DelBtn_Click(object sender, EventArgs e)` (L158-L168)
- **Does:** Deletes a selected arrow entry.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `AddBtn_Click(object sender, EventArgs e)` (L170-L176)
- **Does:** Adds a new arrow entry.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `QuitBtn_Click(object sender, EventArgs e)` (L178-L180)
- **Does:** Closes the dialog without further changes.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `HeadScaleEd_Validated(object sender, EventArgs e)` (L182-L186)
- **Does:** Validates arrow head scale input.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `TailScaleEd_Validated(object sender, EventArgs e)` (L188-L192)
- **Does:** Validates arrow tail scale input.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ScaleEd_Validating(object sender, CancelEventArgs e)` (L194-L210)
- **Does:** Validates scale text box values.
- **Params:** `sender: object`, `e: CancelEventArgs`.
- **Returns:** `void`.

### `ScaleEd_TextChanged(object sender, EventArgs e)` (L212-L215)
- **Does:** Handles scale field updates.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `TailScaleEd_Leave(object sender, EventArgs e)` (L217-L222)
- **Does:** Handles tail scale field blur.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `HeadScaleEd_Leave(object sender, EventArgs e)` (L224-L229)
- **Does:** Handles head scale field blur.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

## src/CallForm.cs

### `CallForm(Root r)` (L21-L26)
- **Does:** Constructs the call form used before inking starts.
- **Params:** `r: Root`.
- **Returns:** Constructor.

### `timer1_Tick(object sender, EventArgs e)` (L28-L37)
- **Does:** Periodically checks visibility/focus for the call form.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `CallForm_KeyPress(object sender, KeyPressEventArgs e)` (L39-L43)
- **Does:** Handles key press events to trigger actions.
- **Params:** `sender: object`, `e: KeyPressEventArgs`.
- **Returns:** `void`.

### `CallForm_Activated(object sender, EventArgs e)` (L45-L55)
- **Does:** Handles form activation to start inking.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `CallForm_MouseUp(object sender, MouseEventArgs e)` (L57-L61)
- **Does:** Handles mouse-up events on the call form.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `_MouseMove(object sender, MouseEventArgs e)` (L63-L72)
- **Does:** Updates position/drag behavior when moving the call form.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `CallForm_Paint(object sender, PaintEventArgs e)` (L80-L83)
- **Does:** Draws the call form visuals.
- **Params:** `sender: object`, `e: PaintEventArgs`.
- **Returns:** `void`.

## src/ColorPickerDlg.cs

### `Form1()` (L14-L17)
- **Does:** Constructs the color picker dialog wrapper.
- **Params:** None.
- **Returns:** Constructor.

## src/FormAbout.cs

### `FormAbout()` (L13-L16)
- **Does:** Constructs the About dialog.
- **Params:** None.
- **Returns:** Constructor.

### `FormAbout_Load(object sender, EventArgs e)` (L18-L39)
- **Does:** Populates About dialog text on load.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

## src/FormButtonHitter.cs

### `FormButtonHitter(Root root)` (L30-L38)
- **Does:** Constructs the helper form used for click-through mode.
- **Params:** `root: Root`.
- **Returns:** Constructor.

### `Initialize()` (L40-L47)
- **Does:** Initializes form positioning and behavior.
- **Params:** None.
- **Returns:** `void`.

### `FormButtonHitter_Click(object sender, EventArgs e)` (L77-L90)
- **Does:** Handles click events to toggle pointer mode.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ToTopMost()` (L93-L100)
- **Does:** Sets the helper form as top-most.
- **Params:** None.
- **Returns:** `void`.

### `timer1_Tick(object sender, EventArgs e)` (L102-L112)
- **Does:** Periodically syncs helper form position.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `FormButtonHitter_MouseDown(object sender, MouseEventArgs e)` (L123-L127)
- **Does:** Handles mouse down interactions on the helper form.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

## src/FormInput.cs

### `FormInput(string caption, string label, string txt, bool ML, Root rt = null, Stroke stk = null, bool invisible = false)` (L25-L92)
- **Does:** Constructs the text input dialog for text/tag editing.
- **Params:** `caption: string`, `label: string`, `txt: string`, `ML: bool`, `rt: Root`, `stk: Stroke`, `invisible: bool`.
- **Returns:** Constructor.

### `TextIn(string txt)` (L94-L100)
- **Does:** Sets the dialog input text.
- **Params:** `txt: string`.
- **Returns:** `void`.

### `TextOut()` (L102-L108)
- **Does:** Retrieves the current dialog text.
- **Params:** None.
- **Returns:** `string`.

### `FontBtn_Click(object sender, EventArgs e)` (L110-L121)
- **Does:** Opens font selection dialog.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ColorBtn_Click(object sender, EventArgs e)` (L123-L135)
- **Does:** Opens color selection dialog.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `InputML_TextChanged(object sender, EventArgs e)` (L137-L148)
- **Does:** Tracks multi-line input changes.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `TB_CtrlAPressed(object sender, KeyPressEventArgs e)` (L150-L158)
- **Does:** Handles Ctrl+A selection in the textbox.
- **Params:** `sender: object`, `e: KeyPressEventArgs`.
- **Returns:** `void`.

### `btCancel_Click(object sender, EventArgs e)` (L160-L191)
- **Does:** Cancels input and closes the dialog.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `boxingCb_TextChanged(object sender, EventArgs e)` (L193-L219)
- **Does:** Handles frame/boxing option changes.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `FormInput_PreviewKeyDown(object sender, PreviewKeyDownEventArgs e)` (L221-L228)
- **Does:** Handles key preview events for dialog shortcuts.
- **Params:** `sender: object`, `e: PreviewKeyDownEventArgs`.
- **Returns:** `void`.

### `VisibleCb_CheckedChanged(object sender, EventArgs e)` (L230-L237)
- **Does:** Toggles text visibility setting.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

## src/ImageLister.cs

### `ImageLister(Root rt)` (L30-L36)
- **Does:** Constructs the clipart selector dialog.
- **Params:** `rt: Root`.
- **Returns:** Constructor.

### `Initialize()` (L38-L74)
- **Does:** Loads clipart lists and initializes UI.
- **Params:** None.
- **Returns:** `void`.

### `SetFillingOrPattern(bool Pattern = false, int f = Filling.NoFrame)` (L76-L82)
- **Does:** Sets fill/pattern defaults for inserted cliparts.
- **Params:** `Pattern: bool`, `f: int`.
- **Returns:** `void`.

### `OpaqueCorner(Bitmap img, int x0, int y0)` (L84-L95)
- **Does:** Tests whether a corner pixel is opaque.
- **Params:** `img: Bitmap`, `x0: int`, `y0: int`.
- **Returns:** `bool`.

### `FromClipB_Click(object sender, EventArgs e)` (L97-L148)
- **Does:** Loads an image from clipboard into the clipart list.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `LoadImageBtn_Click(object sender, EventArgs e)` (L150-L169)
- **Does:** Opens file picker to add clipart images.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `LoadImage(string fnscaled)` (L171-L202)
- **Does:** Loads an image file and registers it as clipart.
- **Params:** `fnscaled: string`.
- **Returns:** `string` — loaded filename.

### `DelBtn_Click(object sender, EventArgs e)` (L204-L216)
- **Does:** Deletes a selected clipart entry.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `InsertBtn_Click(object sender, EventArgs e)` (L218-L243)
- **Does:** Inserts the selected clipart into the drawing.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `getClipArtData(string fn = null, int fill = -2)` (L245-L291)
- **Does:** Builds a clipart metadata object for insertion.
- **Params:** `fn: string`, `fill: int`.
- **Returns:** `ClipArtData`.

### `CancelBtn_Click(object sender, EventArgs e)` (L293-L296)
- **Does:** Cancels the dialog.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ImageLister_KeyDown(object sender, KeyEventArgs e)` (L298-L305)
- **Does:** Handles keyboard shortcuts in the clipart dialog.
- **Params:** `sender: object`, `e: KeyEventArgs`.
- **Returns:** `void`.

### `FillingCombo_SelectedIndexChanged(object sender, EventArgs e)` (L307-L310)
- **Does:** Updates fill selection for clipart.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

## src/PenModifyDlg.cs

### `PenModifyDlg(Root root)` (L19-L35)
- **Does:** Constructs the pen modification dialog.
- **Params:** `root: Root`.
- **Returns:** Constructor.

### `setColor(int alpha, Color c)` (L37-L40)
- **Does:** Sets the pen color and transparency.
- **Params:** `alpha: int`, `c: Color`.
- **Returns:** `void`.

### `getAlpha()` (L42-L45)
- **Does:** Returns the current alpha value.
- **Params:** None.
- **Returns:** `int`.

### `getColor()` (L47-L50)
- **Does:** Returns the current color.
- **Params:** None.
- **Returns:** `Color`.

### `setWidth(float w)` (L53-L59)
- **Does:** Sets pen width.
- **Params:** `w: float`.
- **Returns:** `void`.

### `WidthTb_Validating(object sender, CancelEventArgs e)` (L61-L66)
- **Does:** Validates pen width input.
- **Params:** `sender: object`, `e: CancelEventArgs`.
- **Returns:** `void`.

### `pboxPenWidthIndicator_Move(object sender, EventArgs e)` (L68-L73)
- **Does:** Updates width indicator position.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `getWidth()` (L75-L78)
- **Does:** Returns the current pen width.
- **Params:** None.
- **Returns:** `float`.

### `setDashStyle(DrawingAttributes pen)` (L80-L104)
- **Does:** Sets dash style UI based on drawing attributes.
- **Params:** `pen: DrawingAttributes`.
- **Returns:** `void`.

### `getDashStyle()` (L106-L123)
- **Does:** Returns selected dash style.
- **Params:** None.
- **Returns:** `DashStyle`.

### `ModifyPen(ref DrawingAttributes pen)` (L125-L129)
- **Does:** Opens dialog to modify pen settings.
- **Params:** `pen: ref DrawingAttributes`.
- **Returns:** `bool`.

### `ModifyPenAndFilling(ref DrawingAttributes pen, ref int fill)` (L131-L167)
- **Does:** Modifies pen and fill settings together.
- **Params:** `pen: ref DrawingAttributes`, `fill: ref int`.
- **Returns:** `bool`.

### `hideWidth()` (L169-L176)
- **Does:** Hides width controls.
- **Params:** None.
- **Returns:** `void`.

### `gpPenWidth_MouseDown(object sender, MouseEventArgs e)` (L180-L183)
- **Does:** Begins width drag operation.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `gpPenWidth_MouseMove(object sender, MouseEventArgs e)` (L185-L195)
- **Does:** Updates width during drag.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `gpPenWidth_MouseUp(object sender, MouseEventArgs e)` (L197-L201)
- **Does:** Ends width drag operation.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `pboxPenWidthIndicator_MouseDown(object sender, MouseEventArgs e)` (L203-L206)
- **Does:** Begins indicator drag.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `pboxPenWidthIndicator_MouseMove(object sender, MouseEventArgs e)` (L208-L212)
- **Does:** Updates indicator during drag.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `pboxPenWidthIndicator_MouseUp(object sender, MouseEventArgs e)` (L214-L217)
- **Does:** Ends indicator drag.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `colorEditorManager_ColorChanged(object sender, EventArgs e)` (L219-L222)
- **Does:** Handles color editor manager change events.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `colorEditor_ColorChanged(object sender, EventArgs e)` (L225-L246)
- **Does:** Updates color selection from picker.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `SVSquare_MouseMove(object sender, MouseEventArgs e)` (L248-L254)
- **Does:** Tracks HSV square mouse movement.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `CursorHSI_MouseMove(object sender, MouseEventArgs e)` (L256-L259)
- **Does:** Tracks HSI cursor movement.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `PenModifyDlg_FormClosing(object sender, FormClosingEventArgs e)` (L261-L276)
- **Does:** Handles close validation for pen dialog.
- **Params:** `sender: object`, `e: FormClosingEventArgs`.
- **Returns:** `void`.

## src/zoomForm.cs

### `ZoomForm()` (L15-L18)
- **Does:** Constructs the zoom tool form.
- **Params:** None.
- **Returns:** Constructor.
