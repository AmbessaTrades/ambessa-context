<!-- copied from the Juju repo: runs/scriptlab/storyboard/gaps.md, last changed 03:01 EAT, 25 Nov 2026. Private lines removed. Do not edit here. -->
# The ten engine primitives that would let Juju draw the most moves

Built by tools/build.py; every number is checked again by check.py. Hero seconds are Measured over a Judged match of move to row. A film counts when a blind second reader, given the frames and the closed list, named the move (tools/reads.json).
Order: hero seconds (clips, borrowed pages and the paid board left out) over the largest (72.6) plus films over the largest (5), equal weight (the weight is Judged).

The hero has 434.3 s that are its own argument (kept or bent rows). Of those the offered worlds can say 54.055 s today in their own material (12.4 percent, Measured over a Judged match). With clips and the paid board counted too: 57.058 of 780.237 s, and 61.521 s more in held worlds.

| # | Primitive | Moves it opens | Hero s | Hero s with clips and paid board | Films | Skeleton beats where one of its moves is first or second | Drawable hero s once this and those above land | Verb in design/house/BUILD.json |
|---|---|---|---|---|---|---|---|---|
| 1 | plain_stage | bare_ground, list_answered, number_alone, word_alone | 47.7 | 47.7 | 4 | 23 of 81 | 101.8 (23.4 percent of 434) | none |
| 2 | star_depth | grow_from_centre, tip_to_depth | 72.6 | 72.6 | 2 | 3 of 81 | 174.4 (40.2 percent of 434) | fly_aside |
| 3 | first_back | come_back | 36.1 | 36.1 | 4 | 15 of 81 | 210.5 (48.5 percent of 434) | first_back |
| 4 | height_mesh | stand_up | 31.6 | 31.6 | 4 | 2 of 81 | 242.1 (55.7 percent of 434) | stand_up |
| 5 | layer_lift | lift_paint, lies_on_nature | 45.7 | 45.7 | 3 | 7 of 81 | 287.8 (66.3 percent of 434) | lift |
| 6 | still_run | crowd_of_same, words_on_painting, open_to_real, wider_than_frame | 15.1 | 79.7 | 5 | 13 of 81 | 302.9 (69.8 percent of 434) | none |
| 7 | ties_layer | ties | 38.2 | 48.0 | 3 | 6 of 81 | 341.1 (78.5 percent of 434) | none |
| 8 | time_front | how_far_by_day | 0 | 0 | 3 | 3 of 81 | 341.1 (78.5 percent of 434) | none |
| 9 | split_view | side_by_side | 11.3 | 13.3 | 2 | 2 of 81 | 352.4 (81.1 percent of 434) | none |
| 10 | nested_units | share_of_one, level_below | 23.1 | 23.1 | 1 | 2 of 81 | 375.5 (86.5 percent of 434) | none |

## What each one is, where it goes

