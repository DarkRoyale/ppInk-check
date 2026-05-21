## src/FormCollection.cs (part 3/3)

### `FontBtn_Modify()` (L6832-L6844)
- **Does:** Opens text font modification flow.
- **Params:** None.
- **Returns:** `void`.

### `TagFontBtn_Modify()` (L6845-L6857)
- **Does:** Opens tag font modification flow.
- **Params:** None.
- **Returns:** `void`.

### `btTool_Click(object sender, EventArgs e)` (L6859-L7055)
- **Does:** Handles tool button clicks and updates tool selection.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `btEraser_Click(object sender, EventArgs e)` (L7057-L7066)
- **Does:** Enters eraser mode.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `btPan_Click(object sender, EventArgs e)` (L7069-L7096)
- **Does:** Activates pan/move tool selection.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `btScaleRot_Click(object sender, EventArgs e)` (L7098-L7121)
- **Does:** Activates scale/rotate tool.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `btMagn_Click(object sender, EventArgs e)` (L7124-L7137)
- **Does:** Activates magnet tool.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `btZoom_click(object sender, EventArgs e)` (L7146-L7188)
- **Does:** Toggles zoom tool mode and UI.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `StopAllZooms()` (L7190-L7207)
- **Does:** Stops any active zoom capture or display.
- **Params:** None.
- **Returns:** `void`.

### `StartZoomCapt()` (L7209-L7222)
- **Does:** Starts capturing the zoomed region.
- **Params:** None.
- **Returns:** `void`.

### `ActivateZoomDyn()` (L7224-L7232)
- **Does:** Activates dynamic zoom mode.
- **Params:** None.
- **Returns:** `void`.

### `ActivateSpot()` (L7234-L7239)
- **Does:** Activates spotlight mode.
- **Params:** None.
- **Returns:** `void`.

### `FormCollection_FormClosing(object sender, FormClosingEventArgs e)` (L7241-L7265)
- **Does:** Handles cleanup when the toolbar form closes.
- **Params:** `sender: object`, `e: FormClosingEventArgs`.
- **Returns:** `void`.

### `CustomizeAndOpenSubTools(int active, string title, string[] icons, string TextHintsStr, Func<int,bool>[] clickFuncts)` (L7279-L7341)
- **Does:** Configures and opens the sub-tools panel.
- **Params:** `active: int`, `title: string`, `icons: string[]`, `TextHintsStr: string`, `clickFuncts: Func<int,bool>[]`.
- **Returns:** `void`.

### `changeActiveTool(int active = -1, bool click = false, int visibility = 0)` (L7343-L7359)
- **Does:** Updates sub-tool activation state and visibility.
- **Params:** `active: int`, `click: bool`, `visibility: int`.
- **Returns:** `void`.

### `SubTool_Click(object sender, EventArgs e)` (L7361-L7379)
- **Does:** Handles clicks on sub-tool buttons.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `gpSubTools_MouseDown(object sender, MouseEventArgs e)` (L7381-L7386)
- **Does:** Handles mouse down for sub-tool dragging.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `gpSubTools_MouseMove(object sender, MouseEventArgs e)` (L7388-L7415)
- **Does:** Handles mouse move for sub-tool dragging.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `gpSubTools_MouseUp(object sender, MouseEventArgs e)` (L7417-L7420)
- **Does:** Handles mouse up for sub-tool dragging.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `Btn_SubToolClose_Click(object sender, EventArgs e)` (L7422-L7427)
- **Does:** Closes the sub-tools panel.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `BtnPin_Click(object sender, EventArgs e)` (L7429-L7444)
- **Does:** Pins/unpins the toolbar.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `RestorePolylineData(Stroke st)` (L7446-L7455)
- **Does:** Restores polyline metadata to a stroke after load/undo.
- **Params:** `st: Stroke`.
- **Returns:** `void`.

### `AllowInteractions(bool enter)` (L7457-L7476)
- **Does:** Temporarily disables click-through to allow dialogs.
- **Params:** `enter: bool`.
- **Returns:** `void`.

### `SaveStrokes(string fn = "ppinkSav.txt")` (L7478-L7583)
- **Does:** Saves strokes and metadata to a text file.
- **Params:** `fn: string`.
- **Returns:** `void`.

### `TabletPropertyMetricUnitFromString(string s)` (L7586-L7604)
- **Does:** Parses a tablet metric unit enum from string.
- **Params:** `s: string`.
- **Returns:** `TabletPropertyMetricUnit`.

### `LoadStrokes(string fn = "ppinkSav.txt")` (L7606-L7791)
- **Does:** Loads strokes and metadata from a text file.
- **Params:** `fn: string`.
- **Returns:** `void`.

### `btLoad_Click(object sender, EventArgs e)` (L7795-L7836)
- **Does:** Handles load button click (opens load dialog).
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `btLasso_Click(object sender, EventArgs e)` (L7838-L7855)
- **Does:** Toggles lasso selection mode.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `btSave_Click(object sender, EventArgs e)` (L7857-L7910)
- **Does:** Handles save button click (opens save dialog).
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `IsInside(Stroke lasso, float percent = 0)` (L7912-L7924)
- **Does:** Computes which strokes fall inside a lasso stroke.
- **Params:** `lasso: Stroke`, `percent: float`.
- **Returns:** `Strokes`.

### `ModifyStrokesSelection()` (L7926-L7929)
- **Does:** Refreshes the selection state based on the current lasso.
- **Params:** None.
- **Returns:** `void`.

