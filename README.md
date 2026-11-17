# replace-dead-tools

An agent skill for Claude Code, Codex and Cursor that checks every tool on best-of articles and
awesome-lists for parked domains, shutdowns, acquisitions and archived or deleted GitHub repos,
confirms each verdict with a link an editor can open, and drafts a replace-the-dead-entry pitch.
A check that was blocked stays INCONCLUSIVE. It's never called dead.

    npx skills add arm-pz/replace-dead-tools --skill replace-dead-tools

Ask it things like:
- "Find the dead tools still sitting on those lists, so I can be the replacement."
- "Which tools in these 'best project management apps' articles were discontinued or acquired?"
- "Check these 12 listicle URLs for products that no longer exist."

See a real run: [skillsmith.tech, November 2026](https://github.com/arm-pz/clauderepo/tree/ccr-e894c200-72sjk2/proof/skillsmith-tech): 138 tools checked in 90 seconds,
12 flags, 0 confirmed dead after review (3 domain moves, 2 rebrands, 2 false matches, 5 blocked
checks). Zero is reported as zero.

Step 2 of [get-listed](https://github.com/arm-pz/get-listed) → **replace-dead-tools** →
[find-partners](https://github.com/arm-pz/find-partners). It also starts on its own from a list of
article URLs.
