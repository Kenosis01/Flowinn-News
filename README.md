# Flowinn News

Flowinn News is a lightweight, real-time AI-focused news aggregator that filters, processes, and delivers only high-signal artificial intelligence and technology news. It removes noise such as gadget reviews, promotions, and irrelevant content to keep the feed clean and focused.

## Overview

Flowinn News is designed to provide a fast and minimal reading experience for AI enthusiasts, developers, and researchers. It combines automated scraping, intelligent filtering, and structured data delivery to power a modern news experience.

The system is built around a pipeline that collects news from multiple sources, processes and enriches it, and publishes a clean JSON feed that powers the frontend.

## Key Features

- AI-focused news filtering
- Automated article collection from multiple sources
- Duplicate removal and content deduplication
- Image extraction from articles
- Full article summarization support
- Structured JSON output for frontend use
- Lightweight and fast data delivery
- Designed for both feed and swipe-style interfaces

## How It Works

Flowinn News operates on a fully automated pipeline:

1. RSS feeds and sources are fetched at regular intervals.
2. Articles are collected and normalized into a common format.
3. Duplicate articles are removed using unique identifiers.
4. Non-AI-related content is filtered out.
5. Selected articles are enriched with full text and images when needed.
6. Content is summarized and ranked based on relevance.
7. Final structured data is exported as `news.json`.
8. The JSON file is published to a public repository for frontend consumption.

## Data Format

Each article in the feed follows this structure:

```json
{
  "id": "unique_article_id",
  "title": "Article title",
  "date": "publish date",
  "url": "source URL",
  "summary": "short or expanded summary",
  "image": "image URL if available",
  "source": "publisher name"
}