1. **plain_stage**: a stage that shows the ground alone, one number, one to three words, or a short list that fills as it is said, on the film's own plain ground or its bare sky. Where: catalog.rs: stage plain_ground with events word, item, clear; draw.rs type_at on the look's bed. Films: 7prMGQnO8n4, J0wWNytEXS4, ZgpMtombn9A, bjEr7L2Rj9s.
2. **star_depth**: real catalogue stars as points at true distances, seen from any side and flown through. Where: worlds/stars.rs projecting x, y, z through fly.rs Flight; catalog.rs stage star_depth with events grow, aside, sink. Films: G4w-a8NgnnQ, J0wWNytEXS4. Also helps sink_in, true_gap, bare_ground (51.6 hero s of those moves, most of them counted elsewhere).
3. **first_back**: an earlier state of the same table drawn again as a picture, with one layer off. Where: check.rs refuses a row at or before one reached; worlds/mod.rs At row -1. A copy of the table under another id would bring the first picture back unchanged (read in check.rs line 122, untried). Films: 5gbgKYMEySI, DVmoKR6QI5Y, J0wWNytEXS4, ZgpMtombn9A.
4. **height_mesh**: a real region raised as a mesh with side walls, or cut as a profile, true scale times a factor on screen. Where: worlds/map.rs Cam::see already takes a height (0 today); juju-gather relief.rs fetches tiles. Films: 7prMGQnO8n4, J0wWNytEXS4, bjEr7L2Rj9s, v_wjyuKPJXc.
5. **layer_lift**: each layer of a map (colour, names, frontiers, towns, rivers, relief) leaves or comes back behind one front. Where: worlds/map.rs Map::draw: an amount for each layer; towns and rivers from Natural Earth. Films: 7prMGQnO8n4, J0wWNytEXS4, gY3F1AQpow0. Also helps come_back (36.1 hero s of those moves, most of them counted elsewhere).
6. **still_run**: one real still whole and full frame with a slow push or a travel across it, its exact quotation on the clear side when it has one, and a run of stills on an even beat. Where: worlds/archive.rs: a still as a clip, Use::Cut or Use::Room at 1920 wide; event cut already exists. Films: ABWrP69A6mE, G4w-a8NgnnQ, J0wWNytEXS4, ZgpMtombn9A, qxAIE8s9-NA. Also helps exhibit (61.5 hero s of those moves, most of them counted elsewhere).
7. **ties_layer**: a persistent set of sourced lines between places that grow in order, stay, and follow a moved end. Where: worlds/map.rs after the journeys: table.rs MapT.ties; same in worlds/route.rs. Films: 7prMGQnO8n4, J0wWNytEXS4, fUHHdx0N8kQ.
8. **time_front**: a front of equal travel time over real land or a road network, with its clock. Where: worlds/map.rs: a time for each cell in place of reach. Films: 7prMGQnO8n4, LqvlFsTaZgE, v_wjyuKPJXc.
9. **split_view**: one table drawn in two states, half a frame each, same view. Where: worlds/mod.rs frame: two Places into two halves. Films: ABWrP69A6mE, J0wWNytEXS4.
10. **nested_units**: the units inside a chosen outline come up at the next level, and one unit can be ringed with its share. Where: table.rs: shapes by level; worlds/map.rs draws the second level inside one id. Films: J0wWNytEXS4.

How far the order rests on one film: with any one film other than the hero taken away, 7 of the ten stay. Those that enter or leave: drain, nested_units, split_view, time_front, vector_edges. Measured arithmetic over Judged matches.

Rows the engine cannot say in their own form count against the primitive they wait for: star_depth takes 77.4, 83.7, 136.0 and 374.0 s (a gap, a push and a pointer among stars); layer_lift takes 454.6 and 623.2 s (a push into drawn land whose roads and woods are not in our base).

## Not in the ten

- vector_edges: trace_the_edge, then_now; 5.3 hero s, 2 films. Frontiers drawn from the rings as lines, in part or whole, for any dated step. BUILD verb then_now.
- drain: one_left; 15.1 hero s, 1 films. Every colour but one goes to grey, or all things but one leave. BUILD verb drain.
- true_size: draw_it_true; 14.0 hero s, 1 films. Bodies ease from the size they are drawn at to their true size in the same view.
- look_by_scene: ground_flip; 12.1 hero s, 1 films. A scene names its own ground, and a cut may be one clean frame with no dip to black. BUILD verb flip.
- arrow_test: test_directions; 8.7 hero s, 1 films. Arrows of measured length and bearing on the map plane that grow, stay or pull back.
- point_count: count_is_things; 3.4 hero s, 1 films. Sourced points lit in order whose number is the counter. BUILD verb count_real.
- night_base: night_lights; 0 hero s, 1 films. A second base picture on the same bounds mixed in by an event. BUILD verb night.
- Candidates count nowhere: spread_thin waits for point_count and for a frame on real land; wrong_move waits for shape_move and for a frame on real land.

## Skeletons that may be offered today

