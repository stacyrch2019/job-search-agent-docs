# How It Works

This document provides a high-level guide to how the job search agent works.

## Overview

The agent hits two job sites (LinkedIn and Indeed), loops through search terms, deduplicates results, and saves those results in a file. 

## Search Terms

Edit your `search_terms` list in `job_search.py`. The current defaults are aimed at roles in software documentation.

## Job Sites

The jobspy library scrapes LinkedIn and Indeed independently. If LinkedIn fails, the search still works for Indeed.

## Error Handling

Sometimes LinkedIn rejects search terms and the script still runs instead of crashing. 

## Output File

The output file is `ai_jobs_YYYY-MM-DD.csv.` The columns consist of job ID, the site, the `job_url_direct`, the company, location, and job posted. The file tells you whether or not a role is remote. The file also gives you the `company_url` and the `company_url_direct`. 