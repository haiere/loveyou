# A Message For You

A single-page romantic web experience by **Haiere** that delivers a personalized animated message with soft glassmorphism visuals, floating hearts, and optional calm instrumental background music.

![Preview](https://i.postimg.cc/8PJ0bhb1/H-haiere.webp)

## Overview

**A Message For You** is a lightweight, self-contained web app built with HTML, CSS, and vanilla JavaScript.  
It lets the user enter a name, then reveals a cinematic message sequence: **I → Love → You → [Name]** with smooth transitions and a polished visual style.

It is suitable for:
- Personal gifts and surprise messages.
- Learning modern CSS animation and UI effects.
- Prototyping single-page interactive experiences.
- Demonstrating accessible front-end patterns.

## Features

- Personalized message flow with name input.
- Smooth word-by-word animation sequence.
- Glassmorphism-inspired interface.
- Floating particles and twinkling stars.
- Animated hearts during the message reveal.
- Optional background audio with mute toggle.
- Keyboard support with Escape navigation.
- Responsive layout for mobile and desktop.
- Accessibility-friendly markup and motion preferences.

## Requirements

The project runs entirely in a browser.

| Requirement | Details |
|---|---|
| Operating system | Any modern OS |
| Browser | Chrome, Firefox, Safari, Edge |
| JavaScript | Enabled |
| Audio | Optional, HTML5 Audio supported |

## Quick Start

1. Open `index.html` in a modern browser.
2. Enter your name.
3. Click **Start**.
4. Watch the animated sequence.
5. Use **Play again** or **Change name** on the final screen.

## Installation

### Direct use
Download the `index.html` file and open it in your browser.

### Clone the repository:

```bash
git clone https://github.com/haiere/loveyou
cd loveyou
open index.html
``` 

No build step is required.

## Usage

### Basic flow
1. **Intro screen** — Enter a name with at least 2 characters.
2. **Animation screen** — The words appear one by one with visual effects.
3. **Final screen** — The personalized message is shown with action buttons.

### Audio controls
- The mute button is located in the top-right corner.
- Audio starts muted by default.
- Audio will attempt to play after user interaction.

### Keyboard shortcuts
- **Escape** — Removes focus from the input on the intro screen.
- **Escape** — Goes to **Change name** on the final screen.

## Configuration

You can customize the behavior in the JavaScript config object:

```javascript
const CONFIG = {
    AUDIO_URL: 'https://files.catbox.moe/j0r70l.mp3',
    VOLUME: 0.35,
    HEART_INTERVAL_MS: 700,
    HEART_LIFETIME_MS: 12000,
    WORD_HOLD_MS: 1700,
    WORD_GAP_MS: 350,
    TRANSITION_DELAY_MS: 800,
    NAME_MIN_LENGTH: 2,
};
```

| Setting | Description |
|---|---|
| `AUDIO_URL` | Direct link to the background music file. |
| `VOLUME` | Music volume from `0.0` to `1.0`. |
| `HEART_INTERVAL_MS` | Interval between floating heart spawns. |
| `HEART_LIFETIME_MS` | Time before a heart disappears. |
| `WORD_HOLD_MS` | Duration each word stays visible. |
| `WORD_GAP_MS` | Delay between word transitions. |
| `TRANSITION_DELAY_MS` | Screen fade timing. |
| `NAME_MIN_LENGTH` | Minimum name length allowed. |

## Project Structure

```txt
index.html
```

The entire project is contained in a single HTML file with embedded CSS and JavaScript.

## Supported Platforms

- Desktop: Chrome, Firefox, Safari, Edge.
- Mobile: Safari on iOS, Chrome on Android, Samsung Internet.
- Touch-friendly and responsive on smaller screens.

## Troubleshooting

### Audio does not play
- Most browsers require a user gesture before audio can start.
- Click the mute button or interact with the page.
- Make sure the audio URL is reachable.

### Animations feel slow
- Reduce particle or heart counts.
- Enable hardware acceleration in the browser.
- Use reduced motion settings if needed.

### Input validation fails
- The name must contain at least 2 characters.
- Leading and trailing spaces are trimmed automatically.

### Screen transitions get stuck
- Refresh the page and try again.
- Check the browser console for JavaScript errors.

## Security and Privacy

- No user data is collected or stored.
- Everything runs client-side in the browser.
- No cookies, analytics, or tracking scripts are included.
- The optional audio file is the only external resource.

## Performance Notes

- Single-file architecture reduces requests.
- Animations use `transform` and `opacity` for smoother rendering.
- Particle and heart counts are intentionally limited.
- Reduced-motion support lowers CPU and GPU usage.

## Development

To edit the project:
1. Open `index.html` in a text editor.
2. Modify HTML, CSS, or JavaScript.
3. Save the file.
4. Refresh the browser.

No special development environment is required.

## Testing

Recommended manual tests:
- Validate empty, short, and valid input.
- Test audio mute and unmute.
- Test transitions between all screens.
- Test on desktop and mobile sizes.
- Test with reduced motion enabled.
- Test the Escape key behavior.

## Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Make your changes.
4. Submit a pull request.

Please keep the single-file structure and accessibility support intact.

## Build and Release

No build process is required.

1. Verify the latest changes.
2. Test in multiple browsers.
3. Commit and tag the release.
4. Deploy the `index.html` file to a static host.

## License

This application is provided as open source. See the `LICENSE` file for details. 

## Author

Created by **Haiere & HajirStudio** as a personal greeting tool.

## Support

For questions, issues, or suggestions, open an issue in the repository.