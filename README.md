# Aigis

I got tired of asking myself "wait, how do I run this thing again?" every time I switched projects.

Aigis is a CLI/TUI that keeps track of your projects and how to work with them. It's basically a smarter `cd` that remembers what each project needs.

---

## The problem

You know the drill:

- Project's in some folder you can't remember
- Need to check if the dev server's already running
- Was this the one using Docker or just npm?
- Which git branch were you even on?
- Want to spin up a new React app but can't remember if it's `npm create vite` or `npx create-react-app` or what

I kept a messy `~/projects` folder and a bunch of shell aliases that barely helped.

---

## What it does

### Keeps a registry of your projects

Add a project once, switch to it anytime. Tag things however you want. Open in whatever editor you use.

### Figures out what's actually running

Checks processes, Docker containers, open ports. Shows you if your project's already up or if you forgot to kill something.

### Knows your stack

Detects package.json, Cargo.toml, go.mod, whatever. Shows git status, current branch, uncommitted changes.

### Runs stuff

Hit a key to start dev server, run tests, build, spin up Docker. It just runs the commands your project already has.

### Bootstraps new projects

Wraps `cargo init`, `bun create`, `npm create vite`, etc. Pick a template, name it, done.

### Works in the terminal

Fast CLI for when you know what you want. TUI when you're browsing or forgot the command.

---

## What what will be supported on the first release

- JavaScript/TypeScript (Node, Bun, Deno)
- Rust
- Go
- Python
- C/C++
- Docker/Compose
- Git
- Nix (basic detection) // this one will be on v2

More stuff gets added when I need it or someone asks for it.

---

## What this isn't

Not a build tool. Not a package manager. Not trying to replace your editor or your terminal setup.

Just a layer on top that remembers things so you don't have to.

---

## Current state

I'm actively building this for my own use. It works but things will change. Don't rely on anything being stable yet.

If you want to try it, cool. If you find bugs or have ideas, open an issue.

---

## Why "Aigis"?

Greek word for shield. Sounded cool and wasn't taken on crates.io and pkg.go.dev.
