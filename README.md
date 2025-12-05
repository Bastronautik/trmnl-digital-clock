# Digital Clock Plugin

A retro-style digital clock plugin for TRMNL that recreates the nostalgic look of 80's/90's digital clocks with customizable display options.

## Overview

This plugin displays the current time and date in a classic 14-segment LED display style. It automatically syncs with your TRMNL device's timezone and offers multiple customization options for time format, date format, and visual theme.

## Features

- **Retro 14-segment LED display** - Authentic digital clock aesthetic
- **Timezone support** - Automatically uses your TRMNL user timezone
- **Multiple time formats** - Choose between 24-hour or 12-hour (AM/PM) format
- **Date format options** - US or European date formatting
- **Color themes** - Dark or light mode display
- **Optional location display** - Show your location name on the clock

## Settings

### Location
- **Type:** Text input (optional)
- **Description:** Enter your location name (e.g., "Amsterdam", "New York")
- **Default:** Empty

### Time Format
- **Type:** Dropdown
- **Options:**
  - 24-hour format
  - 12-hour (AM/PM) format
- **Default:** 24-hour

### Date Format
- **Type:** Dropdown
- **Options:**
  - DD MMM YYYY (European format)
  - MMM DD, YYYY (US format)
- **Default:** DD MMM YYYY (European)

### Color Mode
- **Type:** Dropdown
- **Options:**
  - Dark - White digits on dark background
  - Light - Black digits on light background
- **Default:** Dark

## Technical Details

- **Strategy:** Static
- **Refresh Interval:** 15 minutes
- **Screen Padding:** Yes
- **Dark Mode Support:** No (uses custom color mode setting instead)

## How It Works

The plugin uses JavaScript to render each digit using SVG paths that simulate a 14-segment display. The time is calculated based on your TRMNL user's UTC offset to ensure accurate local time display. The clock updates every 15 minutes to keep your display fresh while minimizing battery usage.

## Layout Support

This plugin supports all TRMNL layout sizes:
- Full screen
- Half horizontal
- Half vertical
- Quadrant
