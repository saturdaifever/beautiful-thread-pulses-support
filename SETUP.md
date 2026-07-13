# Beautiful Thread Pulses Setup Guide

Beautiful Thread Pulses adds live ChatGPT and Codex control to Stream Deck on macOS.

## Requirements

- macOS 12 or later.
- Stream Deck 7.1 or later.
- ChatGPT App for macOS with Codex access.
- A supported Stream Deck device or Stream Deck Mobile layout.

## Install

1. Install the `Beautiful Thread Pulses.streamDeckPlugin` file from Elgato Marketplace.
2. Restart Stream Deck if the plugin does not appear immediately.
3. Choose the bundled profile for your device, or add individual Beautiful Thread Pulses actions to an existing profile.
4. Open ChatGPT on the same macOS user account that runs Stream Deck.

The bundled profiles provide reviewed Work, Codex, voice, reasoning, approval, and review layouts. Start there before building a profile manually.

## The Five Action Types

- **Settings** — adjust the visual environment, including Ambient, LED Gain, and Neighbor Influence.
- **Shortcut Settings** — inspect the ChatGPT command catalog and the current keybinding status.
- **Audio Settings** — choose sounds, themes, volume, and reverb, or mute sound feedback.
- **Thread Visual** — show a recent thread and its live attention state; press it to return to that thread.
- **Custom Key** — run a detected ChatGPT or Codex command using a ready-made preset or a custom choice.

The bundled profiles may contain hidden helper actions required by the integration. The action list remains focused on the five types users need to configure directly.

## Shortcut Discovery

Beautiful Thread Pulses reads the command catalog and keybindings from the ChatGPT App installed on your Mac. It refreshes automatically when the app or its shortcut settings change.

A Custom Key can show four useful states:

- active — the command is ready;
- unbound — ChatGPT knows the command but no shortcut is assigned;
- disabled — the shortcut is disabled in ChatGPT;
- unavailable — the command is not present in the installed app version.

The plugin never rewrites ChatGPT shortcuts. If a command is unbound or disabled, edit it in ChatGPT and wait for the existing Stream Deck key to refresh.

## Thread Awareness And Approvals

Thread Visual keys can show running, completed, waiting for input, waiting for approval, warning, and failure states. Press a Thread Visual key to return to the associated thread.

Approval and decline controls act on a concrete waiting request selected through the current thread context. Always review sensitive file, network, or shell actions in ChatGPT before approving them.

## Visual Settings

- **Ambient** changes the base illumination of the key surface.
- **LED Gain** changes the strength of state color.
- **Neighbor Influence** changes how much a lit key affects adjacent keys.

These controls simulate a coherent mechanical keyboard surface on the Stream Deck displays; they do not control physical hardware LEDs.

## Audio Settings

Sound feedback is optional. Completion is enabled by default, while other attention sounds can be selected per state. Use Audio Settings to choose a theme, preview sounds, adjust volume and reverb, or disable audio completely.

## Troubleshooting

Plugin does not appear:
- Restart Stream Deck.
- Confirm Stream Deck 7.1 or later is installed.
- Reinstall the plugin from Marketplace.

Shortcuts remain unavailable:
- Open ChatGPT and confirm the command exists in Keyboard Shortcuts.
- Assign or enable the shortcut in ChatGPT.
- Leave Stream Deck running while the catalog refreshes.

Thread state does not update:
- Open ChatGPT and confirm Codex is available.
- Confirm Stream Deck and ChatGPT run under the same macOS user.
- Restart Stream Deck, then open the affected thread again.

Approval controls do not respond:
- Select the Thread Visual key showing the approval state.
- Review the concrete request in ChatGPT.
- Retry the matching approval or decline control.

## Privacy

See the standalone [Privacy Policy](PRIVACY.md).
