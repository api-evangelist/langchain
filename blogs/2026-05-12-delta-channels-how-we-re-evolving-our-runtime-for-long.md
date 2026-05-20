---
title: "Delta Channels: How We’re Evolving our Runtime for Long-Running Agents"
url: "https://www.langchain.com/blog/delta-channels-evolving-agent-runtime"
date: "Tue, 12 May 2026 20:44:08 GMT"
author: ""
feed_url: "https://blog.langchain.com/rss.xml"
---
Long-running agents have a storage problem: checkpointing full state at every step grows at O(N²). DeltaChannel is a new primitive in LangGraph 1.2 that checkpoints only the diff each step and writes full snapshots periodically, keeping storage costs flat as sessions grow longer. It ships by default in Deep Agents v0.6, with no config changes or data migration required.
