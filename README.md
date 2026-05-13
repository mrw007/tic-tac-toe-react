# Tic-Tac-Toe React Demo

A small React learning project built while following the Udemy course **React - The Complete Guide (incl. Next.js, Redux)**.

This app implements a classic tic-tac-toe game with a polished UI and a simple component-based architecture. It is intended as a hands-on demo for practicing core React concepts such as state management, derived state, event handling, conditional rendering, and component composition.

## What This App Does

- Lets two players take turns placing `X` and `O` on a 3x3 board
- Highlights the currently active player
- Allows player names to be edited during the game
- Tracks and displays the move log
- Detects winning combinations
- Detects draw conditions when all squares are filled
- Supports restarting the match with a rematch action

## Built With

- React 19
- Vite
- JavaScript (ES Modules)
- CSS

## React Concepts Practiced

This demo is useful for learning and reinforcing:

- `useState` for local component state
- Passing data via props
- Lifting state up to a parent component
- Derived values based on existing state
- Immutable state updates
- Conditional rendering
- Rendering lists with `map()`
- Splitting UI into reusable components

## Project Structure

```text
src/
	App.jsx
	index.jsx
	index.css
	winning-combinations.js
	components/
		GameBoard.jsx
		GameOver.jsx
		Log.jsx
		Player.jsx
```

## Getting Started

### Prerequisites

- Node.js 18 or newer
- npm

### Installation

```bash
npm install
```

### Start The Development Server

```bash
npm run dev
```

Then open the local URL shown by Vite in your terminal.

## Available Scripts

```bash
npm run dev
```

Starts the Vite development server.

```bash
npm run build
```

Builds the app for production.

```bash
npm run preview
```

Previews the production build locally.

```bash
npm run lint
```

Runs ESLint for the project.

## How The Game Works

- The board state is derived from the recorded turns instead of being stored separately as the primary source of truth
- The active player is calculated from the current turn history
- The winner is derived by checking the board against predefined winning combinations
- A draw is declared when all nine turns are used and no winner exists

## Learning Purpose

This repository is a training project, not a production application. The goal is to practice React fundamentals by building a complete but manageable UI example from scratch.

## Course Reference

Based on exercises and concepts from the Udemy course **React - The Complete Guide (incl. Next.js, Redux)**.