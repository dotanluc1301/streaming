# Streaming Project

## Overview

This project is a single-page streaming front-end built around TMDB data and multiple embed provider sources.
It allows users to browse movies and TV shows, open details in a modal, select a streaming provider, and play content via an embedded iframe.
The app also supports watchlist/favorite sync, history tracking, and a settings panel for TMDB API configuration.

## Features

- Browse popular movies and TV shows using TMDB.
- Hero carousel with featured trending content.
- Search and discovery pages with filters for genre, country, and language.
- Detailed modal views for movies and TV shows.
- Streaming provider selection with direct iframe embedding.
- TV show season and episode controls.
- Watchlist and favorites synced via TMDB account APIs.
- Continue watching history saved in localStorage.
- Responsive design with modern UI interactions.

## Streaming Mechanism

1. The app fetches content metadata from TMDB using a TMDB API key.
2. When a user opens a movie or TV show, the modal loads details from TMDB.
3. The user can choose a streaming provider from the modal or player controls.
4. The selected provider is converted into an embed URL using the TMDB ID.
5. The player iframe is updated with the provider-specific embed URL.

## Configuration

- `TMDB API Key` can be set in the settings panel.
- `Default Provider` can be selected in settings for new sessions.
- Subtitle language support is available via the `Subtitle Language` setting.

## Notes

- New providers use TMDB IDs directly and do not rely on IMDb lookup.
- The app remains a client-side HTML page with all logic embedded in `index.html`.
