# AllSpaces Reddit Research Tool

## Overview
Internal read-only data research tool for AllSpaces.com. This tool connects 
to the Reddit Data API to monitor public posts and comments across a 
predefined set of real estate and rental-focused subreddits.

## Purpose
AllSpaces.com is an AI-powered property rental marketplace that consolidates 
residential, commercial, short-term, and unconventional rental listings into 
a single platform. This tool helps our product team identify trending pain 
points, feature requests, and market trends discussed by real renters and 
landlords on Reddit — informing our product roadmap and content strategy.

## What This Tool Does
- Connects to the Reddit Data API using OAuth 2.0 authentication
- Makes read-only GET requests to retrieve public posts and comments
- Targets the following subreddits:
  - r/realestate
  - r/landlord
  - r/renting
  - r/ApartmentHunting
  - r/nyc (housing/rental topics only)
  - r/personalfinance (housing cost discussions only)
- Collects: post titles, body text, comment text, upvote counts, timestamps, 
  and subreddit name
- Stores aggregated topic data in a private internal database for 90 days, 
  then deletes it
- Runs on a scheduled basis within free-tier rate limits 
  (under 100 queries per minute)

## What This Tool Does NOT Do
- Does not post, comment, vote, or interact with Reddit in any way
- Does not collect or store Reddit usernames or user identifiers
- Does not display Reddit content publicly or on AllSpaces.com
- Does not use data to train AI/ML models
- Does not exceed free-tier API rate limits

## Compliance
This tool is built in full compliance with Reddit's Responsible Builder 
Policy, Developer Terms, and Data API Terms. It is an internal-only tool 
with fewer than 10 authorized users.

## Platform
AllSpaces.com — https://www.allspaces.com

## Contact
Mark R. A. Arenella — Founder, AllSpaces.com
