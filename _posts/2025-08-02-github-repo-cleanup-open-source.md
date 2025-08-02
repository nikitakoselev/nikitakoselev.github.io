---
layout: post
title: "My First Open Source Tool: GitHub Repo Cleanup"
date: 2025-08-02 10:00:00 +0300
---

Have you ever heard the phrase _"Clean your room first"_ before starting something big?

That's exactly how I kicked off this blog and my AI learning journey — by cleaning up my **cluttered GitHub profile**.

---

## Problem: 325 Forked Repos

At some point, I got obsessed with forking every interesting repo I came across.  
Eventually, it became a mess — **325 repos**, most untouched, all clogging my dashboard.

Manually deleting them? Absolutely not.

![GitHub profile with cluttered forks](/assets/images/image1.png)

---

## My Rule: Solve My Problems With Code

I believe in learning by solving your own problems — and this was the perfect case.  
So I set out to write a small **Python tool** that would:

- List all my repositories
- Show basic info + readme preview
- Ask me which ones to delete
- Allow marking protected repos (via a config file)
- Batch delete confirmed ones
- Support safer actions: **archive** or **make private**

---

## Building It: On an Old Tablet, With AI Help

I built everything on a **Surface tablet** running Windows 10 — far from ideal, but it worked.

I used:
- **Visual Studio Code**
- **GitHub Copilot (free tier)**
- **ChatGPT** to structure and debug
- A lot of coffee

![Setting up Copilot in VS Code](/assets/images/image2.png)

---

## Bugs? Of Course There Were Bugs

The tool didn’t work at first — common story.

I hit problems like:
- Missing GitHub username during API calls
- Repos not deleting due to permission errors
- Debugging token storage

![Early error during repo deletion](/assets/images/image4.png)

But I fixed them iteratively. That’s what building looks like.

---

## Iterating: Batch Delete & Safeguards

Once the basics worked, I needed batch deletion. So I added it.

![Batch delete workflow](/assets/images/image6.png)

I also made sure the tool doesn’t delete:
- Starred repos
- Whitelisted names in a config
- Anything without confirmation

And instead of just deleting, it now offers to:
- **Archive** the repo
- **Make it private**

Much safer.

---

## Sharing It as Open Source

Eventually, I decided to open source it. Why?

Because:
- It helped me
- Others have the same problem
- It’s a simple but empowering first project

👉 [Check it out on my GitHub](https://github.com/nikitakoselev)

---

## What I Learned

- **Solve your own pain first**
- **Start tiny — grow through usage**
- **Don’t wait until you’re an expert**
- **Ship something that helps you — and share it**

---

## What's Next

This is just the first of many experiments.  
Next up: building small automations and AI workflows to create **alternative income streams** — and documenting all of it right here.

**The blog, like the projects, will evolve as I do.**

Thanks for reading.
