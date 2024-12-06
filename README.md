[Ashot](ashot.png)

Ashot is a wrapper script for capturing screenshots in Hyprland.
It offers various modes for taking screenshots and allows you to save them or copy them to your clipboard.

## Features

- Capture full screen, active window, specific area, or custom screenshots.
- Save images in PNG, JPEG, or PPM formats.
- Configure screenshot quality and scaling.
- Optionally capture mouse cursors.
- Simple configuration via a dedicated config file.

## Prerequisites

Ensure you have the following packages installed:

- **grim**: For taking screenshots.
- **slurp**: For selecting screen areas.
- **wl-copy**: For copying screenshots to clipboard.
- **jq**: For parsing JSON from Hyprland commands.

## Configuration

| Option                    | Description                                                 |
|----------------------------|------------------------------------------------------------|
| `SCREENSHOT_DIR`           | Directory where screenshots will be saved.                 |
| `SCREENSHOT_MASK`          | Filename format for screenshots (timestamp-based).         |
| `SCREENSHOT_FORMAT`        | Format of the screenshots (options: `png`, `ppm`, `jpeg`). |
| `SCREENSHOT_QUALITY`       | Quality of the screenshot (0-100 percent).                 |
| `SCREENSHOT_COMPRESSION`   | Compression level for the image (0-9).                     |
| `SCREENSHOT_SCALE`         | Scaling factor for the screenshot.                         |
| `SCREENSHOT_CURSORS`       | Whether to capture mouse cursors (`true` or `false`).      |

## Installation

```sh
git clone https://github.com/yourusername/ashot.git
cd ashot
chmod +x ashot
cp ashot ~/.local/bin/
cp config ~/.config/ashot
```


