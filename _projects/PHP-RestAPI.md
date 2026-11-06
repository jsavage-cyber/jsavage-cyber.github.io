---
layout: project
title: "PHP Rest API"
description: "My first large scale PHP Rest API"
github: https://github.com/jsavage-cyber/PHP-Rest-API
tags: [Php, SQL]
---

## Overview

This project was part of my university software architecture module, and it took me about a week to finish, as it was my first encounter with the dreaded PHP!

## How it works

It’s a REST API that serves data from a university-hosted MySQL database, which I managed through phpMyAdmin. The API has four endpoints, several of which accept parameters so users can narrow down their searches. Alongside the endpoints, the repo contains a helper for executing queries, the database connection, and an .htaccess file that routes every request through a single entry point where it’s authenticated. The project originally used a bearer token for authentication, which has been removed from the published code.

```php
$offset = (int)($page - 1) * 10;
$sql = "SELECT id AS content_id, award_id, title, abstract, type, track
        FROM dis2025_content
        ORDER BY dis2025_content.id
        LIMIT 10 OFFSET " . (int)$offset;
```
It ain't pretty but it sure is interesting ^

## What I learned

The biggest lesson? I’d rather not build a career around PHP if I can avoid it! While it was interesting, I found it a frustrating language to learn, especially combined with SQL as someone new to both. That said, building my own REST API from scratch was genuinely rewarding. It gave me a much clearer understanding of how routing, authentication and HTTP status codes work under the hood, and that’s knowledge I’ll carry into future projects whatever language I’m using.

Thanks for reading!