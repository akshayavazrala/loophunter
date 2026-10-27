# Loop Hunter: Flow Graph Game

Flipped-classroom activity.

**Before class:** students open `index.html` and read the "Before class: study" tab (flow graphs, dominators, back edges, loop headers, natural loops, irreducible graphs).

**In class:** switch to "In class: play". Four levels, each with questions on:
entry node, back edges, loop header(s), loop body (natural loop).

## Run
Double-click `index.html`. No install, no internet needed.

## How answers are computed
Dominators are computed with the iterative dataflow algorithm; back edge = edge u->v where v dominates u; natural loop = v plus nodes that reach u without passing v.

## Add your own graph
Edit the `LEVELS` array in `index.html`: nodes `[id,x,y]` (first node is the entry), edges `[from,to,optionalCurve]`, and a list of questions (`entry`, `back`, `header`, `body` with `h`).

## Scoring
10 points per question, -3 per wrong attempt, -3 if a hint is used (minimum 2).
