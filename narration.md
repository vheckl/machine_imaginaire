# Narration Export

All narrator/voice, instructional, and caption text pulled from `script.js`, in gameplay order. Game logic, IDs, CSS, and generic interaction chrome ("click to continue", "click dice to roll", "skip game", etc.) are omitted.

A final section at the bottom covers the three new "rule panel" texts — these actually live as static markup in `index.html`, not in a JS array, so they're flagged separately.

---

## VOICE_LINES

*(s1 — opening biographical narration)*

1. My name is Vera Molnár. I was born in Budapest in 1924. I died in Paris in 2023. I worked every single day in between.
2. I trained as a painter. I started with nymphs and trees — the usual things young painters do.
3. But very quickly I understood that what interested me was not the image. It was the *system* that produced the image.
4. I began to impose rules on myself. Divide the surface into a grid. Assign values. Follow them without deviation.
5. No intuition. No mood. No 'today I feel like painting something blue.' Only the rule.
6. The art world found this cold. Mechanical. They preferred painters who suffered visibly.
7. I did not care. I was asking a different question entirely: what happens when you remove the artist from the decision?
8. What is left? Is it still art? And if it is — then what exactly was the artist contributing in the first place?
9. For years I had no computer. Computers were for the military, for scientists. Not for Hungarian women painters in Paris.
10. So I invented one. In my head. I called it the *machine imaginaire* — the imaginary machine.
11. I divided paper into grids. I wrote out the rules. Then I sat down and followed them, cell by cell, mark by mark.
12. I was the processor. My hand was the plotter. And the algorithm — that was mine.
13. In 1968 I finally got access to a real computer — an IBM 2250 at the Université de Paris in Orsay.
14. It had a screen. A light pen. I could watch the image change in real time as I adjusted the parameters.
15. I called this the méthode conversationnelle — the conversational method. The machine and I, talking.
16. It did not change what I was doing. It only made it faster. And showed me possibilities I could never have imagined alone.
17. But first — let me show you what an algorithm actually looks like.

---

## ALGO_STEPS

*(s2 — what an algorithm is, before Game 1)*

1. An algorithm is a set of instructions precise enough that anything can follow them. Every step is defined. Every situation has exactly one answer.
2. A simple one: is it raining? Yes — take an umbrella. No — leave without. Every case covered. No judgment needed once you are following it.
3. The thinking happens before — when you design the rule. After that, anyone can run it. A child, a machine, or me with a pencil on graph paper.
4. Here is the rule you will execute in a moment. Look at a number. If it is odd, make a mark. If it is even, leave the cell empty. That is the whole algorithm.
5. Nothing about the result is decided by taste. The number decides. The rule decides. You simply carry it out — cell by cell, until the grid is full.
6. Let me show you what that feels like.

---

## G1_PRE

*(Game 1 — pre-play narration)*

1. Here is a rule: if the number is odd — place a mark. If the number is even — leave the cell empty.
2. You don't need to hold that in your head — the rule stays on screen the whole time you're working.
3. Twenty-five numbers. Twenty-five decisions. Follow the rule exactly.

---

## G1_POST

*(Game 1 — post-play narration)*

1. You just executed a program.
2. The rule existed before you picked up the pencil. The result followed from it completely.
3. This is where I started — long before I had access to a computer. The algorithm on paper, myself as the processor.

---

## Game 1 — appreciation screen (showAppreciate)

*(One-off strings, not part of a named array — shown right after G1_POST)*

- **eyebrow:** You executed the algorithm
- **title:** Take a moment.
- **sub:** Every mark here was decided by the rule — odd or even — not by you. Yet it looks composed. That is the strange thing about algorithms.
- **yourCap:** Your composition — Game 1

---

## Level transition — Game 1 → Inclinaisons (showLevelTransition)

*(One-off strings)*

- **complete:** Level 1 complete
- **title:** Inclinaisons
- **sub:** 03 — Execute the algorithm

---

## SKETCH_STEPS

