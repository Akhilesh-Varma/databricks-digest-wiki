---
type: story
story_id: hn_48402970
episode_date: 2026-06-05
rank: 2
source: hacker_news
url: "https://www.earthmover.io/blog/virtual-zarr/"
title: Cloud-optimizing the GOES-16 satellite data archive without copying data
quality_score: 0.626
content_hash: "sha256:b88feb1b5e6fe2d95d844683ba1d4b09f1253abc1e34d44ba7537006cce4fad3"
concepts: [virtual-zarr, virtualizarr, icechunk, arraylake, zarr, analysis-ready-cloud-optimized-arco, goes-16, cloud-object-storage, lift-and-shift-migration]
companies: [earthmover, usgs, noaa, nasa, ecmwf]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-05 10:17:42.955000"
tags: [story, source/hacker-news]
---

## Summary
Earthmover demonstrates how to cloud-optimize the GOES-16 satellite imagery archive using VirtualiZarr, Icechunk, and Arraylake without duplicating or modifying the original files. The core problem is that many scientific file formats predate cloud object storage and perform poorly in that environment, yet data providers face budget and policy constraints that prevent full conversion. Virtual Zarr stores solve this by providing cloud-optimized access that references the original files via HTTP range requests, avoiding the cost of storing petabyte-scale datasets twice. Major public agencies such as NOAA, NASA, USGS, and ECMWF are pushing for Analysis-Ready, Cloud-Optimized data, making this approach increasingly relevant. The result is a single virtual Zarr store covering the entire GOES-16 archive with no data copying required.

## Key claims
- VirtualiZarr, Icechunk, and Arraylake were used to create a virtual Zarr store for the GOES-16 archive without copying any data.
- Many scientific file formats predate cloud object storage by over 15 years and are poorly suited for it.
- A 'lift and shift' migration uploads data to cloud storage in original formats, providing cloud access but few cloud-native benefits.
- Duplicating petabyte-scale datasets to convert them to cloud-optimized formats can double storage costs.
- Virtual Zarr stores enable cloud-optimized access to archival files by referencing their contents over HTTP without modification.
- Agencies including USGS, NOAA, NASA, and ECMWF are championing Analysis-Ready, Cloud-Optimized (ARCO) data stores.

## Source
- **Origin:** hacker_news
- **URL:** <https://www.earthmover.io/blog/virtual-zarr/>

## Related
[[concepts/virtual-zarr|virtual-zarr]] · [[concepts/virtualizarr|virtualizarr]] · [[concepts/icechunk|icechunk]] · [[concepts/arraylake|arraylake]] · [[concepts/zarr|zarr]] · [[concepts/analysis-ready-cloud-optimized-arco|analysis-ready-cloud-optimized-arco]] · [[concepts/goes-16|goes-16]] · [[concepts/cloud-migration|cloud-migration]] · [[concepts/object-storage|object-storage]] · [[concepts/cloud|cloud]] · [[companies/earthmover|Earthmover]] · [[companies/usgs|USGS]] · [[companies/noaa|NOAA]] · [[companies/nasa|NASA]] · [[companies/ecmwf|ECMWF]] · [[episodes/2026-06-05|2026-06-05]]
