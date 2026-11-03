---
name: Pong Arcade
mode: experience
platform: web
tokens:
  colors:
    background: "#000000"
    foreground: "#FFFFFF"
  geometry:
    boardAspectRatio: "1:1"
    corners: "0"
  effects:
    shadows: none
    gradients: none
---

# Design

## Visual direction

Faithful, stark 1970s arcade. The game board is the interface, without ornamental UI chrome.

## Layout

Responsive square field fitting the available desktop viewport while preserving logical game coordinates. The player paddle is on the left and the CPU paddle is on the right. Score digits sit at the top, centered on each player's half.

## Geometry and typography

White narrow vertical rectangular paddles, a small white square ball, a solid vertical white center divider, dashed white horizontal top and bottom boundaries, and large blocky white score digits. Use a monospace system font. No rounded corners.

## States and feedback

Initial start prompt, active rally, one-second centered serve, paused prompt, and terminal YOU WIN or CPU WINS message. Feedback is visual only.

## Interaction

Up and Down move the left paddle, Space starts or restarts, and P pauses or resumes. Control keys never scroll the page. No touch controls.

## Responsive behavior

Scale the square board uniformly and keep gameplay coordinates consistent. Desktop keyboard remains required on narrow viewports.

## Further notes

- Browser window focus is required for keyboard input.
- Large frame gaps are clamped to avoid physics jumps.
- Run the gameplay check by opening `pong.html?test` in a browser.