Offered pairs: 0 of 20 (rule in choose.json offer_rule). Not offered in any system: dated-run, group-chat, map-chronicle, odd-record, old-sources, real-reason, runaway-counter, scale-ladder, survival-ledger, wrong-picture.

A move counts for a beat only when the maker ranked it and a blind reader named it.

| Skeleton | System | Seconds with a move | Beats with a move | By one maker alone | Beats with nothing and no legal hold |
|---|---|---|---|---|---|
| dated-run | near-worlds | 0.062 | 1 of 8 | 2 of 8 | sign, step, blow, wide, second, count, after |
| dated-run | moving-borders | 0.462 | 3 of 8 | 7 of 8 | rule, step, blow, second, count |
| group-chat | near-worlds | 0.0 | 0 of 8 | 0 of 8 | entry, want, move, join, turn, cost, deal, back |
| group-chat | moving-borders | 0.715 | 3 of 8 | 6 of 8 | entry, want, join, cost, back |
| map-chronicle | near-worlds | 0.0 | 0 of 8 | 2 of 8 | name, rule, first_map, event, turn, worst, answer, last_map |
| map-chronicle | moving-borders | 0.884 | 5 of 8 | 8 of 8 | name, rule, last_map |
| odd-record | near-worlds | 0.0 | 0 of 8 | 0 of 8 | find, doubt, source, inside, far_back, match, answer, left_open |
| odd-record | moving-borders | 0.0 | 0 of 8 | 2 of 8 | find, doubt, source, inside, far_back, match, answer, left_open |
| old-sources | near-worlds | 0.0 | 0 of 6 | 0 of 6 | known, turn_in, source, gather, practice, land |
| old-sources | moving-borders | 0.0 | 0 of 6 | 0 of 6 | known, turn_in, source, gather, practice, land |
| real-reason | near-worlds | 0.0 | 0 of 8 | 0 of 8 | puzzle, frame, stage, piece, turn, piece2, reckoning, echo |
| real-reason | moving-borders | 0.165 | 2 of 8 | 5 of 8 | puzzle, frame, piece, turn, piece2, reckoning |
| runaway-counter | near-worlds | 0.649 | 2 of 9 | 3 of 9 | flash, ask, normal, turn, loss, edge, close |
| runaway-counter | moving-borders | 0.0 | 0 of 9 | 2 of 9 | flash, ask, normal, climb, turn, beyond, loss, edge, close |
| scale-ladder | near-worlds | 0.727 | 5 of 8 | 6 of 8 | question, turn, home |
| scale-ladder | moving-borders | 0.0 | 0 of 8 | 0 of 8 | object, question, rung, turn, near, home, limit, close |
| survival-ledger | near-worlds | 0.137 | 1 of 11 | 3 of 11 | number, cause, first_loss, choice, need, stranger, rival, worst, last_day, ask |
| survival-ledger | moving-borders | 0.137 | 1 of 11 | 5 of 11 | number, cause, first_loss, choice, need, stranger, rival, worst, last_day, ask |
| wrong-picture | near-worlds | 0.048 | 1 of 7 | 1 of 7 | ask, expected, test, objection, answer, harder |
| wrong-picture | moving-borders | 0.054 | 1 of 7 | 3 of 7 | ask, break, test, objection, answer, harder |

## Against design/house/BUILD.json (eight verbs, ranked there by gain and safety, not by seconds)

- Verbs of BUILD.json in this ten: fly_aside, first_back, stand_up, lift.
- BUILD verbs outside the ten: then_now, drain, night, count_real. They are cheap or safe; they open few hero seconds.
- In this ten and not a BUILD verb: plain_stage, still_run, ties_layer, time_front, split_view, nested_units. BUILD's `flip` note (the ground swap) is look_by_scene here.
- BUILD.json says roads are not on disk. ties_layer needs a sourced list of ties; runs/scriptlab/films/7prMGQnO8n4 names an open Roman road set (seen at 137 s, its licence not checked).
- The rule of READ-FIRST holds: runs/harvest ENGINE.md, when it lands, orders the build. This file is evidence for that order.
