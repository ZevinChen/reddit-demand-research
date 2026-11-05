# Reddit Community Needs Assistant

Personal, **non-commercial**, **read-only** developer tool that uses the official [Reddit Data API](https://www.reddit.com/dev/api) (OAuth) so I can build products that solve problems Redditors already talk about in public threads.

This is **not** academic research and is **not** an application to the Reddit for Researchers (RFR) program. It is a personal developer workflow for product discovery and prioritization.

## Purpose / benefit for Redditors

I use public discussions only to understand recurring problems, feature requests, and open questions, then ship tools or content that address those needs. Redditors benefit when products match what they already ask for. The tool never posts, comments, votes, DMs, or otherwise engages on Reddit.

## Scope

- **Access:** OAuth client for the official Data API only (no scraping, no unofficial endpoints)
- **Actions:** read-only — search/list public posts and comments in a small set of subreddits relevant to each product idea
- **Write actions:** none (no submit, edit, vote, message, or moderation)
- **Audience:** me only (personal tool; not a multi-tenant SaaS; no redistribution of Reddit data)
- **Commercial use of Reddit data:** none — I will not sell, license, share, or commercialize Reddit data, and I will not use it for ads targeting or to train AI/ML models
- **Rate limits:** stay within free-tier limits (e.g. 100 QPM) and honor `X-Ratelimit-*` headers
- **User-Agent:** descriptive string including platform, app id, version, and `/u/Downtown-Act-9950`
- **Deleted content:** purge stored post/comment bodies and author identifiers promptly when content or accounts are deleted on Reddit (target within 48 hours)
- **Privacy:** no inference of sensitive attributes; no re-identification against off-platform identifiers

## Why not Devvit

[Devvit](https://developers.reddit.com/docs/) runs interactive apps *inside* Reddit. This workflow is an external, offline analysis tool that queries public listings across several subreddits and summarizes themes on my local machine for product planning. That pattern is outside Devvit’s in-platform app model, which is why I am requesting Data API access as a developer whose use case is not supported by Devvit.

## Planned implementation

- Language: Python
- Auth: Reddit OAuth2 (script/personal use once approved)
- Storage: short-lived local notes / caches only; no public dataset dump
- Repo: implementation scripts will be added here after access is granted

## Subreddits (initial)

Small, topic-specific sets only, for example:

- `r/startups`
- `r/SaaS`
- plus 1–3 niche communities tied to the product under consideration

No mass scanning of the whole site; no cross-posting.

## Operator

- Reddit account: `/u/Downtown-Act-9950`
- Contact: `zevinchen1993@gmail.com`
- Prior request id (revision of same use case): `18704215`

## Status

Awaiting revised Data API access approval. This README is the public source / product description for the access request.

## Compliance

I agree to follow Reddit’s [Developer Terms](https://www.redditinc.com/policies/developer-terms), [Data API Terms](https://www.redditinc.com/policies/data-api-terms), [Public Content Policy](https://support.reddithelp.com/hc/en-us/articles/23558095570836-Public-Content-Policy), and [Responsible Builder Policy](https://support.reddithelp.com/hc/en-us/articles/42728983564564-Responsible-Builder-Policy).
