## src/FormOptions.cs (part 2/2)

### `ZoomScaleEd_Validating(object sender, CancelEventArgs e)` (L1165-L1171)
- **Does:** Validates zoom scale input.
- **Params:** `sender: object`, `e: CancelEventArgs`.
- **Returns:** `void`.

### `ZoomContinousCb_CheckedChanged(object sender, EventArgs e)` (L1173-L1176)
- **Does:** Toggles continuous zoom.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ZoomEnabledCb_SelectedIndexChanged(object sender, EventArgs e)` (L1178-L1181)
- **Does:** Toggles zoom enablement.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `hiGlobal_Enter(object sender, EventArgs e)` (L1183-L1186)
- **Does:** Focus handler for hotkey controls.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `hiGlobal_Leave(object sender, EventArgs e)` (L1188-L1191)
- **Does:** Blur handler for hotkey controls.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `FormOptions_Leave(object sender, EventArgs e)` (L1193-L1195)
- **Does:** Handles dialog focus loss.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `cbAllowHotkeyInPointer_CheckedChanged(object sender, EventArgs e)` (L1197-L1200)
- **Does:** Toggles hotkey handling while in pointer mode.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `hi_OnHotkeyChanged(object sender, EventArgs e)` (L1202-L1226)
- **Does:** Updates hotkey bindings from UI.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `comboLanguage_SelectedIndexChanged(object sender, EventArgs e)` (L1228-L1243)
- **Does:** Switches language selection.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `InverseWheelCb_CheckedChanged(object sender, EventArgs e)` (L1245-L1249)
- **Does:** Toggles mouse wheel inversion.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `SnapInPointerKeysChanged(object sender, EventArgs e)` (L1251-L1257)
- **Does:** Updates pointer snapshot key configuration.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `SubToolsBar_cb_CheckedChanged(object sender, EventArgs e)` (L1259-L1262)
- **Does:** Toggles sub-tools bar visibility.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `FormOptions_FormClosed(object sender, FormClosedEventArgs e)` (L1264-L1267)
- **Does:** Handles cleanup when options dialog closes.
- **Params:** `sender: object`, `e: FormClosedEventArgs`.
- **Returns:** `void`.

### `ActivateDbgWinBtn_Click(object sender, EventArgs e)` (L1269-L1273)
- **Does:** Activates debug window display.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `APIRestEd_Validating(object sender, CancelEventArgs e)` (L1275-L1289)
- **Does:** Validates REST API address input.
- **Params:** `sender: object`, `e: CancelEventArgs`.
- **Returns:** `void`.

### `APIRestEd_KeyPress(object sender, KeyPressEventArgs e)` (L1291-L1299)
- **Does:** Handles key press in REST API field.
- **Params:** `sender: object`, `e: KeyPressEventArgs`.
- **Returns:** `void`.

### `FitToCurveEd_CheckedChanged(object sender, EventArgs e)` (L1301-L1304)
- **Does:** Toggles FitToCurve for strokes.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `CaptStrokesOnlyCb_CheckedChanged(object sender, EventArgs e)` (L1306-L1309)
- **Does:** Toggles stroke-only snapshots.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `PensOnTwoLinesCb_CheckedChanged(object sender, EventArgs e)` (L1311-L1314)
- **Does:** Toggles two-line pen display.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `MeasureEnabledCb_CheckedChanged(object sender, EventArgs e)` (L1316-L1322)
- **Does:** Toggles measure tool enablement.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `Measure2ScaleEd_Validated(object sender, EventArgs e)` (L1324-L1327)
- **Does:** Validates measurement scale input.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `Measure2DigEd_Validated(object sender, EventArgs e)` (L1329-L1332)
- **Does:** Validates measurement digits input.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `Measure2DigEd_Validating(object sender, CancelEventArgs e)` (L1334-L1345)
- **Does:** Validates measurement digits on edit.
- **Params:** `sender: object`, `e: CancelEventArgs`.
- **Returns:** `void`.

### `Measure2UnitEd_TextChanged(object sender, EventArgs e)` (L1347-L1350)
- **Does:** Updates measurement unit text.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `MeasureAngleCb_CheckedChanged(object sender, EventArgs e)` (L1352-L1355)
- **Does:** Toggles angle measurement display.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ColorPickerEnaCb_CheckedChanged(object sender, EventArgs e)` (L1357-L1360)
- **Does:** Toggles color picker tool availability.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `comboPensLineStyle_Changed(object sender, EventArgs e)` (L1362-L1372)
- **Does:** Updates line style option for pens.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `SwapSnapBehaviorsCb_CheckedChanged(object sender, EventArgs e)` (L1374-L1377)
- **Does:** Toggles swap snapshot behavior.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `AltAsOneCommandCb_MouseClick(object sender, MouseEventArgs e)` (L1379-L1385)
- **Does:** Handles Alt-as-command option click.
- **Params:** `sender: object`, `e: MouseEventArgs`.
- **Returns:** `void`.

