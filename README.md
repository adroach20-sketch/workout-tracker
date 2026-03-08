# Workout Tracker

A lightweight personal workout tracker built as a single HTML file. Designed to be pulled up on a phone at the gym — dark theme, big tap targets, zero dependencies.

## What It Does

- Shows today's workout based on the day of the week
- Tracks weight, reps, and sets for each exercise
- Pre-fills inputs with your last logged values
- History view with progress charts per exercise
- Week navigation to look ahead or log missed days
- Green dots on days you've logged workouts

## Weekly Schedule

| Day       | Workout          | Location  |
|-----------|------------------|-----------|
| Monday    | Pull + Legs      | Cedardale |
| Tuesday   | Boxing           | 6 AM Class |
| Wednesday | Upper Hypertrophy| Cedardale |
| Thursday  | Boxing           | 6 AM Class |
| Friday    | Legs + Core      | Cedardale |
| Saturday  | Full Body Circuit | Basement (optional) |
| Sunday    | Rest             | — |

## Tech

- Single `index.html` file — all CSS and JS inline
- No frameworks, no dependencies, no build step
- localStorage for all data (persists in browser)
- Hosted as a static site on Render

## How to Run Locally

Just open `index.html` in a browser.

## How to Deploy

Connect this repo to Render as a **Static Site**. Set the publish directory to the repo root (`.`). It will serve `index.html` automatically.

## Data

All workout data is stored in your browser's localStorage. If you clear browser data, the history is gone. This is a personal tool — no accounts, no server, no database.
