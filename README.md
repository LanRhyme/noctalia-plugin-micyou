# noctalia-plugin-micyou

MicYou control and audio level monitor plugin for Noctalia 5

## Features

- Background headless daemon management for `micyou` CLI
- Real-time dynamic volume ring replicated from Tauri AudioRing with smooth lerp interpolation
- Native attached interactive control panel
  - Switch connection mode between Wi-Fi, USB (ADB), and Web
  - Gain slider adjustment (0 to 30 dB)
  - AI Noise Suppression toggle (PureVox)
  - Quick launch buttons for TUI and Desktop GUI
- Quick toggle shortcut card for Noctalia Control Center
- Automatic Morandi theme color synchronization

## Installation

Clone or link this repository to your Noctalia plugins directory:

```bash
git clone https://github.com/LanRhyme/noctalia-plugin-micyou ~/.config/noctalia/plugins/micyou
```

Enable the plugin in `~/.config/noctalia/settings.toml`:

```toml
[plugins]
enabled = [
  "lanrhyme/micyou"
]
```

Add the widget to your bar configuration in `~/.config/noctalia/settings.toml`:

```toml
[bar]
widgets = [
  "lanrhyme/micyou:widget"
]
```

## Gestures

- Left Click: Toggle attached control panel
- Right Click: Toggle service start or stop
- Middle Click: Launch TUI terminal console

## License

MIT License
