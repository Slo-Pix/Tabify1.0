# Tabify

![Tabify](banner.png)

A guitar arrangement tool — web editor.

Write and edit guitar tablature with techniques, left/right hand finger notation, and printable export. No accounts, no frameworks, no dependencies.

## Web Editor

Open `editor.html` in a browser or visit the [hosted version](https://tabifyeditor.vercel.app).

- 16th-note grid editor with 6-string (guitar) and 4-string (ukulele) tablature
- Techniques: hammer-on, pull-off, slide, bend, vibrato, harmonics (natural + artificial)
- Finger notation: L.H. (1-2-3-4) and R.H. (P-I-M-A-C)
- Interactive fretboard with scale overlays — adapts to any tuning and string count, including custom
- Custom time signatures
- Export to printable HTML with metadata (key, BPM, time, tuning)
- File-based save/open using `.tbfy` format
- Undo/redo, copy/paste, section reordering
- 5 guitar + 3 ukulele tuning presets, plus fully custom tuning support (string count follows the notes you type)
- Built-in chromatic tuner — microphone pitch detection showing note, octave, and cents sharp/flat before you start arranging
- Installable PWA — works fully offline after the first visit
- Responsive UI — collapsible toolbar and dropdown docs navigation on mobile

### Keyboard Shortcuts

| Key | Action |
|-----|--------|
| Arrow keys | Move cursor |
| 0-9 | Enter fret number |
| Tab | Jump one beat |
| Escape | Close modals |
| Ctrl+Z | Undo |
| Ctrl+Shift+Z / Ctrl+Y | Redo |
| Ctrl+C | Copy measure |
| Ctrl+V | Paste measure |
| Ctrl+S | Save as .tbfy file |

## Tech Stack

- **Web**: Vanilla HTML, CSS, JavaScript — no frameworks, no build step
- **Format**: JSON-based `.tbfy` files
- **Offline**: Service worker precaches the app shell (`service-worker.js`)

## Documentation

See the full [documentation](https://tabifyeditor.vercel.app/docs.html) for detailed guides on the editor, keyboard shortcuts, supported tunings, and the `.tbfy` file format.

For a code-level walkthrough of every file and the main data flows, see [workflow.md](workflow.md).

## License

MIT
