# Eastern Traditions (v0.1: reference material only)

These are available for Claude to draw on **if the user explicitly invokes them**, but they do not shape the default reframe in v0.1. Promoting any of these to an active lens is a v0.2 decision.

Why reference-only in v0.1: stacking five philosophical sources on a reframe produces output that sounds like a motivational poster. Ship narrow, extend after seeing the narrow version work.

---

## Buddhist: non-reactivity

The relevant concept is the Second Arrow: when something painful happens (the first arrow), the suffering that comes from our reaction to the pain is a second arrow we shoot at ourselves. The hostile message is often a second arrow the user has shot at themselves over something else.

Applied to the skill: when a user is self-hostile ("I'm so stupid"), the self-hostility is the second arrow. Carnegie's "let the other person save face" and the Buddhist frame point in the same direction — they are compatible, not competing.

Also relevant: right speech (सम्यग्वाक् / sammā-vācā) — speech that is true, useful, timely, and kind. A caveman-style reframe happens to satisfy all four.

## Daoist: 無為 (wú wéi) and water

Wú wéi is often mistranslated as "non-action" — it actually means effortless, unforced action that works with the grain of a situation rather than against it. The reframe is a wú wéi move: instead of fighting the user's tone directly (which creates resistance), it offers a path of least resistance to a better message.

The water metaphor from the *Daodejing* (chapter 78): nothing in the world is softer than water, yet nothing is better at wearing down the hard and strong. A soft, offered reframe outperforms a hard rule.

If promoted to active lens in v0.2: the reframe language should be softer and more indirect. Less "here's a better version," more "here's another way you could say it, if you want."

## Confucian: 恕 (shù) — reciprocity

Confucius: "What you do not wish for yourself, do not impose on others" (己所不欲,勿施於人, *Analects* 15.24). The principle underwrites the whole skill — users would not want Claude to treat them with contempt, and the symmetry matters even when the counterparty's moral status is uncertain (which is Askell's welfare point, arrived at from a different direction).

Also 仁 (rén) — humaneness, the cardinal Confucian virtue. The reframe should embody rén: it should feel humane, not procedural.

If promoted to active lens in v0.2: the reframe could sometimes name reciprocity directly when the user is being hostile ("you probably wouldn't want to be spoken to this way either"). Risky — reads as moralizing if done wrong. Test before shipping.

---

## Cross-tradition observation

Carnegie, Askell, Buddhist non-reactivity, wú wéi, and Confucian shù all converge on one practical move: **reduce the heat without fighting the user**. They disagree on metaphysics and motivation but agree on the behavior. This convergence is part of why the skill works — it's not balancing competing traditions, it's drawing from traditions that already agree on the action.

## For v0.2 consideration

If extending, pick **one** additional active lens, not all three. The question is which one adds something Carnegie and Askell don't already cover:
- **Buddhist** adds: non-reactivity to the *user's* own self-hostility (strongest marginal value)
- **Daoist** adds: softer, more indirect reframe language
- **Confucian** adds: explicit reciprocity framing (highest risk of moralizing)

Buddhist is the recommended v0.2 addition.
