# Reddit Demand Research Assistant

Personal, **read-only** research helper that uses the [Reddit Data API](https://www.reddit.com/dev/api) (OAuth) to study public discussions and surface unmet user needs.

## Purpose

Help Redditors indirectly by turning public posts and comments into clearer product priorities: recurring pain points, feature requests, and open questions—so builders can ship things people actually ask for.

## What it does

- Authenticate with a registered OAuth client and a descriptive User-Agent
- Search and read **public** posts and comments in selected subreddits
- Summarize themes (pain points, requests, questions) for personal product research
- Respect Reddit rate limits and API terms

## What it does **not** do

- Post, comment, vote, or send DMs
- Moderate communities
- Scrape without OAuth or exceed rate limits
- Retain content after it is deleted on Reddit
- Train AI/ML models on Reddit data
- Resell or redistribute Reddit data

## Planned stack

- Language: Python (or similar)
- Auth: Reddit OAuth2
- Access: official Data API only
- Storage: short-lived local notes; purge deleted content promptly

## Subreddits

Chosen per research topic (examples: `r/startups`, `r/SaaS`, and niche product communities). No mass cross-posting.

## Operator

- Reddit account: `/u/Downtown-Act-9950`
- Contact: `zevinchen1993@gmail.com`

## Status

Early planning / awaiting Data API access approval. Source and scripts will live in this repository as the project progresses.

## Compliance

Use is subject to Reddit’s [Developer Terms](https://www.redditinc.com/policies/developer-terms), [Data API Terms](https://www.redditinc.com/policies/data-api-terms), and [Responsible Builder Policy](https://support.reddithelp.com/hc/en-us/articles/42728983564564-Responsible-Builder-Policy).
