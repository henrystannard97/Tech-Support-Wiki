---
layout: default
title: Creating a new Dev Site
parent: General Processes
---

# General Processes

## Table of contents

1. TOC
{:toc}

## Creating a new Dev Site

1. Log into the dev database server and copy and edit the query below into the **Organisations** database.
    ```sql
    insert into organisations  
    values('councilname',    'PROD_PULSE_councilname', 'councilname', 'C:\FileStore\councilname\', 'C:\FileStore\councilname\', 'pulsesoftware.com')
    ```
2. Once the query has been run, run the **Copy PROD to DEV - Single DB pipeline**. 