# Project: ppInk

## Quick Stats
| Metric | Value |
|--------|-------|
| Language | C# (.NET Framework 4.8) (src/ppInk.csproj L8-L12) |
| Framework | Windows Forms + Microsoft.Ink (src/Program.cs L99-L105, src/Root.cs L5-L11) |
| Database | File-based INI/config storage (ppInk/config.ini, ppInk/hotkeys.ini, ppInk/pens.ini) |
| Architecture | Desktop monolith (single WinForms app) (src/Program.cs L99-L151) |
| Entry Point | `src/Program.cs` (L44-L153) |
| Source Files | 28 C# source files (excluding *.Designer.cs) |
| Lines of Code | ~19,507 C# LOC (excluding *.Designer.cs) |

## Purpose
ppInk is a Windows on-screen annotation tool for mouse, touchscreen, and pen input. It provides drawing tools (lines, shapes, arrows, text, cliparts, etc.) and is designed for presentations and screen capture workflows. (readme.md L18-L34)

## Key Dependencies
| Package | Version | Purpose |
|---------|---------|---------|
| GameOverlay.Net | 4.3.1 | Overlay rendering/timing support for WinForms drawing (src/packages.config L3) |
| SharpDX | 4.2.0 | DirectX interop for rendering/graphics (src/packages.config L4) |
| SharpDX.Direct2D1 | 4.2.0 | Direct2D rendering layer (src/packages.config L5) |
| SharpDX.DXGI | 4.2.0 | DXGI interop (src/packages.config L6) |

## Monorepo Packages
Not a monorepo (single solution `ppInk.sln`).
