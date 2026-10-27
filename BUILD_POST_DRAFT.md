# A custom Manila poker table in one HTML file

Snow White and the Seven Gnomes is a play-money poker prototype: one human and seven personality-weighted computer opponents. The opponents use heuristics rather than live LLM calls, so each move needs no paid inference service.

The interesting part is custom house rules: a 32-card deck, both hole cards mandatory, flush above full house, rotating dealer and suit-based tiebreaks. A generic poker evaluator is not enough; it must evaluate exactly the allowed five-card combinations.

This edition separates fictional character names from the original table. Rules are customised in source, not through a settings screen. GitHub records revisions, semantic versions identify releases, and Render serves the static HTML. Hosting and source links will be added after this edition is deployed and tested.

The next work is regression testing edge cases, especially side pots and tied straights. For people building games with local rules: which rule caught a plausible-looking evaluator doing the wrong thing?

Status: prepared source edition; live demo and browser validation pending. Do not publish this draft as a shipped-build claim until verified.
