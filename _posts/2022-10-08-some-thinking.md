---
layout: post
title:  "Some thinking about the River"
author: "Murasame"
---

# how River prevent the attack of the attacker

The River's data is real-time stream, we cannot wait as normal blockchain for the block to be confirmed. So we need some consensus algorithm to prevent the attacker from attacking the River.

# POW

The stream is not like the normal data, it need low latency or high throughput.
> **Why 'or' but not 'and'?**
> 
> On the most of the scenario, we don't need low latency or high throughput at same time (gaming need low latency udp but not high throughput, video need mid latency and high throughput). we can make River have two type of node, one for low latency, one for high throughput.
The River's node should can be host anyone to extend the network.

So we have to pay the hoster for the stream. We need POW to pay the hoster.

# POS

We need POS for the hoster to guarantee the hoster's node. They need this mechanism to proof they are not want to cheating.

# BFT
We should select out some trustworthy node for verify the work.

> **What we verify? And how?**
> 
> we don't know when the stream end, But we can sample the stream to verify the work. We can use the hash of the sample to verify the work. 

# Conclusion

So we decide to implement POW + POS + BFT on River Network.