## src/FormCollection.cs (part 1/3)

### `RegisterTouchWindow(IntPtr hWnd, RegisterTouchFlags flags)` (L34-L35)
- **Does:** P/Invoke registration for touch input on the form.
- **Params:** `hWnd: IntPtr`, `flags: RegisterTouchFlags`.
- **Returns:** `bool`.

### `MyNativeMethods.LoadCustomCursor(string path)` (L40-L49)
- **Does:** Loads a custom cursor from file using a native cursor handle.
- **Params:** `path: string` — cursor file path.
- **Returns:** `Cursor`.

### `MyNativeMethods.LoadCursorFromFile(string path)` (L51)
- **Does:** P/Invoke for loading a cursor handle from file.
- **Params:** `path: string`.
- **Returns:** `IntPtr`.

### `BuildArrowBtn(string head, string tail, Color col)` (L356-L384)
- **Does:** Renders a toolbar bitmap for arrow head/tail previews.
- **Params:** `head: string`, `tail: string`, `col: Color`.
- **Returns:** `Bitmap`.

### `SetButtonPosition(Button previous, Button current, int spacing, int Orient = -1)` (L386-L411)
- **Does:** Positions a toolbar button relative to another based on orientation.
- **Params:** `previous: Button`, `current: Button`, `spacing: int`, `Orient: int`.
- **Returns:** `void`.

### `SetSmallButtonNext(Button previous, Button current, int incr, int Orient = -1)` (L413-L428)
- **Does:** Positions a small stacked button relative to another.
- **Params:** `previous: Button`, `current: Button`, `incr: int`, `Orient: int`.
- **Returns:** `void`.

### `buildPenIcon(Color col, int transparency, bool Sel, bool Fading, string LineStyle = "Stroke", float width = 100.0F)` (L430-L462)
- **Does:** Builds a pen button bitmap with color, transparency, and line style overlays.
- **Params:** `col: Color`, `transparency: int`, `Sel: bool`, `Fading: bool`, `LineStyle: string`, `width: float`.
- **Returns:** `Bitmap`.

### `GetIconInfo(IntPtr hIcon, ref IconInfo pIconInfo)` (L472-L474)
- **Does:** P/Invoke to read icon metadata.
- **Params:** `hIcon: IntPtr`, `pIconInfo: ref IconInfo`.
- **Returns:** `bool`.

### `CreateIconIndirect(ref IconInfo icon)` (L476)
- **Does:** P/Invoke to create an icon/cursor from icon info.
- **Params:** `icon: ref IconInfo`.
- **Returns:** `IntPtr`.

### `CreateCursorFromBitmap(Bitmap bmp, int hotX = -1, int hotY = -1)` (L479-L491)
- **Does:** Creates a cursor from a bitmap and sets its hotspot.
- **Params:** `bmp: Bitmap`, `hotX: int`, `hotY: int`.
- **Returns:** `Cursor`.

### `buildColorPicker(Color col, int transparency)` (L493-L513)
- **Does:** Builds a colored picker icon bitmap with alpha.
- **Params:** `col: Color`, `transparency: int`.
- **Returns:** `Bitmap`.

### `FormCollection(Root root)` (L515-L592)
- **Does:** Constructs the toolbar form and initializes buttons, InkOverlay, and resources.
- **Params:** `root: Root`.
- **Returns:** Constructor.

### `ConvertMeasureLength(double hl)` (L594-L597)
- **Does:** Converts a HIMETRIC length using the configured scale.
- **Params:** `hl: double`.
- **Returns:** `double`.

### `Initialize()` (L603-L1431)
- **Does:** Builds the toolbar UI, loads resources, wires events, and prepares tool state.
- **Params:** None.
- **Returns:** `void`.

### `SetSubBarPosition(Panel Tb, Button RefButton)` (L1433-L1449)
- **Does:** Positions a sub-toolbar panel near a reference button.
- **Params:** `Tb: Panel`, `RefButton: Button`.
- **Returns:** `void`.

