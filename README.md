# Number Guesser (Interactive Range Guesser)

An interactive range-based number guessing application featuring a dynamic web-based dashboard and a Jupyter Notebook integration. The project is implemented in pure HTML, CSS, and JavaScript, with a Python notebook variant.

## Project Structure

The project consists of the following primary components:

*   **`index.html`**: A standalone web application containing the complete user interface, responsive layout, retro audio synthesizer, particle engine, and game mechanics.
*   **`Interactive_Number_Guessing_Game_(1).ipynb`**: A Jupyter Notebook designed to run in environments like Google Colab or local Jupyter servers. It contains:
    *   An interactive CLI-based Python script for terminal-based number guessing.
    *   An embedded HTML implementation that renders the complete web dashboard directly inside notebook outputs using `IPython.display.HTML`.

---

## Features

### 1. Game Setup & Customization
*   **Variable Limits**: Users can specify custom minimum and maximum range bounds (e.g., 1 to 100).
*   **Adjustable Lives**: Quick selection buttons for 10, 6, or 3 lives, alongside a custom input field for entering a specific number of attempts.
*   **Interactive Input Control**: Real-time slider with custom range adjustments, accompanied by nudge buttons (`-` and `+`) to increment or decrement the guess by one.

### 2. Feedback Systems
*   **Dynamic Assistant**: Gippy, the robot assistant, responds to guesses with interactive dialogue and animated mood expressions depending on the guess outcome.
*   **Proximity Thermometer**: A multi-stage visual indicator that updates with different states (Cold, Warm, Hot, and Super Close) based on the absolute mathematical distance to the secret number.
*   **Timeline History**: A sequential list displaying past guesses labeled with high/low directions and temperature statuses.

### 3. Audiovisual Enhancements
*   **Retro Sound Synthesizer**: Web Audio API-driven synthesis generating real-time tone cues for game actions (clicks, successes, high/low warnings, errors). Sound can be toggled on or off directly via the interface.
*   **Confetti Particle Engine**: An HTML5 Canvas particle renderer that executes a celebration animation upon winning.
*   **Dynamic Theme Selection**: Switchable UI skins including a pastel playground layout (light theme), slate console dashboard (high-contrast dark theme), and arcade dashboard (cyberpunk theme).

### 4. Metrics & Score Tracking
*   **Persisted Stats**: LocalStorage keeps track of persistent records across sessions.
*   **Live Dashboard**: Real-time update charts showing games played, win rate percentage, best winning streak, and personal record (fewest guesses to solve).
*   **Animated Counter Ticker**: Counters count up dynamically to display target metric values on the scoreboard.

---

## Technical Architecture

*   **Core Logic**: Vanilla JavaScript with object state-oriented programming.
*   **Styling**: Pure CSS3 utilizing custom properties (CSS variables) to handle live theme swapping without reloading the page.
*   **Responsiveness**: Flexbox layouts and CSS Grid structures styled to resize automatically for both mobile screen displays and desktop windows.
*   **Audio rendering**: Synthetic wave oscillators (`sine` and `triangle` wave types) generated using standard hardware interfaces via the browser's `AudioContext`.

---

## How to Play

### Option A: Web Application
1. Open the [index.html](index.html) file in any modern web browser (Chrome, Firefox, Edge, Safari).
2. Set your custom range boundaries and the number of lives.
3. Click **START GAME! 🚀**
4. Drag the range slider or use the nudge buttons to target a number.
5. Click **SUBMIT GUESS! 🎯** to submit. The thermometer and Gippy will help guide your next guess.

### Option B: Jupyter Notebook
1. Open [Interactive_Number_Guessing_Game_(1).ipynb](Interactive_Number_Guessing_Game_(1).ipynb) in a notebook environment (Google Colab, VS Code, or JupyterLab).
2. Execute the first code cell to play the command-line Python variation.
3. Execute the second code cell to render the complete visual HTML5 dashboard inline inside your notebook output.
