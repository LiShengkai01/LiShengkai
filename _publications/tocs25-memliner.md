---
title: "Lining up Garbage Collection and Application for a Far-Memory-Friendly"
collection: publications
category: manuscripts
permalink: /publication/tocs25-memliner
excerpt: #'This paper is about the number 1. The number 2 is left for future work.'
date: 2025-6-25
venue: 'Transactions on Computer Systems, accepted, awaiting publication'
slidesurl: #'http://academicpages.github.io/files/slides1.pdf'
paperurl: #'http://academicpages.github.io/files/paper1.pdf'
bibtexurl: #'http://academicpages.github.io/files/bibtex1.bib'
citation: #'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

Aligning the memory accesses of the application and GC threads to reduce resource competition.

###### Abstract

Far-memory techniques that enable applications to use remote memory are increasingly appealing in modern data centers, supporting applications’ large memory footprint and improving machines’ resource utilization. Unfortunately, most far-memory techniques focus on OS-level optimizations and are agnostic to managed runtimes and garbage collections (GC) underneath applications written in high-level languages. With different object-access patterns from applications, GC can severely interfere with existing far-memory techniques, breaking remote memory prefetching algorithms and causing severe local-memory misses. 

We developed MemLiner, a runtime technique that improves the performance of far-memory systems by aligning memory accesses from application and garbage collection threads so that they follow similar memory access paths, thereby (1) reducing the localmemory working set and (2) improving remote-memory prefetching through simplified memory access patterns. We implemented MemLiner in two widely-used GCs in OpenJDK: G1 and Shenandoah. Our evaluation with a range of widely-deployed cloud systems shows MemLiner improves applications’ end-to-end performance by up to 3.3× and reduces applications’ tail latency by up to 220.0×.