### `setPenWidthBarPosition()` (L1451-L1454)
- **Does:** Positions the pen width panel on screen.
- **Params:** None.
- **Returns:** `void`.

### `setClipArtDlgPosition()` (L1456-L1477)
- **Does:** Positions the clipart dialog relative to the toolbar.
- **Params:** None.
- **Returns:** `void`.

### `AltTabActivate()` (L1488-L1513)
- **Does:** Ensures forms are correctly positioned/visible after Alt-Tab focus changes.
- **Params:** None.
- **Returns:** `void`.

### `SetVidBgImage()` (L1568-L1586)
- **Does:** Updates the video recording toolbar background based on state.
- **Params:** None.
- **Returns:** `void`.

### `IC_MouseWheel(object sender, CancelMouseEventArgs e)` (L1588-L1634)
- **Does:** Handles mouse wheel actions to adjust pen width, colors, or tag size.
- **Params:** `sender: object`, `e: CancelMouseEventArgs`.
- **Returns:** `void`.

### `AltKeyPressed()` (L1636-L1639)
- **Does:** Checks if Alt is currently pressed.
- **Params:** None.
- **Returns:** `bool`.

### `btAllButtons_MouseDown(object sender, MouseEventArgs e)` (L1641-L1649)
- **Does:** Handles toolbar button press and starts long-click tracking.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `btAllButtons_MouseUp(object sender, MouseEventArgs e)` (L1651-L1659)
- **Does:** Ends toolbar button press and resets movement state.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `btAllButtons_RightClick(object sender, EventArgs e)` (L1661-L1670)
- **Does:** Maps context-menu right-clicks back to button click handling.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `longClickTimer_Tick(object sender, EventArgs e)` (L1672-L1682)
- **Does:** Simulates long-click behavior for toolbar buttons.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `getStrokeProperties(Stroke st)` (L1684-L1698)
- **Does:** Determines fill type based on stroke extended properties.
- **Params:** `st: Stroke`.
- **Returns:** `int` — fill value.

### `setStrokeProperties(ref Stroke st, int FilledSelected)` (L1700-L1728)
- **Does:** Applies fill/fading metadata to a stroke.
- **Params:** `st: ref Stroke`, `FilledSelected: int`.
- **Returns:** `void`.

### `AddEllipseStroke(int CursorX0, int CursorY0, int CursorX, int CursorY, int FilledSelected)` (L1731-L1753)
- **Does:** Creates an ellipse stroke from cursor points and applies fill attributes.
- **Params:** `CursorX0, CursorY0, CursorX, CursorY: int`, `FilledSelected: int`.
- **Returns:** `Stroke`.

### `AddRectStroke(int CursorX0, int CursorY0, int CursorX, int CursorY, int FilledSelected)` (L1755-L1781)
- **Does:** Creates a rectangle stroke and applies fill attributes.
- **Params:** `CursorX0, CursorY0, CursorX, CursorY: int`, `FilledSelected: int`.
- **Returns:** `Stroke`.

### `AddImageStroke(int CursorX0, int CursorY0, int CursorX, int CursorY, string fn, int Filling = -10)` (L1783-L1832)
- **Does:** Creates a stroke representing a clipart/image with metadata for size/position.
- **Params:** `CursorX0, CursorY0, CursorX, CursorY: int`, `fn: string`, `Filling: int`.
- **Returns:** `Stroke`.

### `buildAni(string fn)` (L1834-L1862)
- **Does:** Initializes APNG animation metadata from filename and image data.
- **Params:** `fn: string`.
- **Returns:** `AnimationStructure`.

### `AddLineStroke(int CursorX0, int CursorY0, int CursorX, int CursorY)` (L1864-L1880)
- **Does:** Creates a line stroke between two points.
- **Params:** `CursorX0, CursorY0, CursorX, CursorY: int`.
- **Returns:** `Stroke`.

