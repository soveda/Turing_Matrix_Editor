# Turing Matrix Editor

Standalone Web MIDI editor for the **Turing Matrix** Workshop Computer card.

This editor configures the card's saved settings in the browser. It does not replace the
front-panel controls.

## What it edits

- Turing layer settings
  - scale
  - octave range
  - pulse length mode
  - channel 2 loop offset
  - pulse output mode
  - CV output range
- Mixer layer settings
  - mix curve
  - lane link
  - rise
  - fall
  - lane 1 low/high
  - lane 2 low/high

## Using it

1. Open the HTTPS-hosted editor in desktop Chrome or Edge.
2. Connect the card.
3. Read the current settings from the card.
4. Change the settings in the form.
5. Send the settings back to the card.

## Notes

- Desktop Chrome or Edge is required. Web MIDI/SysEx is not supported reliably on iOS or Safari.
- Android MIDI support varies by device, cable/OTG adapter, and hub. Connect the card before opening the page and use a powered hub if detection is unreliable.
- The editor remembers only the selected colour theme. Settings remain local until **Send To Card** is pressed; the card stores successfully sent settings.
- **Load Defaults** changes the form locally and never overwrites the card until **Send To Card** is pressed.
- Open **Developer diagnostics** to inspect input/output ports and recent MIDI events after a failure. It is hidden during normal use and its log can be cleared.
- `Z middle` is the Turing layer.
- `Z up` is the mixer layer.
- `Z down` remains tap tempo.

## Attribution

The Turing Matrix editor and card build on ideas and code from **Tom Whitwell** and
**Chris Johnson**.

## Hosting

The editor is available at:

`https://soveda.github.io/Turing_Matrix_Editor/web`

## Files

- `web/index.html`
- `web/app.js`
- `web/styles.css`
