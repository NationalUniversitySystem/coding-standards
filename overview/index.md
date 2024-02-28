---
title: Overview
layout: default
nav_order: 2
---

# Overview

Our code should be simple, accessible, readable, and well-documented.

## Simple

For many reasons, NU prizes simple code. This makes the codebase easier to maintain; it speeds up site load times and deployment times; priorities change frequently; and over time, various teams and team members touch different parts of the codebase. We strive to help stakeholders identify goals rather than specific methods to reach their goals, reflect on the best way to achieve those goals, and achieve the shared vision with a minimum viable product.

To help keep things simple, follow these guidelines:

- Follow WordPress coding standards, particularly WPVIP standards.
- Do things the "WordPress way," meaning generally include functionality in plugins, styling in themes, and WP functions where feasible.
- Use native components (basic HTML elements with built-in functionality) where possible. (For example, use the `<nav>` element for navigation.)
- Use the least amount of markup possible. (For example, avoid nesting `<div>`s repeatedly.)
- Make use of the cascade in CSS. (For example, set the main font on the `<body>` tag so it only needs to be overriden for heading tags. As another example, favor lower specificity selectors like `.group` rather than high-specificity selectors like `#chat-box` or `.group .content.black a.highlight`.)
- Extend Core blocks rather than building wholly separate blocks where feasible.
- Remove code rather than commenting it out.
- Develop mobile-first. This is a shift from how the teams built in the past, but over time as we move to this paradigm it speeds up page loads for mobile screens significantly.

## Accessible

As an organization that receives some government funding, NU aims to be fully WCAG 2.1 level A compliant.

## Readable

Although we value small file sizes, we value readability higher. Don't nest functions deeply if an easier-to-read alternative is available. Similarly, use plenty of whitespace in code - particularly indention following WP Coding Standards - to make it easy to skim through the contents of a file.

## Well-documented

Comments and commits should be written thoughtfully so that it's easy for an outsider to understand how things work and why they were set up a particular way.

Within code files, use comments that state a function's name, parameters, and returns. Use an active voice ("Parse API results", not "Function to parse API results" or "Parsing API results") and succinct sentences.

Within commits, title the commit using an active voice ("Add hero section") and add helpful context in the description ("Replace multiple test variants with February 2024 CRO winner.").