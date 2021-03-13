---
layout: post
title: Single cell Gene Regulatory Network analysis with `pySCENIC`
---
<div style="text-align: justify">

## Gene Regulatory Networks with sc/snRNA-Seq data


I have been interested on [Gene Regulatory Networks](https://www.frontiersin.org/articles/10.3389/fcell.2014.00038/full) (GRN) since my molecular biology days, and this interest got augmented once I started working with single cell datasets. <br>  

## Why `pySCENIC`?

Many tools have been released to reconstruct GRNs, but my favourite by far is [SCENIC](https://www.nature.com/articles/s41596-020-0336-2) in its fastest implementation: [pySCENIC](https://github.com/aertslab/pySCENIC). I have managed to run `pySCENIC` on a dataset <br> of 150K cells using all ~33K genes on a OpenStack instance with 20 cores and 256 GiB of RAM. This job took about 8 hours in this set up (so I left it running overnight).    

Although I think `pySCENIC` is really nice tool, sometimes there are some frustrating dependency-related issues, and once you have the final results, following up with<br> downstream analysis is not really evident. Here I will share my `pySCENIC` setup and some ideas on how to further analyse `pySCENIC` results, which I have gathered along <br> the way from my own experience and from other colleages. 




