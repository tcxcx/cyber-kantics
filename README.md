# cyber-kantics

A Claude **skill** that decomposes a product, feature, protocol, or growth loop into the philosophical *thinking-machine* types it actually runs on — **Cartesian, Humean, Kantian, decisionist, Girardian** — surfaces the **hidden machine** (the logic actually driving behavior, which is rarely the one the builder intended), names the failure loop, and prescribes how to recompose the stack.

It is a diagnostic lens for incentive design: tokenomics, fee/loyalty/VIP mechanics, recommender and feed logic, engagement and status loops, referral mechanics, agent behavior — anything that shapes desire.

## The five machines

| Machine | Relates action to… | Signature | Characteristic failure |
|---|---|---|---|
| **Cartesian** | fixed a-priori rules | hard-coded thresholds, "code is law", explicit if/else | brittle, gameable |
| **Humean** | quantified own-history data | volume tiers, surge pricing, "more usage → more" | can't escape its probability space; self-consumption |
| **Kantian** | rules *derived* from cases under constraints | reflective judgment, a "constitution" filtering a raw engine | expensive; can ossify back into rules |
| **Decisionist** | the *exception* | freeze/blacklist, circuit breaker, admin override | the exception normalizes |
| **Girardian** | *mimetic* desire (I want it because others want it) | status tiers, VIP, leaderboards, social proof | the loop amplifies to mutual destruction; mercenary, non-sticky |

The core move is one question: **which machine is actually running under the one they think they built?** The crisp discriminator: *whose data is in the function — yours (Humean) or other people's (Girardian)?*

## Install

A `.skill` file is a zip with a `SKILL.md` inside. Two ways to use it:

**Claude Code / Cowork (as a plugin skill):** drop the `cyber-kantics/` folder into your skills directory (e.g. a marketplace plugin's `skills/` folder, or your project's `.claude/skills/`), so the path is `…/skills/cyber-kantics/SKILL.md`. It loads automatically when a matching task appears.

**Upload the artifact:** in surfaces that accept a `.skill` upload, use `cyber-kantics.skill` directly.

**Manual:** unzip `cyber-kantics.skill` and place the resulting `cyber-kantics/` folder wherever your environment discovers skills.

> Skills load by their `description`. This one is written to trigger even when you don't name the framework — e.g. "why does this loop burn out?" or "review the incentive logic of X."

## Usage

Point it at a system and ask for a decomposition:

- "Decompose `feat/kawaii-vip-fee-discount` into its machine stack."
- "Is this fee tier Humean or Girardian?"
- "Why does this leaderboard burn out, and how do I make it sticky?"
- "Review the behavioral logic of a stablecoin with a freeze function."

It returns: a stack inventory (surface → machine type), intended-vs-actual with the hidden machine, the failure loop, the missing machines (each an explicit vulnerability), and an ordered recomposition mapped to concrete surfaces.

## Credits

This skill is an applied synthesis of two texts; the underlying ideas are theirs, not mine:

- **Yuk Hui**, *Kant Machine: Critical Philosophy after AI* (2026) — the Cartesian / Humean / Kantian → cybernetics core.
- **Fernando Wirtz**, "The Philosophy Behind Artificial Intelligence: Cyber-Kantianism and Dark Girardianism," *421.news*, 5 June 2026 — the decisionist and Girardian extensions, and the "dark Girardianism" reading of the tech-right. The skill's name borrows Wirtz's term *Cyber-Kantianism*. https://www.421.news/en/ia-thiel-yuk-hui-kant-girardi-philosophy-en/

The decisionist machine draws on Carl Schmitt; the Girardian machine on René Girard's mimetic theory.

## License

MIT — see [LICENSE](LICENSE). Applies to the skill text and packaging. The conceptual framework is credited above and remains the work of its authors.
