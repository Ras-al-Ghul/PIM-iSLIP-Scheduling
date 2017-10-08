# Packet Switch Scheduling Algorithms

Two packet scheduling algorithms - **Parallel Iterated Matching (PIM)** and **iSLIP** have been implemented.

## Files
- `pim.py` - Parallel Iterated Matching (PIM)
- `islip.py` - iSLIP implementation. More information about the algorithm here: http://dl.acm.org/citation.cfm?id=310896

## Inputs
- `uniform_input` - 8x8 Uniform traffic
- `fullskew_input` - 4x4 Fullskew traffic
- `fullcycle_input` - 8x8 FullCycle traffic
- `input4` - 3x3 Input traffic
- `input5` - 4x4 Input traffic

## To run  
`./pim.py < input_file` to run PIM on the specified input file.  
`./islip.py < input_file` to run iSLIP on the specified input file.  
**NOTE:** Needs a `pip install tabulate` first.

Both the scripts display the workout of the given scheduling problem using the algorithm. Each iteration of each round with Request Phase, Grant Phase and Accept Phase is displayed, and this also displays the round based statistic at the end (total number of rounds taken for the given input, and iterations per round)
