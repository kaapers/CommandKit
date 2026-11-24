# CommandKit
 
A pocket cheat sheet for developers. Search git, terminal and Xcode commands by the **problem** you have, not by the command name.
 
> Example: type "undo last commit" and get `git reset --soft HEAD~1`.
 
## Features
 
### Planned
- Searchable command library (git, terminal, Xcode shortcuts)
- "I messed up" search: finds commands by keywords like undo, revert, oops
- Panic tab: the most common disasters as big buttons
- Favorites
- Tap to copy a command
- Add, edit and delete your own commands
- Quiz mode to learn commands
### Later ideas
- Snippet vault
- Coding time tracker
- Dev journal
- Widget with a command of the day
## Tech
 
- Swift
- SwiftUI
- SwiftData (or Codable + AppStorage)
- Xcode
## Project structure
 
```
CommandKit/
├── CommandKitApp.swift
├── ContentView.swift
├── Shared/
├── Commands/
├── Snippets/
├── Tracker/
├── Journal/
└── Assets.xcassets
```
 
## Getting started
 
1. Clone the repo:
```
git clone <repo-url>
```
2. Open the `.xcodeproj` file in Xcode
3. Pick a simulator and press Run
## Team workflow
 
- One branch per feature, for example `feature/commands`
- Pull before you start working
- Never edit the same file at the same time
- Merge with a Pull Request and review each other's code
- Never commit API keys or secrets
## Team
 
| Person | Area |
|--------|------|
| A | Commands, Journal |
| B | Snippets, Tracker |
 
## Status
 
Work in progress. Just getting started.
 