### `ExtendPolyLineStroke(Stroke st, int CursorX, int CursorY, int FilledSelected)` (L1882-L1902)
- **Does:** Extends an existing polyline stroke with a new point.
- **Params:** `st: Stroke`, `CursorX: int`, `CursorY: int`, `FilledSelected: int`.
- **Returns:** `Stroke`.

### `ArrowVarLen()` (L1904-L1907)
- **Does:** Computes arrowhead length based on pen width.
- **Params:** None.
- **Returns:** `double`.

### `PrepareArrowBitmap(string fn, Color col, int transparency, double PenWidth_p, float angle_r, out int conn_len)` (L1909-L1955)
- **Does:** Renders an arrowhead bitmap scaled/rotated to pen size and angle.
- **Params:** `fn: string`, `col: Color`, `transparency: int`, `PenWidth_p: double`, `angle_r: float`, `conn_len: out int`.
- **Returns:** `Bitmap`.

### `AddArrowStroke(int CursorX0, int CursorY0, int CursorX, int CursorY)` (L1957-L2004)
- **Does:** Creates an arrow stroke with head/tail image metadata.
- **Params:** `CursorX0, CursorY0, CursorX, CursorY: int`.
- **Returns:** `Stroke`.

### `AddNumberTagStroke(int CursorX0, int CursorY0, int CursorX, int CursorY, string txt)` (L2006-L2026)
- **Does:** Creates a numbered tag stroke with text metadata.
- **Params:** `CursorX0, CursorY0, CursorX, CursorY: int`, `txt: string`.
- **Returns:** `Stroke`.

### `AddTextStroke(int CursorX0, int CursorY0, int CursorX, int CursorY, string txt, StringAlignment Align, int fil_in = -1)` (L2029-L2073)
- **Does:** Creates a text stroke with alignment and background fill metadata.
- **Params:** `CursorX0, CursorY0, CursorX, CursorY: int`, `txt: string`, `Align: StringAlignment`, `fil_in: int`.
- **Returns:** `Stroke`.

### `ModifyTextInStroke(Stroke stk, string txt, bool invisibleDlg = false)` (L2076-L2110)
- **Does:** Opens the text editor dialog to modify text in an existing stroke.
- **Params:** `stk: Stroke`, `txt: string`, `invisibleDlg: bool`.
- **Returns:** `DialogResult`.

### `NearestStroke(Point pt, bool ptInPixel, out Stroke minStroke, out float pos, bool Search4Text = true, bool butLast = false, bool Magnet = true)` (L2112-L2145)
- **Does:** Finds the closest stroke to a point, optionally restricted to text.
- **Params:** `pt: Point`, `ptInPixel: bool`, `minStroke: out Stroke`, `pos: out float`, `Search4Text: bool`, `butLast: bool`, `Magnet: bool`.
- **Returns:** `float` — distance.

### `MagneticEffect(int cursorX0, int cursorY0, ref int cursorX, ref int cursorY, bool Magnetic = false)` (L2147-L2301)
- **Does:** Adjusts cursor coordinates to snap to nearby strokes or axes.
- **Params:** `cursorX0, cursorY0: int`, `cursorX: ref int`, `cursorY: ref int`, `Magnetic: bool`.
- **Returns:** `void`.

### `Scale(Strokes Sel, Stroke Hover, int Xc, int Yc, int X0, int Y0, int X, int Y)` (L2306-L2331)
- **Does:** Computes a scale factor and applies scaling to selected strokes.
- **Params:** `Sel: Strokes`, `Hover: Stroke`, `Xc, Yc, X0, Y0, X, Y: int`.
- **Returns:** `void`.

### `Rotate(Strokes Sel, Stroke Hover, int Xc, int Yc, int X0, int Y0, int X, int Y)` (L2333-L2359)
- **Does:** Computes a rotation angle and applies rotation to selected strokes.
- **Params:** `Sel: Strokes`, `Hover: Stroke`, `Xc, Yc, X0, Y0, X, Y: int`.
- **Returns:** `void`.

