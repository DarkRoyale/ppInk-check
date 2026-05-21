## src/FormDisplay.cs

### `FormDisplay(Root root)` (L70-L87)
- **Does:** Constructs the display form, initializes transparency matrices, and runs initialization.
- **Params:** `root: Root`.
- **Returns:** Constructor.

### `Initialize()` (L89-L217)
- **Does:** Allocates canvases/DCs, sizes the display window, and prepares drawing surfaces.
- **Params:** None.
- **Returns:** `void`.

### `ToTopMostThrough()` (L219-L227)
- **Does:** Sets the display form to top-most and click-through.
- **Params:** None.
- **Returns:** `void`.

### `ClearCanvus()` (L229-L233)
- **Does:** Clears the primary canvas and redraws the display.
- **Params:** None.
- **Returns:** `void`.

### `ClearCanvus(Graphics g)` (L235-L242)
- **Does:** Clears a provided graphics canvas.
- **Params:** `g: Graphics`.
- **Returns:** `void`.

### `DrawBorder(bool Focus, Graphics g = null)` (L244-L253)
- **Does:** Draws the window mode border on the display surface.
- **Params:** `Focus: bool`, `g: Graphics`.
- **Returns:** `void`.

### `DrawSnapping(Rectangle rect)` (L256-L275)
- **Does:** Draws the snapshot selection rectangle overlay.
- **Params:** `rect: Rectangle`.
- **Returns:** `void`.

### `DrawButtons(bool redrawbuttons = true, bool exiting = false)` (L277-L280)
- **Does:** Convenience wrapper to redraw toolbar buttons.
- **Params:** `redrawbuttons: bool`, `exiting: bool`.
- **Returns:** `void`.

### `DrawButtons(Graphics g, bool redrawbuttons = true, bool exiting = false)` (L282-L351)
- **Does:** Renders toolbar button overlays onto the canvas.
- **Params:** `g: Graphics`, `redrawbuttons: bool`, `exiting: bool`.
- **Returns:** `void`.

### `DrawOneStroke(Graphics g, Stroke st, DrawingAttributes DA = null, Bitmap bmp = null)` (L353-L414)
- **Does:** Renders a single stroke, including text and images.
- **Params:** `g: Graphics`, `st: Stroke`, `DA: DrawingAttributes`, `bmp: Bitmap`.
- **Returns:** `void`.

### `DrawStrokes()` (L416-L419)
- **Does:** Redraws all strokes on the display.
- **Params:** None.
- **Returns:** `void`.

### `DrawStrokes(Graphics g)` (L421-L615)
- **Does:** Renders all strokes onto the provided graphics surface.
- **Params:** `g: Graphics`.
- **Returns:** `void`.

### `DrawStrokes(Bitmap bmp, bool IgnoreBackground = false)` (L619-L776)
- **Does:** Draws strokes onto a bitmap, optionally ignoring background.
- **Params:** `bmp: Bitmap`, `IgnoreBackground: bool`.
- **Returns:** `void`.

### `MoveStrokes(int dy)` (L779-L790)
- **Does:** Moves strokes vertically by a pixel delta.
- **Params:** `dy: int`.
- **Returns:** `void`.

### `N1(int i, int j)` (L798-L803)
- **Does:** Reads a pixel value from the current screen buffer.
- **Params:** `i: int`, `j: int`.
- **Returns:** `uint`.

### `N2(int i, int j)` (L804-L809)
- **Does:** Reads a pixel value from the current screen buffer (second channel).
- **Params:** `i: int`, `j: int`.
- **Returns:** `uint`.

### `L(int i, int j)` (L810-L815)
- **Does:** Reads a pixel value from the previous screen buffer.
- **Params:** `i: int`, `j: int`.
- **Returns:** `uint`.

### `Nnext1()` (L817-L821)
- **Does:** Advances to the next pixel in the current buffer and returns its value.
- **Params:** None.
- **Returns:** `uint`.

### `Nnext2()` (L822-L826)
- **Does:** Advances to the next pixel in the secondary buffer and returns its value.
- **Params:** None.
- **Returns:** `uint`.

### `Lnext()` (L827-L831)
- **Does:** Advances to the next pixel in the previous buffer and returns its value.
- **Params:** None.
- **Returns:** `uint`.

### `SnapShot(Rectangle rect, string dest = "")` (L833-L923)
- **Does:** Captures a snapshot of the selected region and saves it to disk.
- **Params:** `rect: Rectangle`, `dest: string`.
- **Returns:** `void`.

