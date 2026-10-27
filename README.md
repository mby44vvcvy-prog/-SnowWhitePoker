# Snow White and the Seven Gnomes

An anonymised, play-money Manila poker demo. One human plays against seven heuristic computer opponents; these are personality-weighted rules, not live language models.

## Version 1.0.0
This is the initial fairytale release, derived from the existing Manila game. Character names are fictional. No Disney artwork or assets are included.

## Rules
32 cards, ranks 7 to Ace. Both hole cards and exactly three community cards are mandatory. Flush beats full house. A-7-8-9-10 is the low straight. Five community cards appear one per betting round; the first is revealed before action. Dealer rotates; next player posts one chip. Eight players start with 50 chips for a ten-hand match. Suit order is spades, diamonds, clubs, hearts. No real-money wagering.

## Customisation
Edit the roster for names, icons and heuristic personalities. The ranks and suits arrays define the deck. scoreFive and labels define hand rankings; compareSuitTiebreak defines house ties. Starting chips and match length are currently literals in several functions: update them together and test. Rules are source-code customisations, not a runtime settings editor.

## GitHub and Render
Create a NEW repository and upload these files as an initial commit. Do not fork or copy the original git history: earlier commits contain personal names. Deploy as a Render static site, publish directory '.', build command 'echo Static site ready', branch main. Verify the live version before announcing it.

## Versioning
Use semantic versions: patches for bug fixes, minor versions for compatible features, major versions for incompatible rule changes. Update the visible footer and CHANGELOG together. Git commits record changes; release tags mark tested versions; Render deploys the selected branch. Keep a known-good commit for rollback.

## Validation status
Names have been replaced and source checked. Browser playtesting and deployment of this edition are still pending. The inherited game needs regression tests for all-in pots, tie rules, hand rankings and restarting while computer timers are pending before stronger reliability claims.
