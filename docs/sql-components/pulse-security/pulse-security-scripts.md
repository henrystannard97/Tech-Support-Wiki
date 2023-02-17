---
layout: default
title: Pulse Security
parent: SQL Scripts
nav_order: 2
---

# Pulse Security

## Table of contents

1. TOC
{:toc}

## Change position start date

To change a position start date:
1. Find the user ID of the user, this can be done following the SQL below.
    ```sql
    SELECT * FROM smpuserdetail
    where firstname = '_'
    ```
2. Copy the userid and find the positions set against the user, follow the SQL below.
    ```sql
    select * from pulseuserpositions
    where userid ='_`
    ```
3. Find the position and compare the start date with what is shown in the UI. Now use the script below to set the new position start date. This start date must follow the date/time format in the database. For example: '2023-02-27 00:00:00.000'

    ```sql
    UPDATE pulseuerpositions
    SET PositionStartDate ='_'
    WHERE ID = '_' AND USERID = '_'
    ```
