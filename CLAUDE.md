# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Japanese meme maker web application called "shimaimashita-maker" that allows users to overlay text on an anime-style image. The application enables users to select rectangular regions on the image and add multi-line, word-wrapped text within those regions.

## Architecture

- **Single-file application**: The entire application is contained in `index.html` with embedded CSS and JavaScript
- **Canvas-based image manipulation**: Uses HTML5 Canvas API for image rendering and text overlay
- **Interactive region selection**: Users can drag to create new text regions or move existing ones
- **Text rendering**: Supports multi-line text with automatic word wrapping within selected regions
- **Export functionality**: Generates downloadable PNG files with text overlays

## Key Components

- **Image loading**: References `normal.png` as the base image for text overlay
- **Rectangle selection system**: Handles mouse events for creating and moving text regions
- **Text rendering engine**: Implements word wrapping and multi-line text drawing within clipped canvas regions
- **Export system**: Creates clean output without selection borders for download

## Development Notes

- The application is designed to run directly in a browser without build tools
- Text is rendered in black at 34px font size with automatic line breaks
- The selection rectangle has a red dashed border for user interaction
- The base image (normal.png) should be kept in the same directory as index.html