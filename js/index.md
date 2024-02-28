---
title: JS
layout: default
nav_order: 3
---

# JS

## Simple

A lot of our codebase was built with dependencies such as jQuery. Though that was beneficial at the time, we now prefer to avoid such dependencies where possible. Prefer fewer dependencies and native JavaScript over frameworks and dependencies. When touching old code, try to update it so it no longer requires dependencies, so eventually we can remove them.

## Built

JavaScript should be processed (such as by `wp-scripts`). This makes it easier to ensure final transpiled file will be as cross-browser compatible as possible.