### `AltAsOneCommandCb_CheckStateChanged(object sender, EventArgs e)` (L1387-L1401)
- **Does:** Updates Alt-as-command option.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `AltAsOneCommandCb_MouseUp(object sender, EventArgs e)` (L1403-L1407)
- **Does:** Handles Alt-as-command mouse up events.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `CbHKRot_CheckedChanged(object sender, EventArgs e)` (L1409-L1420)
- **Does:** Toggles hotkey rotation option.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `Click4StrokeCb_CheckedChanged(object sender, EventArgs e)` (L1422-L1425)
- **Does:** Toggles click-to-stroke behavior.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `SpotColorPnl_Click(object sender, EventArgs e)` (L1427-L1443)
- **Does:** Sets spotlight color.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `SpotOnAltCb_CheckedChanged(object sender, EventArgs e)` (L1445-L1448)
- **Does:** Toggles spotlight on Alt key.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `SpotRadTb_Validated(object sender, EventArgs e)` (L1450-L1453)
- **Does:** Validates spotlight radius input.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `NewArrowEditBtn_Click(object sender, EventArgs e)` (L1455-L1459)
- **Does:** Opens arrow edit dialog.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `MagnetAngleEd_Validated(object sender, EventArgs e)` (L1461-L1465)
- **Does:** Validates magnetic angle input.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `IndexOnDockUndockCb_CheckedChanged(object sender, EventArgs e)` (L1468-L1471)
- **Does:** Toggles index creation on dock/undock.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `FfmegFileNameTxt_Validated(object sender, EventArgs e)` (L1473-L1476)
- **Does:** Validates FFmpeg filename template.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `IndexDefaultTxt_Validated(object sender, EventArgs e)` (L1478-L1481)
- **Does:** Validates index default file name.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `CreateM3u_CheckedChanged(object sender, EventArgs e)` (L1483-L1487)
- **Does:** Toggles M3U index creation.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `IndexDefaultTxt_TextChanged(object sender, EventArgs e)` (L1489-L1492)
- **Does:** Tracks index default text changes.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `UndockOnIndexCb_CheckedChanged(object sender, EventArgs e)` (L1494-L1497)
- **Does:** Toggles undock on index creation.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `NoEditM3Cb_CheckedChanged(object sender, EventArgs e)` (L1499-L1502)
- **Does:** Toggles M3U editing option.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `tbSnapFileTemplate_TextChanged(object sender, EventArgs e)` (L1504-L1516)
- **Does:** Updates snapshot filename template.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `tbSnapFileTemplate_Validating(object sender, CancelEventArgs e)` (L1518-L1530)
- **Does:** Validates snapshot filename template.
- **Params:** `sender: object`, `e: CancelEventArgs`.
- **Returns:** `void`.

### `tbSnapFileTemplate_Validated(object sender, EventArgs e)` (L1532-L1535)
- **Does:** Confirms snapshot filename template validation.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `tbSnapPath_TextChanged(object sender, EventArgs e)` (L1537-L1549)
- **Does:** Updates snapshot path text.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `StartFoldedCb_CheckedChanged(object sender, EventArgs e)` (L1551-L1554)
- **Does:** Toggles start-folded setting.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `KeepUnfoldedPointerCb_CheckedChanged(object sender, EventArgs e)` (L1556-L1559)
- **Does:** Toggles keep-unfolded in pointer mode.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `ExtraPensCb_CheckedChanged(object sender, EventArgs e)` (L1561-L1564)
- **Does:** Toggles extra pen set option.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.

### `VideoTabCtrl_Selecting(object sender, TabControlCancelEventArgs e)` (L1566-L1569)
- **Does:** Handles video tab selection validation.
- **Params:** `sender: object`, `e: TabControlCancelEventArgs`.
- **Returns:** `void`.

### `VideoTabCtrl_SelectedIndexChanged(object sender, EventArgs e)` (L1571-L1574)
- **Does:** Updates UI when the video tab changes.
- **Params:** `sender: object`, `e: EventArgs`.
- **Returns:** `void`.
