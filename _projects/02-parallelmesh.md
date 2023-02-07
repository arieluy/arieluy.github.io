---
title: "Parallel Tetrahedral Mesh Generation"
excerpt: "Parallelize the fast Tetrahedral Meshing Algorithm to speed up 3D mesh generation."
header:
  teaser: /assets/images/projects/yoda.png
gallery:
  - url: /assets/images/projects/yoda2.png
    image_path: /assets/images/projects/yoda2.png
  - url: /assets/images/projects/yoda.png
    image_path: /assets/images/projects/yoda.png
---

*December 2020*

*Final project for [Parallel Computer Architecture](http://www.cs.cmu.edu/afs/cs/academic/class/15418-f20/www/) class, with Alex Havrilla.*

{% include gallery layout="half" caption="Input triangular mesh and output tetrahedral mesh"%}

Tetrahedral meshing is the process of converting a 3D surface triangle mesh into a tetrahedral mesh of the interior volume. We added parallelism to the triangle insertion section of the [fast Tetrahedral Meshing Algorithm](https://yixin-hu.github.io/ftetwild.pdf){:target="_blank"}, using shared-memory parallelism on high-core CPU machines. We tested various partitioning schemes experimentally and wrote a [paper](https://arieluy.github.io/fTetWild/ParallelFinalReport.pdf){:target="_blank"} analyzing the results. \[[presentation](https://youtu.be/4iJxYMom9to){:target="_blank"}\] \[[GitHub](https://github.com/arieluy/fTetWild/){:target="_blank"}\]