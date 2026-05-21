## src/Root.cs

### `ClipArtData.Clone()` (L73)
- **Does:** Returns a shallow copy of the clipart metadata structure.
- **Params:** None.
- **Returns:** `ClipArtData` — cloned instance.

### `TestMessageFilter.TestMessageFilter(Root root)` (L98-L101)
- **Does:** Stores the root reference for message filtering.
- **Params:** `root: Root` — application root instance.
- **Returns:** Constructor.

### `TestMessageFilter.PreFilterMessage(ref Message m)` (L103-L132)
- **Does:** Intercepts WM_HOTKEY and start-inking messages to trigger toolbar activation or index creation.
- **Params:** `m: Message` — Windows message.
- **Returns:** `bool` — true when handled.

### `Root.MinMagneticRadius()` (L345)
- **Does:** Computes the minimum magnetic radius based on configured value and constant minimum.
- **Params:** None.
- **Returns:** `int`.

### `Root.ExpandVarCmd(string cmd, int x, int y, int w, int h)` (L488-L509)
- **Does:** Expands environment variables and replaces snapshot/video placeholders in a command template.
- **Params:** `cmd: string` — template; `x,y,w,h: int` — coordinates/size values.
- **Returns:** `string` — expanded command string.

### `Root.IsVideoRecordingSelected()` (L511-L514)
- **Does:** Indicates whether video recording mode is active.
- **Params:** None.
- **Returns:** `bool`.

### `Root.Root()` (L517-L573)
- **Does:** Initializes defaults, loads configuration files, creates core forms and API server, and registers hotkeys.
- **Params:** None.
- **Returns:** Constructor.

### `Root.callshortcut()` (L575-L598)
- **Does:** Toggles inking based on current visibility, optionally entering snapshot mode.
- **Params:** None.
- **Returns:** `void`.

### `Root.TrayIcon_BalloonTipClicked(object sender, EventArgs e)` (L600-L615)
- **Does:** Opens Explorer to the last snapshot file when the tray balloon is clicked.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `Root.TrayIcon_Click(object sender, MouseEventArgs e)` (L617-L633)
- **Does:** Handles tray icon clicks to toggle drawing or dock state.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `Root.StartInk()` (L635-L681)
- **Does:** Creates and shows the drawing UI, initializes undo state, selects pen, and focuses the toolbar.
- **Params:** None.
- **Returns:** `void`.

### `Root.StopInk()` (L682-L746)
- **Does:** Hides drawing UI, cleans up OBS resources, and restores the call form when exiting ink mode.
- **Params:** None.
- **Returns:** `void`.

### `Root.ClearInk()` (L748-L754)
- **Does:** Deletes all strokes and redraws the display.
- **Params:** None.
- **Returns:** `void`.

### `Root.ShowBalloonSnapshot()` (L756-L759)
- **Does:** Shows the tray balloon notification for snapshots.
- **Params:** None.
- **Returns:** `void`.

### `Root.UndoInk()` (L761-L786)
- **Does:** Restores the previous stroke state from the undo ring buffer.
- **Params:** None.
- **Returns:** `void`.

### `Root.Pan(int x, int y)` (L788-L802)
- **Does:** Moves all strokes by a delta and refreshes the display.
- **Params:** `x: int`, `y: int` — delta offsets.
- **Returns:** `void`.

### `Root.SetInkVisible(bool visible)` (L804-L816)
- **Does:** Toggles ink visibility and updates toolbar icons/rendering.
- **Params:** `visible: bool`.
- **Returns:** `void`.

### `Root.RedoInk()` (L818-L836)
- **Does:** Restores a later stroke state from the redo buffer.
- **Params:** None.
- **Returns:** `void`.

### `Root.Dock()` (L838-L854)
- **Does:** Collapses/docks the toolbar and updates dock icon based on orientation.
- **Params:** None.
- **Returns:** `void`.

### `Root.UnDock()` (L856-L879)
- **Does:** Expands the toolbar and optionally adds an index entry on undock.
- **Params:** None.
- **Returns:** `void`.

### `Root.Pointer()` (L881-L899)
- **Does:** Enters pointer mode (click-through) and prepares the helper form.
- **Params:** None.
- **Returns:** `void`.

### `Root.UnPointer()` (L901-L918)
- **Does:** Exits pointer mode and restores input focus to the toolbar.
- **Params:** None.
- **Returns:** `void`.

### `Root.SelectPen(int pen)` (L920-L923)
- **Does:** Delegates pen selection to the toolbar form.
- **Params:** `pen: int` — pen index.
- **Returns:** `void`.

### `Root.SetDefaultPens()` (L925-L1006)
- **Does:** Creates default pen attributes and enables the default pen set.
- **Params:** None.
- **Returns:** `void`.

### `Root.SetDefaultConfig()` (L1008-L1022)
- **Does:** Initializes default hotkeys and snapshot paths.
- **Params:** None.
- **Returns:** `void`.

### `Root.SetTrayIconColor()` (L1024-L1040)
- **Does:** Chooses the tray icon color based on configuration and available files.
- **Params:** None.
- **Returns:** `void`.

### `Root.GetPenNumber(string sName)` (L1042-L1050)
- **Does:** Extracts a pen index from a `PENxx_` configuration key.
- **Params:** `sName: string` — config key name.
- **Returns:** `int` — pen index or -1.

