# Lumines Frame Editor

`Lumines Frame Editor` is a single-file tool for arranging Lumines board states frame by frame so you can revisit and analyze them later at your own pace. You can redraw boards by hand, add or duplicate frames, and play them back to follow move sequences and board changes visually.

To keep it easy to publish on GitHub Pages, the implementation is contained in a single file: `lumines_frame_editor.html`.

## Features

- Edit a fixed-size `16 x 10` board
- Place cells using 5 colors plus Garbage
- Add, duplicate, delete, and clear frames
- Move through frames on a timeline and play them back in sequence
- Add captions to individual frames
- Export the current frame as a PNG
- Paste a game screenshot with `Ctrl+V`, select the board area, and import it into the current frame
- Show the number of color-specific squares in the current board's clear area
  - `Normal`: 2x2
  - `BURST`: 2x2 or larger

## How To Use

1. Open `lumines_frame_editor.html` in a browser.
2. Choose a color from the palette on the left, then drag on the board to edit it.
3. Use `Add` or `Duplicate` to create more frames, and write notes in `Caption` if needed.
4. Press `Play` to preview the frames in order.
5. Use `Export PNG` when you want to save the current frame as an image.

If you want to reconstruct a board from an image, copy a game screen, press `Ctrl+V` on the page, drag over the board area in the preview on the right, and click `Import From Image`. The color detection is automatic, but it is not very accurate, so manual cleanup is often necessary.

## Controls

- Left drag: paint
- Right drag: erase
- `ArrowLeft` / `ArrowRight`: move between frames
- `Space`: play / stop
- `N`: add a blank frame
- `D`: duplicate the current frame

## File Structure

- `lumines_frame_editor.html`: application
- `README.md`: Japanese README
- `README.en.md`: English README

## Purpose

This tool is meant less for solving Lumines boards on the spot and more for documenting them so they can be reviewed and discussed later. It is suited for match review, strategy notes, move breakdowns, and sharing how a board changes over time.
