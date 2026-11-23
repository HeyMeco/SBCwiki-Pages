---
weight: 9
title: "KDiskMark"
description: KDiskMark sequential and random disk rankings.
summary: Sequential and random read and write speeds, in MB/s.
bookToC: false
---

# KDiskMark

A Linux disk benchmark in the style of CrystalDiskMark, built on fio. SEQ1M tests read and write 1 MiB blocks in order, RND4K tests use random 4 KiB blocks; Q is the queue depth and T the thread count. Higher is better.

5 passes of 1 GiB. Read and write for each test share one scale, in MB/s.

{{< benchmark-charts kind="board" benchmarks="kdiskmark-seq1m-q8t1,kdiskmark-seq1m-q1t1,kdiskmark-rnd4k-q32t1,kdiskmark-rnd4k-q1t1" >}}