### `Root.StringToColor(string colorStr)` (L1052-L1057)
- **Does:** Converts a color string into a `System.Drawing.Color`.
- **Params:** `colorStr: string`.
- **Returns:** `Color`.

### `Root.ReadOptions(string file)` (L1059-L1951)
- **Does:** Parses ini-style configuration files to populate pens, hotkeys, and runtime options.
- **Params:** `file: string` — config filename.
- **Returns:** `void`.

### `Root.FillImageStampFromConfig(string sPara, ref ClipArtData ImgStamp)` (L1953-L2004)
- **Does:** Parses clipart stamp settings and registers the image path.
- **Params:** `sPara: string` — serialized stamp data; `ImgStamp: ref ClipArtData` — output struct.
- **Returns:** `string` — resolved image path.

### `Root.Fill2Str(int i)` (L2006-L2014)
- **Does:** Converts a fill enum value to its config string.
- **Params:** `i: int` — fill value.
- **Returns:** `string`.

### `Root.SaveOptions(string file)` (L2016-L2682)
- **Does:** Writes current settings back into ini-style configuration files.
- **Params:** `file: string` — config filename.
- **Returns:** `void`.

### `Root.CompleteConfig(string NewConfig, string OldConfig)` (L2684-L2698)
- **Does:** Computes missing config entries to append when upgrading configs.
- **Params:** `NewConfig: string`, `OldConfig: string`.
- **Returns:** `string` — lines to append.

### `Root.OnAbout(object sender, EventArgs e)` (L2702-L2706)
- **Does:** Opens the About dialog.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `Root.OnOptions(object sender, EventArgs e)` (L2713-L2724)
- **Does:** Opens the Options dialog if drawing UI is not visible.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `Root.SetHotkey()` (L2726-L2745)
- **Does:** Registers the global hotkey and optional index hotkey with the OS.
- **Params:** None.
- **Returns:** `void`.

### `Root.UnsetHotkey()` (L2747-L2751)
- **Does:** Unregisters global hotkeys.
- **Params:** None.
- **Returns:** `void`.

### `Root.ChangeLanguage(string filename)` (L2753-L2762)
- **Does:** Loads a localization file and rebuilds tray menu text.
- **Params:** `filename: string` — language file path.
- **Returns:** `void`.

### `Root.OnExit(object sender, EventArgs e)` (L2764-L2770)
- **Does:** Unregisters hotkeys and exits the application.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `Root.HiMetricToPixel(double hi)` (L2772-L2782)
- **Does:** Converts HIMETRIC units to pixels with overflow guards.
- **Params:** `hi: double`.
- **Returns:** `int`.

### `Root.PixelToHiMetric(double pi)` (L2784-L2794)
- **Does:** Converts pixels to HIMETRIC units with overflow guards.
- **Params:** `pi: double`.
- **Returns:** `int`.

### `Root.MakeRelativePath(string fromPath, string toPath)` (L2796-L2815)
- **Does:** Builds a relative path between two filesystem paths.
- **Params:** `fromPath: string`, `toPath: string`.
- **Returns:** `string`.

### `Root.ConvertMeasureLength(double hl)` (L2818-L2821)
- **Does:** Converts a length using the configured measurement scale.
- **Params:** `hl: double`.
- **Returns:** `double`.

### `Root.LineStyleToString(ExtendedProperties props)` (L2823-L2842)
- **Does:** Maps extended properties to a line style string.
- **Params:** `props: ExtendedProperties`.
- **Returns:** `string`.

### `Root.LineStyleFromString(string s)` (L2844-L2862)
- **Does:** Parses a line style string to a `DashStyle`.
- **Params:** `s: string`.
- **Returns:** `DashStyle`.

### `Root.NextLineStyleString(string s, bool CustomList=false)` (L2864-L2899)
- **Does:** Rotates to the next enabled line style based on configuration.
- **Params:** `s: string` — current style; `CustomList: bool` — use configured enable mask.
- **Returns:** `string`.

### `Root.AppGetFocus()` (L2902-L2905)
- **Does:** Brings the application to foreground.
- **Params:** None.
- **Returns:** `void`.

### `Root.ContainsInsensitive(StringCollection Arr, string key)` (L2907-L2913)
- **Does:** Case-insensitive membership check for string collections.
- **Params:** `Arr: StringCollection`, `key: string`.
- **Returns:** `bool`.

### `Root.InputBox(string prompt="", string title="ppInk", string deflt="")` (L2915-L2961)
- **Does:** Displays a simple modal input dialog and returns user text.
- **Params:** `prompt: string`, `title: string`, `deflt: string`.
- **Returns:** `string`.

### `RegisterHotKey(IntPtr hwnd, int id, int fsModifiers, int vk)` (L2964)
- **Does:** P/Invoke for registering system hotkeys.
- **Params:** `hwnd: IntPtr`, `id: int`, `fsModifiers: int`, `vk: int`.
- **Returns:** `int`.

### `UnregisterHotKey(IntPtr hwnd, int id)` (L2966)
- **Does:** P/Invoke for unregistering system hotkeys.
- **Params:** `hwnd: IntPtr`, `id: int`.
- **Returns:** `int`.

### `SetForegroundWindow(IntPtr hWnd)` (L2968)
- **Does:** P/Invoke to bring a window to the foreground.
- **Params:** `hWnd: IntPtr`.
- **Returns:** `IntPtr`.
