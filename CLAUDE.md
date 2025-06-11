# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Pac-Man game implementation intended to be built with HTML, CSS, and JavaScript. The project is currently in its initial state with only basic setup files.

## Commands

### Development
- No build command currently configured
- No lint command currently configured
- Test command exists but not implemented: `npm test` (currently returns an error)

## Architecture Notes

This is a greenfield project. When implementing the Pac-Man game, consider:

1. **File Structure**: Create a logical structure such as:
   - `index.html` - Main game HTML file
   - `css/` - Stylesheets for the game
   - `js/` - JavaScript game logic
   - `assets/` - Game sprites, sounds, and other media

2. **Game Components**: Key elements to implement:
   - Game board/maze
   - Pac-Man player character
   - Ghost enemies (Blinky, Pinky, Inky, Clyde)
   - Pellets and power pellets
   - Score tracking
   - Lives system
   - Game states (start, playing, game over)

3. **Technology Stack**: 
   - Plain HTML, CSS, and JavaScript (based on package.json keywords)
   - No framework dependencies currently defined