### `PenForDrawOn(DrawingAttributes dr, DashStyle st)` (L925-L933)
- **Does:** Creates a pen instance based on drawing attributes and dash style.
- **Params:** `dr: DrawingAttributes`, `st: DashStyle`.
- **Returns:** `Pen`.

### `DrawLineOnGraphic(Graphics g, int CursorX0, int CursorY0, int CursorX, int CursorY, DrawingAttributes dr = null, DashStyle st = DashStyle.Solid)` (L935-L941)
- **Does:** Draws a line onto the output canvas.
- **Params:** `g: Graphics`, `CursorX0, CursorY0, CursorX, CursorY: int`, `dr: DrawingAttributes`, `st: DashStyle`.
- **Returns:** `void`.

### `DrawRectOnGraphic(Graphics g, int CursorX0, int CursorY0, int CursorX, int CursorY, DrawingAttributes dr = null, DashStyle st = DashStyle.Solid)` (L942-L950)
- **Does:** Draws a rectangle onto the output canvas.
- **Params:** `g: Graphics`, `CursorX0, CursorY0, CursorX, CursorY: int`, `dr: DrawingAttributes`, `st: DashStyle`.
- **Returns:** `void`.

### `DrawImagesOnGraphic(Graphics g, List<Point> pts, Image img, int W, int H, DrawingAttributes dr = null, DashStyle st = DashStyle.Solid, bool OnLine = false)` (L951-L984)
- **Does:** Draws images along points (optionally rotated on a line).
- **Params:** `g: Graphics`, `pts: List<Point>`, `img: Image`, `W,H: int`, `dr: DrawingAttributes`, `st: DashStyle`, `OnLine: bool`.
- **Returns:** `void`.

### `DrawEllipseOnGraphic(Graphics g, int CursorX0, int CursorY0, int CursorX, int CursorY, DrawingAttributes dr = null, DashStyle st = DashStyle.Solid)` (L985-L993)
- **Does:** Draws an ellipse onto the output canvas.
- **Params:** `g: Graphics`, `CursorX0, CursorY0, CursorX, CursorY: int`, `dr: DrawingAttributes`, `st: DashStyle`.
- **Returns:** `void`.

### `DrawArrowOnGraphic(Graphics g, int CursorX0, int CursorY0, int CursorX, int CursorY, DrawingAttributes dr = null, DashStyle st = DashStyle.Solid)` (L995-L1008)
- **Does:** Draws an arrow onto the output canvas.
- **Params:** `g: Graphics`, `CursorX0, CursorY0, CursorX, CursorY: int`, `dr: DrawingAttributes`, `st: DashStyle`.
- **Returns:** `void`.

### `DrawCustomOnGraphic(Graphics g, int CursorX0, int CursorY0, int CursorX, int CursorY)` (L1010-L1057)
- **Does:** Draws a custom shape or pattern stroke.
- **Params:** `g: Graphics`, `CursorX0, CursorY0, CursorX, CursorY: int`.
- **Returns:** `void`.

### `Test()` (L1059-L1126)
- **Does:** Debug/test routine for drawing behavior.
- **Params:** None.
- **Returns:** `int`.

### `UpdateFormDisplay(bool draw, bool prepared = false)` (L1129-L1187)
- **Does:** Redraws the display based on current strokes and state.
- **Params:** `draw: bool`, `prepared: bool`.
- **Returns:** `void`.

### `timer1_Tick(object sender, EventArgs e)` (L1194-L1389)
- **Does:** Periodic update for fade effects, animation, and screen capture.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `DrawInProgressStroke(GameOverlay.Drawing.Graphics g)` (L1391-L1401)
- **Does:** Draws the in-progress stroke for DirectX overlay rendering.
- **Params:** `g: GameOverlay.Drawing.Graphics`.
- **Returns:** `void`.

### `DXUpdateFormDisplay(bool prepared = false)` (L1403-L1410)
- **Does:** Updates the DirectX overlay output.
- **Params:** `prepared: bool`.
- **Returns:** `void`.

### `timerDX_Tick(object sender, EventArgs e)` (L1412-L1465)
- **Does:** Timer tick handler for DirectX overlay updates.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `FormDisplay_VisibleChanged(object sender, EventArgs e)` (L1467-L1478)
- **Does:** Responds to visibility changes to pause/resume timers.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `FormDisplay_FormClosed(object sender, FormClosedEventArgs e)` (L1480-L1505)
- **Does:** Cleans up device contexts and graphics resources on close.
- **Params:** `sender: object`, `e: FormClosedEventArgs`.
- **Returns:** `void`.

### `HasFocus()` (L1510-L1523)
- **Does:** Checks whether the display form has focus or is active.
- **Params:** None.
- **Returns:** `bool`.
