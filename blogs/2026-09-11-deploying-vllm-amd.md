---
title: "Deploying vLLM AMD"
url: "https://community.vastdata.com/t/deploying-vllm-amd/2066#post_1"
date: "2026-09-11"
author: "@jason.massae Jason Massae"
feed_url: "https://community.vastdata.com/posts.rss"
---
As long-context LLM inference scales, GPU High Bandwidth Memory (HBM) becomes the primary bottleneck as the Key-Value (KV) cache grows linearly. Pairing vLLM’s native OffloadingConnector with host DRAM and VAST Data spills KV from GPU → CPU → NFS, bypassing GPU memory limits and cutting warm Time-To-First-Token (TTFT) when prefixes hit the CPU/FS tiers. Read more: Deploying vLLM AMD Let us know if you have any questions
