---
layout: default
title: Pulse Security
parent: SQL Scripts
nav_order: 1
---

# Pulse Security

## Table of contents

1. TOC
{:toc}

## Change additional role name/tooltip

1. Find the table for additional roles
    ```sql
    SELECT * FROM PulseAdditionalRoles
    ```
2. Create an update statement
    ```sql
    UPDATE PulseAdditionalRoles
    SET Tooltip = 'New ToolTip'
    WHERE ID ='_'

## Remove additional attributes

