## src/Program.cs

### `Main(string[] args)` (L44-L153)
- **Does:** Initializes culture and assembly loading, enforces single instance, resolves runtime folders, wires exception handlers, instantiates `CallForm`/`Root`, and starts the WinForms message loop.
- **Params:** `args: string[]` — command-line args (supports `-c` for config folder override).
- **Returns:** `void`.

### `PrepareConfigFolder(string programFolder, string runningFolder)` (L155-L193)
- **Does:** Ensures the running config folder is writable and copies non-binary assets into a writable folder when needed.
- **Params:** `programFolder: string` — base install folder; `runningFolder: string` — desired config folder.
- **Returns:** `string` — resolved running folder path.

### `UIThreadException(object sender, ThreadExceptionEventArgs t)` (L195-L227)
- **Does:** Logs UI thread exceptions, shows a crash dialog, and exits on fatal errors.
- **Params:** `sender: object` — event sender; `t: ThreadExceptionEventArgs` — exception payload.
- **Returns:** `void`.

### `UnhandledException(object sender, UnhandledExceptionEventArgs e)` (L229-L272)
- **Does:** Logs unhandled exceptions, displays a crash dialog, and attempts to write to the Windows event log.
- **Params:** `sender: object` — event sender; `e: UnhandledExceptionEventArgs` — exception payload.
- **Returns:** `void`.

### `EnsureSingleInstance()` (L274-L294)
- **Does:** Detects an existing ppInk process and signals it to start inking instead of launching another instance.
- **Params:** None.
- **Returns:** `bool` — true when no other instance is running.

### `ShowErrorDialog(string title, string errormsg)` (L297-L314)
- **Does:** Shows an error dialog and auto-saves strokes on exit confirmation.
- **Params:** `title: string` — dialog title; `errormsg: string` — error details.
- **Returns:** `DialogResult` — user response.

### `WriteErrorLog(string errormsg)` (L316-L336)
- **Does:** Appends crash details to `crash.txt` in the running folder.
- **Params:** `errormsg: string` — formatted error message.
- **Returns:** `void`.

## src/BuildTimestamp.cs

### `Build.Timestamp` (L1)
- **Does:** Build-time timestamp string constant used for crash logs and version info.
- **Type:** `string`.
