<style>

body {
  max-width: 800px;
}

/*a:visited {
  color: rgb(0, 0, 238);
}*/

h2 + p {
  margin-block-start: -0.5em;
}

p + ul {
  margin-block-start: -0.5em;
}

li {
  line-height: 1.25em;
  margin-bottom: 0.25em;
}

</style>

<!-- TODO: Use [] instead of [][] for links for AOC and Project Euler -->
<!-- TODO: Move or copy some of these notes to the relevant READMEs -->

## 2021

Highlights

- **[Crunchspace][crunchspace].** ([code][crunchspace-code]) Clone of an old Flash game `copter.swf`. Made for Crunchbase hackathon. Phaser.

Rubik's cube

- **[swipecube][swipecube].** ([code][swipecube-code]) Rubik's cube sim for mobile. Novel idea: Can swiped gestures on a grid be as easy and intuitive as turning a real cube? Built on top of [keycube](#keycube).
- [Mobile keypad][mobilecube] for [keycube](#keycube). ([code][mobilecube-code])

Chess

- **[Remarkable Rookies][cwda-code]** implementation for the open-source site [vchess]. The Remarkable Rookies are one of three alternate armies for Ralph Betza's [Chess With Different Armies][cwda-wiki]. Sadly, my pull request was not merged because it instead inspired the creator of vchess to implement CWDA himself :)
<!-- - chess engine TODO put it on github -->
- <a name="pchess"></a> [pchess]. Chess move generator (i.e. an implementation of the rules of chess). Incomplete.

[Advent of Code]\: Highlights

- [AOC 2021.16][aoc-2021-16] "Packet Decoder." ([solution][aoc-2021-16-soln])
- **[AOC 2021.19][aoc-2021-19] "Beacon Scanner."** ([solution][aoc-2021-19-soln]) 3D rotations.
- [AOC 2021.20][aoc-2021-20] "Trench Map." ([solution][aoc-2021-20-soln]) Cellular automata with a twist.
- **[AOC 2021.22][aoc-2021-22] "Reactor Reboot."** ([solution][aoc-2021-22-soln]) Intersecting and splitting n-dimensional rectangles.
- **[AOC 2021.23][aoc-2021-23] "Amphipod."** ([solution][aoc-2021-23-soln]) Using Dijkstra's algorithm (I used a [prebuilt implementation][dijkstra]) to find an optimal solution to a simple game.
- [AOC 2021.24][aoc-2021-24] "Arithmetic Logic Unit." ([solution][aoc-2021-24-soln])
- [AOC 2021.25][aoc-2021-25] "Sea Cucumber." ([star 2 leaderboard #55][aoc-2021-leaderboard]) <!-- TODO put solution online -->

[Project Euler]\: Highlights and backtracking search

- [PE60][euler-60] "Prime pair sets." ([solution][euler-60-soln]) This is the [clique problem][cliques].
- **[PE61][euler-61] "Cyclical figurate numbers."** ([solution][euler-61-soln]) Reinvented [backtracking] thanks to this problem! Now I grok it so much better. This got me started on a handful of other backtrackable problems...
- [PE84][euler-84] "Monopoly odds." ([solution][euler-84-soln])
- **[PE96][euler-96] "Su Doku."** ([solution][euler-96-soln]) Backtracking.
- **[PE161][euler-161] "Triominoes."** ([gif][triominoes-gif]) Backtracking. No code: Project Euler requests that its users not publish solutions for problems 101+.
- [N queens]. Backtracking.

Other

- **Drawing [stars] with HTML5 Canvas.** Fun fact: The aesthetically pleasing 7/3 star, used to great effect in Game of Thrones, has a smaller 7/2 star inside it.
- [Mirror piano]. (forked from [Fourhands by Jord Liu][fourhands]; no intent to merge upstream) Just a small change to a friend's open-source project results in a "mirror piano," where higher notes are on the left side, and lower notes are on the right.
- ["Hard mode" for Set][set-hard-mode]. (forked from [Jacob Belanger][set-jacob]) [Set] is a card game that involves finding "sets" of three cards that are "all matching" or "all disjoint" on each of four features. As a beginner to the game, it's hard to see sets with many disjoint features. I made this project because I wanted to see if I could train myself to see these better by drilling them specifically, though I didn't end up using it much.
- [Typeability]. Command-line visualization of how easy/hard it is to type some text in a given keyboard layout through the lens of "How many times do I need to use a finger twice in a row?"
- [typescript-node-starter]. I haven't used this much yet, but I did use it as the basis for [pchess](#pchess) and typescript-web-starter.
- [typescript-web-starter]. I haven't used this at all. I intended to use it for [Crunchspace](#crunchspace), but ended up using [nwtgck's starter][nwtgck-starter] instead.


## 2020

Rubik's cube: keycube and variations

- <a name="keycube"></a> **[keycube].** ([code][keycube-code])
Keyboard-controlled Rubik's cube sim. Existing cube sims often use transparency or other tricks to allow you to see e.g. some of the back of the cube. This is unrealistic, though done for good reason. **Novel idea:** Show only what is visible from the top right corner or the top left corner (these are the two angles we normally see in real life, and we have to choose which we're facing at any time), allowing the user to switch between the two views with a keypress. **Pro:** Somewhat more realistic piece knowledge when solving. **Con:** Additional keypresses needed. **Possible future work:** Animated turns would make it easier to track pieces while solving. For simplicity, I rendered the cube with 2D graphics, but animation would require a proper 3D cube.
- [eocube]. Cube sim for exploring the concept of [edge orientation]. An actual cube with all its pieces and colors is not shown; it is abstracted to just edges and their orientations.
- [asciicube]. ASCII art cube sim.
<!-- - TODO 1x2x3? https://github.com/prendradjaja/keycube/pull/13 -->
<!-- - TODO double-vision? -->

Rubik's cube: 3style and other

- [3style-comm-drills]. Generates drills (as described by [Bertie Longden]) for learning [3-Style]. BYOC (bring your own comms)
- [letter-pair-trainer]
- [solve-time-graph]

[Advent of Code] ([2020 leaderboard #71][aoc-2020-leaderboard]): Highlights and inspired by

- **[AOC 2020.18] "Operation Order."** ([solution][aoc-2020-18-soln]) Inspired a [lunch-n-learn][lnl-asts].
- **[AOC 2020.20] "Jurassic Jigsaw."** ([solution][aoc-2020-20-soln])
- AOC 2019.{2,5,7,9} "Intcode"
- assembler https://gist.github.com/prendradjaja/5392d3cf8faee4738dd511c2f0683391
- **speedcoding-tool**

Other

- **covid-dashboard**
- **just intonation toy** https://gist.github.com/prendradjaja/2f29d8fb14764588da71c83a06bc74d8
- sleep-tracker
- strava userscript https://gist.github.com/prendradjaja/23601f807e8b1ea8cc02c4082758334f
- toc-tracker


[crunchspace]: https://www.ocf.berkeley.edu/~prendra/crunchspace/
[crunchspace-code]: https://github.com/prendradjaja/crunchspace

[swipecube]: https://modest-spence-f997b1.netlify.app/
[swipecube-code]: https://github.com/prendradjaja/keycube/pull/18

[mobilecube]: https://eloquent-swanson-48aa63.netlify.app/
[mobilecube-code]: https://github.com/prendradjaja/keycube/pull/15

[cwda-code]: https://github.com/yagu0/vchess/pull/17
[cwda-wiki]: https://en.wikipedia.org/wiki/Chess_with_different_armies
[vchess]: https://vchess.club/

[pchess]: https://github.com/prendradjaja/pchess

[advent of code]: https://adventofcode.com/
[aoc-2021-16]: https://adventofcode.com/2021/day/16
[aoc-2021-17]: https://adventofcode.com/2021/day/17
[aoc-2021-18]: https://adventofcode.com/2021/day/18
[aoc-2021-19]: https://adventofcode.com/2021/day/19
[aoc-2021-20]: https://adventofcode.com/2021/day/20
[aoc-2021-21]: https://adventofcode.com/2021/day/21
[aoc-2021-22]: https://adventofcode.com/2021/day/22
[aoc-2021-23]: https://adventofcode.com/2021/day/23
[aoc-2021-24]: https://adventofcode.com/2021/day/24
[aoc-2021-25]: https://adventofcode.com/2021/day/25
[aoc-2021-16-soln]: https://github.com/prendradjaja/advent-of-code-2021/tree/main/16--packet-decoder
[aoc-2021-19-soln]: https://github.com/prendradjaja/advent-of-code-2021/tree/19/19--DONTEDIT
[aoc-2021-20-soln]: https://github.com/prendradjaja/advent-of-code-2021/tree/main/20--trench-map
[aoc-2021-22-soln]: https://github.com/prendradjaja/advent-of-code-2021/tree/main/22--reactor-reboot
[aoc-2021-23-soln]:https://github.com/prendradjaja/advent-of-code-2021/tree/23/23--amphipod
[aoc-2021-24-soln]:https://github.com/prendradjaja/advent-of-code-2021/tree/24/24--arithmetic-logic-unitt
[aoc-2021-leaderboard]: https://adventofcode.com/2021/leaderboard/day/25

[project euler]: https://projecteuler.net/
[euler-60]: https://projecteuler.net/problem=60
[euler-61]: https://projecteuler.net/problem=61
[euler-84]: https://projecteuler.net/problem=84
[euler-96]: https://projecteuler.net/problem=96
[euler-161]: https://projecteuler.net/problem=161
[euler-60-soln]: https://github.com/prendradjaja/euler100/tree/master/060--prime-pair-sets
[euler-61-soln]: https://github.com/prendradjaja/euler100/tree/master/061--cyclic-figurate
[euler-84-soln]: https://github.com/prendradjaja/euler100/tree/master/084--monopoly
[euler-96-soln]: https://github.com/prendradjaja/euler100/pull/14
[triominoes-gif]: ./images/triominoes.gif

[dijkstra]: https://python-forum.io/thread-34122.html
[cliques]: https://en.wikipedia.org/wiki/Clique_problem
[backtracking]: https://en.wikipedia.org/wiki/Backtracking

[n queens]: https://github.com/prendradjaja/toys/tree/master/n-queens

[stars]: https://github.com/prendradjaja/toys/tree/master/stars
[mirror piano]: https://github.com/prendradjaja/fourhands/pull/3/files
[fourhands]: https://github.com/jminjie/fourhands

[set-hard-mode]: https://github.com/prendradjaja/set/pull/2
[set]: https://en.wikipedia.org/wiki/Set_(card_game)
[set-jacob]: https://jacobbelanger.com/projects/SET-Card/

[typeability]: https://github.com/prendradjaja/typeability

[typescript-node-starter]: https://github.com/prendradjaja/typescript-node-starter
[typescript-web-starter]: https://github.com/prendradjaja/typescript-web-starter
[nwtgck-starter]: https://github.com/nwtgck/typescript-on-browser-starter

[keycube]: https://prendradjaja.github.io/keycube/
[keycube-code]: https://github.com/prendradjaja/keycube
[cfop]: https://en.wikipedia.org/wiki/CFOP_method
[eocube]: https://prendradjaja.github.io/keycube-experimental/x/eocube/
[edge orientation]: https://www.speedsolving.com/wiki/index.php/Edge_Orientation
[asciicube]: https://prendradjaja.github.io/keycube-experimental/x/ascii/

[3style-comm-drills]: https://github.com/prendradjaja/3style-comm-drills
[letter-pair-trainer]: https://github.com/prendradjaja/letter-pair-trainer-cli
[solve-time-graph]: https://github.com/prendradjaja/solve-time-graph
[bertie longden]: https://www.youtube.com/watch?v=ciH9l6GNk4w
[3-style]: https://www.speedsolving.com/wiki/index.php/Beyer-Hardwick_Method

[aoc-2020-leaderboard]: https://adventofcode.com/2020/leaderboard
[aoc 2020.18]: https://adventofcode.com/2020/day/18
[aoc 2020.20]: https://adventofcode.com/2020/day/20
[aoc-2020-18-soln]: https://github.com/prendradjaja/advent-of-code-2020/tree/master/18--operation-order
[aoc-2020-20-soln]: https://github.com/prendradjaja/advent-of-code-2020/tree/master/20--jurassic-jigsaw
[lnl-asts]: https://github.com/prendradjaja/ast-lnl
