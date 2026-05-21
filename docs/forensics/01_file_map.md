## File Map

> Note: Binary assets (icons, PNGs, DLLs) are omitted. Generated WinForms designer code is marked as **[GENERATED]** and is not deep-analyzed.

| Path | Type | Purpose | Lines |
|------|------|---------|-------|
| `src/Program.cs` | Entry | App bootstrap, config folder setup, global exception handling | 338 |
| `src/Root.cs` | Core | Central state, configuration, and tool logic | 2971 |
| `src/FormCollection.cs` | UI | Main toolbar/interaction layer and stroke management | 8183 |
| `src/FormDisplay.cs` | UI | Drawing surface rendering and snapshot handling | 1592 |
| `src/FormOptions.cs` | UI | Options dialog and settings editing | 1612 |
| `src/FormInput.cs` | UI | Text input dialog for text/number tools | 239 |
| `src/FormAbout.cs` | UI | About dialog | 41 |
| `src/FormButtonHitter.cs` | UI | Helper form for click targeting | 129 |
| `src/CallForm.cs` | UI | Main host form wiring root + display | 85 |
| `src/PenModifyDlg.cs` | UI | Pen configuration dialog | 278 |
| `src/ArrowSelDlg.cs` | UI | Arrow head selection dialog | 231 |
| `src/ColorPickerDlg.cs` | UI | Color picker wrapper dialog | 19 |
| `src/ImageLister.cs` | UI | Clipart/image selector dialog | 312 |
| `src/zoomForm.cs` | UI | Zoom tool window | 20 |
| `src/Hotkey.cs` | Input | Global hotkey registration and parsing | 127 |
| `src/HotkeyInputBox.cs` | Input | Hotkey input control UI | 173 |
| `src/APIRest.cs` | API | REST listener for remote control | 1115 |
| `src/TinyJson.cs` | Util | JSON parsing/serialization helper | 381 |
| `src/Local.cs` | I18N | Localization loader/lookup | 425 |
| `src/Apng/APngImage.cs` | Media | APNG loading/decoding | 289 |
| `src/Apng/Chunks/Chunk.cs` | Media | APNG chunk base type | 110 |
| `src/Apng/Chunks/CodedChunks.cs` | Media | APNG chunk types | 290 |
| `src/Apng/Frame.cs` | Media | APNG frame utilities | 125 |
| `src/Apng/Helper.cs` | Media | APNG CRC/IO helpers | 159 |
| `src/Apng/StreamExtensions.cs` | Media | Stream extension helpers | 223 |
| `src/BuildTimestamp.cs` | Build | Build-time timestamp constant | 1 |
| `src/ToDoList.cs` | [EMPTY] | Placeholder file | 0 |
| `src/Properties/AssemblyInfo.cs` | Metadata | Assembly metadata | 39 |
| `src/Properties/Resources.Designer.cs` | [GENERATED] | Resource designer accessors | 1502 |
| `src/Properties/Settings.Designer.cs` | [GENERATED] | Settings designer accessors | 26 |
| `src/CallForm.Designer.cs` | [GENERATED] | WinForms designer code | 78 |
| `src/FormAbout.Designer.cs` | [GENERATED] | WinForms designer code | 67 |
| `src/FormButtonHitter.Designer.cs` | [GENERATED] | WinForms designer code | 65 |
| `src/FormCollection.Designer.cs` | [GENERATED] | WinForms designer code | 1213 |
| `src/FormDisplay.Designer.cs` | [GENERATED] | WinForms designer code | 75 |
| `src/FormInput.Designer.cs` | [GENERATED] | WinForms designer code | 191 |
| `src/FormOptions.Designer.cs` | [GENERATED] | WinForms designer code | 3427 |
| `src/HotkeyInputBox.Designer.cs` | [GENERATED] | WinForms designer code | 38 |
| `src/ImageLister.Designer.cs` | [GENERATED] | WinForms designer code | 204 |
| `src/PenModifyDlg.Designer.cs` | [GENERATED] | WinForms designer code | 472 |
| `src/ArrowSelDlg.Designer.cs` | [GENERATED] | WinForms designer code | 237 |
| `src/ColorPickerDlg.Designer.cs` | [GENERATED] | WinForms designer code | 188 |
| `src/zoomForm.Designer.cs` | [GENERATED] | WinForms designer code | 109 |
| `src/ArrowSelDlg.resx` | Resource | Dialog resources | 119 |
| `src/FormAbout.resx` | Resource | Dialog resources | 119 |
| `src/FormButtonHitter.resx` | Resource | Dialog resources | 122 |
| `src/FormCollection.resx` | Resource | Main toolbar resources | 3327 |
| `src/FormDisplay.resx` | Resource | Display resources | 3321 |
| `src/FormInput.resx` | Resource | Input dialog resources | 122 |
| `src/FormOptions.resx` | Resource | Options dialog resources | 4250 |
| `src/HotkeyInputBox.resx` | Resource | Hotkey input resources | 125 |
| `src/ImageLister.resx` | Resource | Image list resources | 125 |
| `src/PenModifyDlg.resx` | Resource | Pen dialog resources | 122 |
| `src/Root.resx` | Resource | Root form resources | 119 |
| `src/CallForm.resx` | Resource | Call form resources | 3318 |
| `src/zoomForm.resx` | Resource | Zoom form resources | 119 |
| `src/Properties/Resources.resx` | Resource | Global resources | 546 |
| `src/App.config` | Config | App-level configuration | 31 |
| `src/defaults.ini` | Config | Default settings template | 272 |
| `src/pensdef.ini` | Config | Default pen definitions | 200 |
| `ppInk/config.ini` | Data | User configuration (persisted) | 296 |
| `ppInk/config_default.ini` | Data | Default config snapshot | 66 |
| `ppInk/hotkeys.ini` | Data | Hotkey definitions (persisted) | 69 |
| `ppInk/pens.ini` | Data | Pen definitions (persisted) | 200 |
| `ppInk/defaults.ini` | Data | Default settings copy | 259 |
| `ppInk/pensdef.ini` | Data | Default pen definitions copy | 200 |
| `ppInk/ppInk.exe.config` | Config | Runtime config for built exe | 31 |
| `ppInk/httpRequests.md` | Docs | REST API request examples | 314 |
| `ppInk/install_microsoft_ink_dll.bat` | Script | Restores Microsoft.Ink DLL version | 5 |
