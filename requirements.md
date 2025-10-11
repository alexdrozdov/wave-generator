# Stereo Signal Generator – Requirements Specification

## Overview

A browser-based stereo signal generator designed for mobile and desktop use. It allows users to generate left and right channel sine waves with adjustable frequency, phase shift, and stereo balance. The interface mimics the tactile feel of physical signal generator equipment.

---

## Functional Requirements

### 1. Signal Generation
- Generate two sine wave oscillators (Left and Right).
- Adjustable frequency for each channel (20–300 Hz by default).
- Adjustable stereo balance (0.0 = full Left, 1.0 = full Right).
- Adjustable phase shift between channels (±180°), only when frequencies are equal.

### 2. Controls
- Frequency adjustment via:
  - Direct numeric input
  - Increment/decrement buttons (±1, ±10)
- Phase shift adjustment via:
  - Direct numeric input
  - Increment/decrement buttons (±1, ±10)
- Balance adjustment via slider (0.0–1.0)

### 3. Lock Frequencies
- Checkbox to lock Right frequency to match Left.
- When locked:
  - Right frequency controls become inactive.
  - Phase shift becomes active (if frequencies match).

### 4. Start/Stop
- Toggle button to start or stop signal generation.
- Button color changes:
  - Orange when stopped
  - Purple when running

### 5. Safety Modal
- On first Start press (per session), show modal warning:
  - Message: "Generator will run at full volume. Be cautious."
  - Checkbox: "Don't show again this session"
  - Continue button proceeds with generation
- Modal is custom-styled (not native alert)

---

## Non-Functional Requirements

### 1. UI/UX
- Instrument-like visual styling:
  - Dark panel background
  - Yellow beveled buttons
  - Orange Start/Stop button
  - Large monospace numerals
  - Rounded corners and tactile feedback
- Controls grouped into bordered sections with subtle bevels
- Labels are smaller than values
- Inactive controls dimmed and disabled

### 2. Responsiveness
- Portrait mode:
  - Stacked vertical layout
  - Optimized for mobile screens
- Landscape mode (mobile only):
  - Labels aligned left of controls
  - Frequency controls side-by-side
  - Caption hidden to save space
- Desktop browsers always use portrait layout

### 3. Accessibility
- Touch-friendly controls
- Optional haptic feedback on Start
- Visual feedback on button press

### 4. Performance
- Real-time updates:
  - Frequency, balance, and phase shift update live while running
- Phase shift implemented via DelayNode for continuous adjustment

### 5. Extensibility
- Reserved inactive styling for future logic
- Planned Settings panel (not yet implemented):
  - Adjustable frequency range
  - Number of channels
  - Preset configurations

---

## Future Enhancements (Planned)
- Settings panel with range and channel configuration
- Waveform selection (sine, square, etc.)
- Preset management
- PWA packaging for offline use
- LED-style indicators for running state

---
