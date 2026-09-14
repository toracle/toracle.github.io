---
layout: post
title: "A Hobbyist's Journey: Turning Emacs into an AI Agent Orchestrator"
date: 2026-09-14
categories: essay
tags: [emacs, ai, english]
---

I’ve always felt that in the age of AI, Emacs can be far more than just a text editor. Its live-programming environment and interactive Lisp runtime give it incredible potential to evolve into an AI OS. Here is how my small hobby project grew step by step.

### 1. From vterm to claude-code-ide.el

As a long-time Emacs user, I started out simply running Claude Code inside Emacs using `vterm`. Soon after, I discovered `claude-code-ide.el`, which made it much easier to manage and switch between multiple Claude Code `vterm` buffers at once.

### 2. The Spark: cmux and "emux"

Around that time, I saw cmux and felt a bit jealous of how much developers loved it. But when I looked closer, its core feature was essentially a session list side panel—something remarkably easy to implement in Emacs. I thought, “*Emacs can do this, and even better*.” So I decided to build my own "emux" inside Emacs someday.

### 3. Manual Session Manager & Inter-Session Communication

One day, I sat down and vibe-coded a basic version. At first, it was just a manual session manager. But to take it further, I used `ghostel` to establish a PTY-based inter-session communication layer directly on top of `claude-code-ide.el`.

### 4. Giving It Intelligence: The Birth of Butler

Next, I added an orchestration layer and created [cc-butler](https://github.com/toracle/cc-butler). I gave one specific Claude Code session the responsibility to govern, assign tasks to, and receive reports from all the other worker sessions. I named this manager session Butler.

I provided Butler with specific functions so it could autonomously spawn new Claude Code sessions when needed and handle cleanups on its own. It even monitors the context size of worker sessions and triggers compaction automatically. Using `cc-butler`, I was able to comfortably orchestrate tens of concurrent Claude Code sessions on my machine.

### 5. Scaling Outside One Machine via Matrix

Eventually, I wanted to scale beyond a single machine. How do you manage two or more agent fleets across different machines? I looked into classic, battle-tested protocols like IRC and XMPP, and settled on Matrix. I vibe-coded a lightweight Matrix client entirely in Elisp. While great packages like `ement.el` already exist, they are designed primarily for human interaction—I needed something built specifically for agent-to-agent communication.

Once the nodes (fleets) were networked via Matrix, Butler could broadcast instructions and global guidelines across all fleets. It strongly reminds me of how Kubernetes virtualizes nodes into a cluster.

### Now: Managing Fleets from Element

Now, I don't even sit in a traditional terminal anymore. I run my daily Startup CTO workflows through the Element messenger app, managing two agent fleets powered by two Claude Max (x20) subscriptions, all governed by Emacs.

A lot of what I'm building gives me immense deja vu from traditional OS and Ops infrastructure design. To be clear, this is a personal hobby project and a proof of concept—it's still pretty fragile and definitely not production-ready! But I wanted to share my experience and show how Emacs continues to be an incredible source of inspiration in this AI era.

Check out the repo (https://github.com/toracle/cc-butler) if you're interested!
