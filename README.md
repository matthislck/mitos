# Mitos

A pattern for learning a new field with an LLM – and proving you actually understood it.

Learning with an LLM is easy to start and hard to keep. You ask, it explains, the explanation is good, and a week later it's gone. Two things never accumulate: **orientation** (where do I start, what builds on what, what is the shape of this field?) and **retention** (at the end of a session you have a chat log, not a structure you can return to). And underneath both sits the real trap: reading a clean explanation *feels* like understanding, so you never find out whether you actually do.

Mitos turns a field into a **directed dependency graph** – concepts as nodes, "prerequisite-of" as the arrows – that you build, document, and then have to **rebuild from memory** to prove you understood it. The gap between the reference graph and the one you can redraw blind is the only thing it measures.

I built this while learning AI and agents, because I kept hitting the same wall: without structure, documentation, and a real test of understanding, learning carries a lot of unnecessary cognitive load – you're holding a field whose whole picture you don't have yet. So I built the tool to learn the topic, with the agent itself.

## How to use it

Mitos is an **idea file**, not an app – there is nothing to install. You copy [`mitos.md`](./mitos.md) into your own LLM agent (Claude Code, Codex, etc.), and it sets the pattern up with you in a short conversation; the output is a small schema your agent then runs from. Obsidian is the viewer.

The loop, once it is set up:

- **generate** – the agent draws an orientation graph of the field, taking the cognitive load of structuring it off you.
- **capture** – you write each concept in your own words and justify its prerequisite edges; the agent examines you Socratically but never writes the answer.
- **validate** – you correct the graph into a reference you trust.
- **reconstruct** – you rebuild the graph from memory, blind.
- **diff** – the agent shows you exactly which connections you missed. That is your study target. Then: next topic.

The full pattern, the reasoning behind it, and the conventions live in [`mitos.md`](./mitos.md).

## Status

v0.1 – experimental, tested on myself across one real topic. It matches how I actually learn; whether it generalizes is an open question. Issues and forks welcome.

## License

MIT – take it, adapt it, build on it. That is the point of an idea file.
