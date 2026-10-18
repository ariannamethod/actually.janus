# TRUELOG

the log of changes, newest first. each entry: what changed, and the run that proves it.

## 2026-10-18 — every alphabet fits through the door

three fixes by Don after Oleg fed the door Russian and got punctuation back: `<meta charset="utf-8">` first in head; `tokenize` moves `[A-Za-z0-9]` → `\p{L}\p{N}` with the `u` flag; `isPunct` likewise, so a single Cyrillic letter is no longer punctuation. Proofs, live browser on this file: the old regex reduced «Дверь помнит всех, кто прошёл сквозь неё» to commas and periods, the new one keeps every word (node probe, both regexes side by side); a Russian corpus reads as 1,068 tokens / 120 sentences, bigrams 170, trigrams 177, hebbian 657, both directions; a Russian origin grows past and future in Russian — chain closed, 12 steps, debt 0.158, 1 crack; the English chain still closes after the fix (12 steps, debt 0.447); ledger glyphs ↑ ↓ · render clean even when the file is served without a charset header. Named limits: STOP list stays English (other languages run a noisier hebbian); RTL rendering unchecked.

## 2026-10-18 — first layer received

`janus.html` as built by Fable on Claude Desktop overnight, one file, 627,879 bytes, the Q corpus inside. Bidirectional field (`succ`/`pred`, `triS`/`triP` — what follows a pair and what precedes one); backward sentences grown from the seam with the last word chosen first; best-of-5 candidates judged by internal coherence plus seam, seam-weighted on the backward side; expectations that must meet a witness, debt 0.9·debt + 0.1·gap; rereading with ±0.1 hysteresis relabeling the past evidence/contra; SPA-lite regrowth of weak seams keeping the old sentence as a layer; calendar drift 365.25/354 with personal dissonance from the day of first opening; six Kuramoto chambers; user words entering the metaweights in both directions. Audited by Don against the builder's own report: every claimed mechanism found at its stated place in the code and exercised in a live browser — 12-step chain closes, backward seam 4.83, the ledger narrates seams, rereads, cracks and regrowth. Builder's named limits at delivery: phone rendering unchecked by him, weights outside the file.