### `ScaleRotate(Strokes Sel, Stroke Hover, int Xc, int Yc, double k, double deg, bool applyOnPen = true)` (L2361-L2487)
- **Does:** Applies scaling/rotation to strokes and updates embedded metadata.
- **Params:** `Sel: Strokes`, `Hover: Stroke`, `Xc, Yc: int`, `k: double`, `deg: double`, `applyOnPen: bool`.
- **Returns:** `void`.

### `mInkObject_StrokesDeleting(object sender, InkOverlayStrokesDeletingEventArgs e)` (L2488-L2493)
- **Does:** Marks deletion strokes when strokes are removed.
- **Params:** `sender: object`, `e: InkOverlayStrokesDeletingEventArgs`.
- **Returns:** `void`.

### `IC_Stroke(object sender, InkCollectorStrokeEventArgs e)` (L2500-L2874)
- **Does:** Main stroke completion handler; records undo, applies tool-specific logic, and refreshes display.
- **Params:** `sender: object`, `e: InkCollectorStrokeEventArgs`.
- **Returns:** `void`.

### `getEquiPointsFromStroke(Stroke stk, double dist, ref int Start, ref double Remain, int Xoff = 0, int Yoff = 0, bool ConvertInkSpaceToPixel = true)` (L2876-L2916)
- **Does:** Computes evenly spaced points along a stroke for patterning.
- **Params:** `stk: Stroke`, `dist: double`, `Start: ref int`, `Remain: ref double`, `Xoff: int`, `Yoff: int`, `ConvertInkSpaceToPixel: bool`.
- **Returns:** `List<Point>`.

### `ComputeTextBoxSize(ref Stroke st)` (L2919-L2953)
- **Does:** Computes and stores text bounding box size in stroke properties.
- **Params:** `st: ref Stroke`.
- **Returns:** `void`.

### `SaveUndoStrokes()` (L2955-L2974)
- **Does:** Stores the current ink state into the undo ring buffer.
- **Params:** None.
- **Returns:** `void`.

### `IC_CursorDown(object sender, InkCollectorCursorDownEventArgs e)` (L2978-L3075)
- **Does:** Handles stylus down events and initializes tool state.
- **Params:** `sender: object`, `e: InkCollectorCursorDownEventArgs`.
- **Returns:** `void`.

### `IC_MouseDown(object sender, CancelMouseEventArgs e)` (L3081-L3232)
- **Does:** Handles mouse-down interactions for drawing and selection tools.
- **Params:** `sender: object`, `e: CancelMouseEventArgs`.
- **Returns:** `void`.

### `IC_MouseMove(object sender, CancelMouseEventArgs e)` (L3238-L3449)
- **Does:** Handles drawing/dragging as the mouse moves.
- **Params:** `sender: object`, `e: CancelMouseEventArgs`.
- **Returns:** `void`.

### `IC_MouseUp(object sender, CancelMouseEventArgs e)` (L3451-L3548)
- **Does:** Finalizes drawing actions and updates state on mouse release.
- **Params:** `sender: object`, `e: CancelMouseEventArgs`.
- **Returns:** `void`.

### `IC_CursorInRange(object sender, InkCollectorCursorInRangeEventArgs e)` (L3550-L3577)
- **Does:** Handles cursor in-range events to update cursor state.
- **Params:** `sender: object`, `e: InkCollectorCursorInRangeEventArgs`.
- **Returns:** `void`.

### `MoveStrokeAndProperties(Stroke movedStroke, int DeltaX, int DeltaY, bool moveStroke = true)` (L3579-L3622)
- **Does:** Moves a stroke and synchronizes its metadata (text, image, pattern points).
- **Params:** `movedStroke: Stroke`, `DeltaX: int`, `DeltaY: int`, `moveStroke: bool`.
- **Returns:** `void`.
