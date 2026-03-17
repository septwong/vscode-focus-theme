# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a VS Code color theme extension providing "Focus" themes (light and dark) that highlight only what matters: strings, constants, top-level definitions, and meaningful comments.

## Development

Press `F5` in VS Code to launch Extension Development Host and test theme changes live.

## Files

- `package.json` - Extension manifest with theme contributions
- `themes/focus-theme-dark.json` - Dark theme token colors
- `themes/focus-theme-light.json` - Light theme token colors

## Making Theme Changes

Edit the JSON files in `themes/`:
- `colors` - Workbench/UI colors (editor, sidebar, tabs, etc.)
- `tokenColors` - Syntax highlighting scopes

Use `Developer: Inspect Editor Tokens and Scopes` command to identify scopes for syntax elements.

## Publishing

Package with vsce:
```bash
vsce package
```
Then publish to VS Code Marketplace or Open VSX Registry.