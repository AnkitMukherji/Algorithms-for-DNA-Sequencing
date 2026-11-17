# Algorithms for DNA Sequencing

A Python/Jupyter collection exploring the computational foundations of read analysis, sequence matching, alignment, and genome assembly.

## Folder guides

- [DNA sequencing algorithm exercises](Exams/README.md)

## Notebook pathway

| Stage | Starting notebooks | Concepts |
| --- | --- | --- |
| Sequence and read handling | [String basics](1.01_StringBasics.ipynb), [DNA strings](1.02_ManipulatingDNAStrings.ipynb), [reference parsing](1.03_ParsingRefGenome.ipynb), [sequencing reads](1.04_WorkingWithSequencingReads.ipynb), [positional read analysis](1.05_AnalyzingReadsByPosition.ipynb) | Representations, parsing, and read-level summaries |
| Exact and approximate matching | [Naive matching](1.06_NaiveExactMatching-MatchingArtificialReads.ipynb), [real reads](1.07_NaiveExactMatching-MatchingRealReads.ipynb), [Boyer–Moore](2.01_BoyerMoore.ipynb), [substring indexing](2.02_SubstringIndex.ipynb), [pigeonhole matching](2.03_ApproximateMatching_pigeonhole.ipynb) | Search efficiency, indexing, and mismatch tolerance |
| Alignment and overlaps | [Edit distance](3.01_EditDistanceDP.ipynb), [global alignment](3.02_GlobalAlignment.ipynb), [overlaps](3.03_FindingOverlaps.ipynb), [all overlaps](3.04_FindingAllOverlaps.ipynb) | Dynamic programming and overlap discovery |
| Assembly | [Shortest common superstring](4.01_ShortestCommonSuperstring.ipynb), [greedy assembly](4.02_GreedySCS.ipynb), [de Bruijn graphs](4.03_DeBruijn.ipynb) | Optimization, heuristics, and graph representation |

## Use

Open the numbered notebooks in a Python/Jupyter environment and work through them in order. Inspect imports and input-file paths before execution. Notebook examples may depend on external sequencing/reference files; this repository has no documented, tested one-command environment setup.

These notebooks are retained as learning and algorithm-development work. Check exercise instructions and attribution before reusing course-derived material.

## Interpretation and tradeoffs

Compare correctness, computational cost, and failure modes across methods. Exact matching assumes no sequencing error; approximate matching and alignment introduce explicit error models or scoring rules. Greedy superstring assembly illustrates a heuristic, while repeat structure can leave multiple plausible reconstructions.

Related: [bioinformatics algorithms organized by biological question](https://github.com/AnkitMukherji/Bioinformatics-Algorithms).