*(s3 — explaining Molnár's 1971 working sketch, before Inclinaisons)*

1. This is my actual working sketch from 1971 — graph paper from a Parisian stationery shop. I still have it. Everything you are about to do in the next game comes from this single page.
2. Notice how it is split in two. On the left is the drawing — the finished pattern of tilted lines. On the right is the algorithm that produced it. I always kept them together on one page: the rule and its result, side by side, so I could never pretend the image came from inspiration. It came from the rule.
3. Look at the writing in the top right, in my own hand: 'blancs 20%, 8 inclinaisons 10% pour chaque.' It means: leave 20 percent of the cells blank, and use eight possible line orientations, each appearing 10 percent of the time. Those two sentences are the complete instructions. Nothing else decides the image.
4. Beneath the writing is a compass wheel. I drew the eight orientations and numbered them 1 through 8 — from horizontal, turning step by step toward vertical. Each direction was given exactly the same chance. I did not let any angle dominate, because the moment one does, it becomes a preference — and preference is exactly what I was trying to remove.
5. And below the compass is the lookup table. This is the heart of it: a number comes in, and the table tells you which of the eight orientations to draw. No interpretation. The number maps to an angle, the angle goes in the cell. That mechanical step — number to angle — is the whole algorithm, written out by hand before any computer touched it.
6. But to run it, I needed a number for every single cell — genuine randomness, from outside myself. Not something I calculated.
7. That turned out to be harder than it sounds. In the 1960s you could not simply ask for one. I found two very different sources — I'll show you both in a moment.
8. Then the execution itself: one number, one decision, one line. An arrow from the table to the grid. No hesitation, no stepping back to reconsider. The algorithm does not have second thoughts — and while I followed it, neither could I.
9. I found this liberating, not limiting. I had spent years trying to escape my own taste — the habits I learned in art school, the reflexes of my culture. The rule let me make marks I would never have chosen, and discover they were beautiful anyway.
10. Cell by cell, the grid filled slowly. What emerged was something I could not have pictured in advance — and yet I had specified every part of how it was made. Both things are true at once. That is the puzzle I spent my life inside.
11. So: does a pattern made entirely by rule still carry my signature? I have never fully answered it. The computer helped me ask the question more sharply. It did not answer it for me.
12. Now it is your turn. You will execute exactly this algorithm — roll for a number, read the table, place the line. You will be the machine.

---

## RAND_LINES

*(s3b — the randomness interlude, before Inclinaisons play begins)*

1. To execute the algorithm, I needed random numbers. One per cell. Numbers I could not predict, could not influence, could not unconsciously shape.
2. This was not a trivial problem. In the 1950s and 60s, randomness was expensive. You had to buy it.
3. The RAND Corporation published one million random digits in 1955. A physical book. You looked up a page, picked a row, read the numbers. Scientists, statisticians, military researchers — they all used it. It sat on shelves next to dictionaries.
4. My colleague François Morellet had a cheaper solution. He used a telephone directory. Any sequence of digits that nobody had arranged on purpose would do.
5. What both methods share: the numbers came from outside the system. No formula. No pattern. Pure external input.
6. A computer cannot do this. What computers call 'random' is a formula — a calculation that produces numbers which look unpredictable but follow a precise sequence. Give it the same starting point and it will produce exactly the same numbers every time.
7. This is why we are using dice in this game — a convention we invented to make the process tangible. We do not know exactly how Molnár sourced her numbers. What matters is the principle: something external to the algorithm, something it cannot predict.

---

## INCL_PRE

*(Inclinaisons — pre-play narration)*

1. A number will appear after you roll. Consult the lookup table. Find which range it falls in. Select the corresponding orientation on the right.
2. You don't need to memorize the table, either — it stays open beside the grid for as long as you need it.
3. If the number falls between 81 and 00 — the cell is blank. Press the confirm button. That emptiness is also part of the rule.
4. Roll the dice to generate your first number.

---

## INCL_POST

*(Inclinaisons — post-play narration)*

1. You executed the algorithm. The composition is yours — but it is also not yours.
2. Look at what the rule produced. The distribution is almost even. Not because you controlled it — because the rule guaranteed it.

---

## Inclinaisons — appreciation screen (showAppreciate)

*(One-off strings, shown right after INCL_POST)*

- **eyebrow:** You executed the algorithm
- **title:** This is yours.
- **sub:** You rolled the dice, read the table, placed each line. The distribution is almost even — not because you aimed for it, but because the rule guaranteed it.
- **yourCap:** Your Inclinaisons execution
- **molnar.caption:** Vera Molnár, Inclinaisons, 1971
- **molnar.placeholderText:** [ insert Inclinaisons (1971): name it inclinaisons-1971.jpg ]

---

## ARTWORK_VOICE

*(s5 — artwork reveal, after Inclinaisons)*

1. This is what the rule produces.
2. Not what I imagined — I could not have imagined it. That was the point.
3. I made hundreds of these. Each one different. Each one the same algorithm.
4. The machine imaginaire, finally, made visible.

---

## ENDING_LINES

*(Reflection comparing Game 1 and Inclinaisons)*

1. Look at the two grids. Same rules. Same logic. Different results.
2. You made both of them. But they look different. Why?
3. In the first game, the rule was simple. A binary decision — mark or empty. Your hand followed it exactly.
4. In the second, the rule was more complex. Eight orientations, a lookup table, a pair of dice. More steps between intention and execution.
5. The more steps, the more the algorithm speaks. The more it becomes itself, and less you.
6. This is what I spent my career trying to understand. Not to eliminate the human — but to see it more clearly.
7. I never thought the algorithm was smarter than me. I thought it was more honest about what it did not know.

---

## OD_VOICE

*(s6 — Order & Disturbance, pre-play narration)*

1. In the first games you followed strict rules — odd or even, a number to a direction. The rule decided everything. The result was pure order.
2. And you won't need to memorize this one either — every choice you make here stays visible and adjustable while you work.
3. But pure order is dead. A perfect grid says nothing. My real work began when I asked: what if I disturb the order — not by accident, but by another rule?
4. Start from a perfect grid where every element is identical. Then introduce deviation — and decide how much, and where it falls. The disturbance itself obeys a rule you choose.
5. I was never looking for chaos. I was looking for the exact moment order becomes alive. Now it is your turn to find it.

---

## OD_INSPIRE_BY_LINE

*(Molnár reference-artwork captions, shown alongside specific OD_VOICE lines during narration)*

**Keyed to OD_VOICE line 3 (index 2) — Interruptions:**
- **eyebrow:** Vera Molnár — Interruptions, ca. 1968/69
- **caption:** A field of lines, then some rotated and erased at random. The order is disturbed — never destroyed — and that is what makes it come alive.

**Keyed to OD_VOICE line 4 (index 3) — (Des)Ordres:**
- **eyebrow:** Vera Molnár — (Des)Ordres, 1974
- **caption:** Concentric squares, slightly displaced. The disturbance is never arbitrary: how much, and where it falls, is decided by a rule.

**Keyed to OD_VOICE line 5 (index 4) — Rectangles:**
- **eyebrow:** Vera Molnár — Rectangles, 1977–81
- **caption:** Order loosened by hand. This is the territory you are about to enter — finding the exact amount of disorder that feels alive.

---

## MOLNAR_WORKS

*(Reference artwork titles/notes used in the gallery and inspiration displays)*

1. **Interruptions, ca. 1968/69** — Lines rotated and erased at random.
2. **(Des)Ordres, 1974** — Concentric squares, slightly disordered.
3. **Rectangles, 1977–81** — Collage, 75 × 75 cm.

---

## Order & Disturbance — studio reveal prompt

*(One-off string, set when the game controls are revealed after OD_VOICE finishes)*

- The studio is yours — disturb, save, and download what you like.

---

## Order & Disturbance — first save appreciation (showAppreciate)

*(One-off strings, shown the first time the player saves a version)*

- **eyebrow:** You disturbed the order
- **title:** This is her question.
- **sub:** You started from a perfect grid and let a rule loosen it — exactly what Molnár did. Order, with just enough disorder to feel alive.
- **yourCap:** Your composition
- **molnar.caption:** Vera Molnár, (Des)Ordres, 1974
- **molnar.placeholderText:** [ insert (Des)Ordres (1974): name it desordres.jpg ]

---

## Rule panel text (⚠ lives in `index.html`, not `script.js`)

*(The on-demand "show the rule" panels added to each game's play phase. These were written directly as static markup, not stored in a JS array — flagged here since they're still narrator/instructional voice content.)*

**Game 1 — `#g1-rule-panel`:**
- Odd number → place a mark. Even number → leave the cell empty. That's the whole rule — you never need to remember it, it's always right here.

**Inclinaisons — `#incl-rule-panel`:**
1. Roll the dice — the two digits together make one number, 01 through 00.
2. Find that number's range in the lookup table.
3. Place a line at the orientation the table gives you — or, for 81–00, leave the cell blank.

**Order & Disturbance — `#od-rule-panel`:**
- The Disturbance slider sets how much deviation to introduce. The buttons below it — Uniform, Progressive, Radial, Inverse — set where across the grid that deviation falls.
