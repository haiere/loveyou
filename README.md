A Message For You

A romantic animated greeting that displays a personalised message with elegant glass‑morphism design and subtle motion effects.

---

Overview

This single‑page HTML application presents a thoughtful, animated message for a special person. After entering a name, the user experiences a gentle word‑by‑word reveal—"I", "Love", "You", and finally the name itself—accompanied by floating hearts, soft particle effects, and a polished glass‑inspired interface.

The application is self‑contained, requires no backend, and runs entirely in the browser. It is designed to be used as a personal greeting, a surprise message, or a romantic gift.

---

Features

· Name‑based personalisation – Enter any name to receive a custom message.
· Animated word reveal – Words appear sequentially with smooth transitions and subtle blur effects.
· Glass‑morphism UI – Apple‑inspired liquid glass cards with backdrop blur, soft borders, and gentle highlights.
· Ambient background – Floating particles, twinkling stars, and drifting hearts create a dreamy atmosphere.
· Name glow effect – The final name is displayed with a soft glow and pulsing heart animation.
· Responsive design – Adapts to all screen sizes, from mobile phones to large displays.
· Accessibility – Supports reduced motion preferences, screen reader labels, and keyboard navigation.
· Privacy‑first – No data is stored or transmitted; the name is only used locally to generate the message.

---

Requirements

· A modern web browser with JavaScript enabled (Chrome, Firefox, Edge, Safari, or similar).
· An internet connection is required only to load the Google Fonts stylesheet (Poppins, Playfair Display, Cormorant Garamond). Once loaded, the fonts are cached by the browser.

---

Installation

The application is a single HTML file. To use it:

1. Open the hosted URL in your browser.
2. Alternatively, download the index.html file and open it locally.

No additional setup, server, or dependencies are required.

---

Usage

Step‑by‑step

1. Enter a name – Type any name into the input field on the intro screen.
2. Submit – Press the “Start” button or hit Enter.
3. Watch the animation – The words "I", "Love", "You", and then the name appear one by one with smooth transitions and subtle sparkle effects.
4. View the final message – The screen shows "I Love You, [name] ♥" with a pulsing heart.
5. Interact – Use the “Play again” button to replay the animation, or “Change name” to go back and enter a different name.

Keyboard shortcuts

· Enter – Submit the name on the intro screen.
· Escape – Blur the input field on the intro screen, or return to the intro screen from the final screen (triggers the “Change name” action).

---

Accessibility

· Reduced motion – The application respects the prefers-reduced-motion system setting. When enabled, animations are simplified or disabled.
· Reduced transparency – The application respects prefers-reduced-transparency by using solid backgrounds instead of glass effects.
· Screen reader support – Semantic HTML and ARIA attributes are used throughout. The animation screen includes aria-live="polite" to announce new words as they appear.
· Keyboard navigation – All interactive elements are reachable via keyboard, with visible focus indicators.
· Form validation – The name input includes real‑time validation with descriptive error messages.

---

Customisation

The application can be easily customised by modifying the CSS variables and JavaScript arrays in the source code.

Changing the message

To change the word sequence, locate the runWordSequence function in the JavaScript section. The current sequence is:

```javascript
await showWord('I', { duration: 1500 });
await showWord('Love', { accent: true, duration: 1600 });
await showWord('You', { accent: true, duration: 1600 });
await showWord(currentName, { isName: true, withGlowRing: true, duration: 2000 });
```

Replace or reorder the words as desired.

Adjusting colours

The colour palette is defined in the :root CSS variables:

```css
--c-pink: #ff8fb1;
--c-pink-soft: #ffc4d6;
--c-glow: #ff6f9c;
--c-maroon: #3a0f1f;
--c-black: #0a0509;
--c-purple: #1a0b2e;
```

Modify these values to match your preferred theme.

Animation timing

Each word’s display duration can be adjusted via the duration property (in milliseconds) passed to showWord. The gap between words is controlled by the gap variable in the runWordSequence function.

---

Privacy

The application is fully client‑side:

· No data is sent to any server.
· No cookies are used.
· No analytics or tracking scripts are included.
· The name you enter is only used to generate the final message and is never persisted or transmitted.

---

Troubleshooting

· Fonts not loading – Check your internet connection; the application relies on Google Fonts. If offline, consider hosting the font files locally.
· Animation does not start – Ensure JavaScript is enabled and that you have entered a valid name (at least 2 characters).
· Reduced motion mode active – If you have system‑level reduced motion enabled, animations will be minimal or disabled. This is intentional and respects user preferences.
· Name not displaying correctly – The input field accepts up to 40 characters. Very long names may wrap on smaller screens.

---

Development

The entire application is contained in a single index.html file. To modify or extend it:

· Edit the HTML structure directly.
· CSS custom properties and styles are located in the <style> block.
· JavaScript logic is at the bottom of the file, inside the <script> tag.

No build tools or compilation steps are required. Open the file in a browser to test changes.

---

License

This application is provided as open source. See the LICENSE file for details.

---

Author

Created by Haiere as a personal greeting tool.

---

Last updated: 2026

Berikut versi README.md yang sudah dirapikan, distrukturkan ulang, dan dibersihkan tanpa emoji. Saya juga menyesuaikan gaya penulisan agar konsisten dengan README proyek sebelumnya.

