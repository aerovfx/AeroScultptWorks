ABrush 0.9.0 — Native 3D sculpting (100% Rust: winit + wgpu + egui)
===================================================================

Builds in this folder
----------------------
  ABrush.app          macOS 11+ Apple Silicon (arm64 / M1·M2·M3)
  windows/abrush.exe  Windows 10/11 64-bit (x86-64)

Both binaries are self-contained — every asset (matcaps, fonts, brush alphas,
Orb pack, HDR environments) is embedded at compile time. No installer, no
external files required.

macOS (Apple Silicon)
---------------------
  • Double-click ABrush.app, or from a terminal:  open ABrush.app
  • First launch: the build is only ad-hoc signed (no Apple Developer ID), so
    macOS Gatekeeper may say "unidentified developer". Right-click the app →
    Open → Open, or run once:
        xattr -dr com.apple.quarantine ABrush.app
  • Renders through Metal.

Windows (x86-64)
----------------
  • Double-click windows\abrush.exe (release build runs with no console window).
  • Renders through DX12 / Vulkan (falls back automatically).
  • SmartScreen may warn on an unsigned exe → "More info" → "Run anyway".
  • Cross-compiled from macOS with the mingw-w64 (GNU) toolchain; the mingw
    runtime is statically linked, so no extra DLLs are needed.

Quick controls
--------------
  • Left-drag on the mesh: sculpt with the active brush (bottom tool strip).
  • Left-drag on empty canvas: rotate.  Alt+drag: pan / zoom.
  • X: toggle X-symmetry.  Ctrl/Cmd+drag: mask.  Ctrl+Z / Ctrl+Shift+Z: undo/redo.
  • Tabs top-center: SCULPT / PAINT / MASK / RENDER.
  • Left rail: TOOL / SCENE / SUBTOOLS / FILTERS / CAMERA / HISTORY / SETTINGS.

CLI (either binary, for automation)
-----------------------------------
  abrush --ui-snapshot out.png [tool|scene|layers|camera|history|settings]
  abrush --render-pbr out.png [pbr|matcap|normal|uv|clay]
  abrush --render-beauty out.png [scale 1..8] [env_idx]
