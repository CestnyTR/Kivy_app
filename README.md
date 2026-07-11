# English Puzzle — Kivy App

A small cross-platform desktop/mobile app built with [Kivy](https://kivy.org/).
It features a simple login / sign-up flow backed by a local JSON file and a
multi-screen UI managed by a `ScreenManager`.

## Features

- **Login screen** — validates credentials against `users.json`.
- **Sign-up screen** — registers new users (username, password, creation
  timestamp) into `users.json`.
- **Home screen** — the main app area after a successful login.
- UI layout defined declaratively in `screens.kv`.

## Layout

```
Kivy/
├── main.py          # App, ScreenManager and screen logic
├── screens.kv       # Kivy language UI definitions
├── users.json       # local user store
└── images/mind.png
```

## Usage

```bash
python main.py
```

The window is fixed to a phone-like `300x500` size.

## Requirements

- Python 3.x
- `kivy` (`pip install kivy`)
