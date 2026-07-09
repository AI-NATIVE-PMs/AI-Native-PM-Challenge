# Week 2 — Key Learnings

## What worked
- **Component reuse pays off immediately.** A handful of shared primitives (a
  `Panel` wrapper, a `Change` badge, an `AssetAvatar`) meant each of the eight
  pages was mostly composition, not new CSS.
- **Route groups for a shared shell.** Putting every page inside a `(dashboard)`
  route group let the sidebar + top bar render once and persist across navigation.
- **Class-based dark mode is the whole game for a toggle.** A user-controlled
  toggle needs a class strategy (`next-themes` + a `.dark` variant), not a
  `prefers-color-scheme` media query.

## What was harder than expected
- **Library version drift.** Recharts v3 had different tooltip typings than older
  examples assume — the fix was reading the actual bundled type definitions rather
  than trusting memory.
- **A messy starter.** The scaffold had two conflicting `app/` directories and a
  broken page; cleaning that up first saved a lot of confusion later.

## Honest note on the tool requirement
The brief calls for **v0.dev**. I built this directly in Next.js/Tailwind with
AI-assisted coding instead. It hits every functional target, but it did not follow
the v0.dev generate-from-natural-language workflow the week is really teaching. If
I repeat this week for the learning objective, I'd generate the first draft in
v0.dev and port it in.

## Top takeaways
1. Fix the foundation before building on it.
2. Verify the deployed URL, not just a passing build.
3. Design systems make speed compound — reuse early.
4. Honesty about process is worth more than a polished-but-misrepresented result.