```md
# A Message For You

A romantic animated greeting that displays a personalised message with elegant glass-morphism design and subtle motion effects.

This single-page HTML application presents a thoughtful, animated message for a special person. After entering a name, the user experiences a gentle word-by-word reveal—"I", "Love", "You", and finally the name itself—accompanied by floating hearts, soft particle effects, and a polished glass-inspired interface.

The application is self-contained, requires no backend, and runs entirely in the browser. It is designed to be used as a personal greeting, a surprise message, or a romantic gift.

---

## Features

- Name-based personalisation — Enter any name to receive a custom message.
- Animated word reveal — Words appear sequentially with smooth transitions and subtle blur effects.
- Glass-morphism UI — Apple-inspired liquid glass cards with backdrop blur, soft borders, and gentle highlights.
- Ambient background — Floating particles, twinkling stars, and drifting hearts create a dreamy atmosphere.
- Name glow effect — The final name is displayed with a soft glow and pulsing heart animation.
- Responsive design — Adapts to all screen sizes, from mobile phones to large displays.
- Accessibility — Supports reduced motion preferences, screen reader labels, and keyboard navigation.
- Privacy-first — No data is stored or transmitted; the name is only used locally to generate the message.

---

## Requirements

- A modern web browser with JavaScript enabled (Chrome, Firefox, Edge, Safari, or similar).
- An internet connection is required only to load the Google Fonts stylesheet (Poppins, Playfair Display, Cormorant Garamond). Once loaded, the fonts are cached by the browser.

---

## Installation

The application is a single HTML file. To use it:

1. Open the hosted URL in your browser.
2. Alternatively, download the `index.html` file and open it locally.

No additional setup, server, or dependencies are required.

---

## Usage

### Step-by-step

1. Enter a name — Type any name into the input field on the intro screen.
2. Submit — Press the "Start" button or hit Enter.
3. Watch the animation — The words "I", "Love", "You", and then the name appear one by one with smooth transitions and subtle sparkle effects.
4. View the final message — The screen shows "I Love You, [name] ♥" with a pulsing heart.
5. Interact — Use the "Play again" button to replay the animation, or "Change name" to go back and enter a different name.

### Keyboard shortcuts

| Shortcut | Action |
|---|---|
| Enter | Submit the name on the intro screen |
| Escape | Blur the input field on the intro screen, or return to the intro screen from the final screen |

---

## Accessibility

- Reduced motion — The application respects the `prefers-reduced-motion` system setting. When enabled, animations are simplified or disabled.
- Reduced transparency — The application respects `prefers-reduced-transparency` by using solid backgrounds instead of glass effects.
- Screen reader support — Semantic HTML and ARIA attributes are used throughout. The animation screen includes `aria-live="polite"` to announce new words as they appear.
- Keyboard navigation — All interactive elements are reachable via keyboard, with visible focus indicators.
- Form validation — The name input includes real-time validation with descriptive error messages.

---

## Customisation

The application can be easily customised by modifying the CSS variables and JavaScript arrays in the source code.

### Changing the message

To change the word sequence, locate the `runWordSequence` function in the JavaScript section. The current sequence is:

```javascript
await showWord('I', { duration: 1500 });
await showWord('Love', { accent: true, duration: 1600 });
await showWord('You', { accent: true, duration: 1600 });
await showWord(currentName, { isName: true, withGlowRing: true, duration: 2000 });
```

Replace or reorder the words as desired.

### Adjusting colours

The colour palette is defined in the `:root` CSS variables:

```css
--c-pink: #ff8fb1;
--c-pink-soft: #ffc4d6;
--c-glow: #ff6f9c;
--c-maroon: #3a0f1f;
--c-black: #0a0509;
--c-purple: #1a0b2e;
```

Modify these values to match your preferred theme.

### Animation timing

Each word's display duration can be adjusted via the `duration` property (in milliseconds) passed to `showWord`. The gap between words is controlled by the `gap` variable in the `runWordSequence` function.

---

## Privacy

The application is fully client-side:

- No data is sent to any server.
- No cookies are used.
- No analytics or tracking scripts are included.
- The name you enter is only used to generate the final message and is never persisted or transmitted.

---

## Troubleshooting

### Fonts not loading

Check your internet connection; the application relies on Google Fonts. If offline, consider hosting the font files locally.

### Animation does not start

Ensure JavaScript is enabled and that you have entered a valid name (at least 2 characters).

### Reduced motion mode active

If you have system-level reduced motion enabled, animations will be minimal or disabled. This is intentional and respects user preferences.

### Name not displaying correctly

The input field accepts up to 40 characters. Very long names may wrap on smaller screens.

---

## Development

The entire application is contained in a single `index.html` file. To modify or extend it:

- Edit the HTML structure directly.
- CSS custom properties and styles are located in the `<style>` block.
- JavaScript logic is at the bottom of the file, inside the `<script>` tag.

No build tools or compilation steps are required. Open the file in a browser to test changes.

---

## License

This application is provided as open source. See the `LICENSE` file for details.

---

## Author

Created by Haiere as a personal greeting tool.

---

Last updated: 2026