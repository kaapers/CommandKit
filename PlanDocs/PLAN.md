# CommandKit: Plan

## Split by feature (tabs), not by UI vs logic
Each person owns whole tabs, so you rarely touch the same files.

## Step 0: together (30 min)
- [x] Create the Xcode project and push to GitHub
- [x] Teammate clones it
- [ ] Add `.gitignore` and `README.md`
- [ ] Create folder groups: Commands, Snippets, Tracker, Journal, Shared
- [ ] `TabView` in ContentView with 4 placeholder screens (`Text("Commands")` etc.)

## Person A: Commands tab, then Journal
Branch: `feature/commands`

1. `CommandItem` struct: name, command, description, category, keywords. Make it `Identifiable`.
2. Hardcoded array of 10 commands (DefaultCommands.swift)
3. List screen with `List` + `ForEach`
4. Search with `.searchable(text:)` + filter (name, description AND keywords)
5. Categories: Git / Terminal / Xcode
6. Detail screen: `NavigationStack` + `NavigationLink`
7. Tap to copy: `UIPasteboard.general.string`
8. Favorites + custom commands (storage)
9. "I messed up" search + Panic tab
10. Journal tab (later)

## Person B: Snippets tab + Tracker tab
Branch: `feature/snippets`, then `feature/tracker`

Snippets:
1. `Snippet` struct: title, code, language, tags
2. List screen + add screen
3. Search by title and tag
4. Save data (storage)

Tracker:
1. `CodingSession` struct: project, start, end
2. Start / stop timer
3. Save sessions
4. Weekly chart (Swift Charts)

## Together (at the end)
- Quiz mode
- Shared theme (colors, fonts)
- Settings screen
- App icon
- Polish and bug fixing

## Git rules
- One branch per feature
- `git pull` BEFORE you start working and BEFORE you push
- Never edit the same file at the same time
- `Shared/` files: tell each other before changing
- Merge with a Pull Request, and review each other's code
- Never commit API keys or secrets

## Who is who
| Person | Name | Tabs |
|--------|------|------|
| A | | Commands, Journal |
| B | | Snippets, Tracker |