### `ModifyStrokesSelection(bool AppendToSelection, ref Strokes InprogressSelection, Strokes StrokesSelection)` (L7931-L7946)
- **Does:** Updates selection set with append/remove behavior.
- **Params:** `AppendToSelection: bool`, `InprogressSelection: ref Strokes`, `StrokesSelection: Strokes`.
- **Returns:** `void`.

### `GetMainModuleFileName(Process process, int buffer = 1024)` (L7949-L7964)
- **Does:** Retrieves the main module path for a process.
- **Params:** `process: Process`, `buffer: int`.
- **Returns:** `string`.

### `AddM3UEntry(string st = null)` (L7967-L8034)
- **Does:** Adds an index entry to the M3U file when recording.
- **Params:** `st: string`.
- **Returns:** `bool`.

### `GetCaptionOfActiveWindow()` (L8037-L8052)
- **Does:** Retrieves the title of the current foreground window.
- **Params:** None.
- **Returns:** `string`.

### `SetWindowPos(IntPtr hWnd, IntPtr hWndInsertAfter, int X, int Y, int cx, int cy, uint uFlags)` (L8056)
- **Does:** P/Invoke to position a window.
- **Params:** `hWnd: IntPtr`, `hWndInsertAfter: IntPtr`, `X,Y,cx,cy: int`, `uFlags: uint`.
- **Returns:** `bool`.

### `GetWindowLong(IntPtr hWnd, int nIndex)` (L8058)
- **Does:** P/Invoke to read window style flags.
- **Params:** `hWnd: IntPtr`, `nIndex: int`.
- **Returns:** `uint`.

### `SetWindowLong(IntPtr hWnd, int nIndex, uint dwNewLong)` (L8060)
- **Does:** P/Invoke to set window style flags.
- **Params:** `hWnd: IntPtr`, `nIndex: int`, `dwNewLong: uint`.
- **Returns:** `int`.

### `btPagePrev_Click(object sender, EventArgs e)` (L8062-L8101)
- **Does:** Moves to the previous page of strokes.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `btPageNext_Click(object sender, EventArgs e)` (L8103-L8147)
- **Does:** Moves to the next page of strokes.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `SetLayeredWindowAttributes(IntPtr hwnd, uint crKey, byte bAlpha, uint dwFlags)` (L8150)
- **Does:** P/Invoke to set window transparency attributes.
- **Params:** `hwnd: IntPtr`, `crKey: uint`, `bAlpha: byte`, `dwFlags: uint`.
- **Returns:** `bool`.

### `GetDesktopWindow()` (L8152)
- **Does:** P/Invoke to get desktop window handle.
- **Params:** None.
- **Returns:** `IntPtr`.

### `GetKeyState(int keyCode)` (L8154)
- **Does:** P/Invoke to get key state.
- **Params:** `keyCode: int`.
- **Returns:** `short`.

### `GetDeviceCaps(IntPtr hdc, int nIndex)` (L8157)
- **Does:** P/Invoke to query device capabilities.
- **Params:** `hdc: IntPtr`, `nIndex: int`.
- **Returns:** `int`.

### `GetDC(IntPtr hWnd)` (L8159)
- **Does:** P/Invoke to get device context.
- **Params:** `hWnd: IntPtr`.
- **Returns:** `IntPtr`.

### `ReleaseDC(IntPtr hWnd, IntPtr hDC)` (L8161)
- **Does:** P/Invoke to release a device context.
- **Params:** `hWnd: IntPtr`, `hDC: IntPtr`.
- **Returns:** `bool`.

### `ShowWindow(int hWnd, int nCmdShow)` (L8163)
- **Does:** P/Invoke to show or hide a window.
- **Params:** `hWnd: int`, `nCmdShow: int`.
- **Returns:** `bool`.

### `GetKeyboardState(byte[] lpKeyState)` (L8167)
- **Does:** P/Invoke to get current keyboard state array.
- **Params:** `lpKeyState: byte[]`.
- **Returns:** `bool`.

### `GetAsyncKeyState(int vKey)` (L8169)
- **Does:** P/Invoke to get async key state.
- **Params:** `vKey: int`.
- **Returns:** `short`.

### `GetForegroundWindow()` (L8172)
- **Does:** P/Invoke to get active window handle.
- **Params:** None.
- **Returns:** `IntPtr`.

### `GetWindowText(IntPtr hWnd, StringBuilder text, int count)` (L8174)
- **Does:** P/Invoke to get window title text.
- **Params:** `hWnd: IntPtr`, `text: StringBuilder`, `count: int`.
- **Returns:** `int`.

### `GetWindowTextLength(IntPtr hWnd)` (L8176)
- **Does:** P/Invoke to get window title length.
- **Params:** `hWnd: IntPtr`.
- **Returns:** `int`.

### `GetWindowThreadProcessId(IntPtr hWnd, out uint ProcessId)` (L8178)
- **Does:** P/Invoke to get owning process ID for a window.
- **Params:** `hWnd: IntPtr`, `ProcessId: out uint`.
- **Returns:** `IntPtr`.

### `QueryFullProcessImageName(IntPtr hProcess, uint dwFlags, StringBuilder lpExeName, ref uint lpdwSize)` (L8180)
- **Does:** P/Invoke to fetch a process image path.
- **Params:** `hProcess: IntPtr`, `dwFlags: uint`, `lpExeName: StringBuilder`, `lpdwSize: ref uint`.
- **Returns:** `bool`.
