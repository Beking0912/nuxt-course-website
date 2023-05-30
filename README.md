# Nuxt3 CheatSheets

## SPA vs SSR

**Single Page:**

1. Initial page load is slow
2. No round trips to server

**Server Side Rendered:**

1. Very fast start up
2. Interactions are slow

**Universal Rendering:**

1. No round trips to server
2. Very fast start up

## Organizing Code in Nuxt 3

1. Default to Pages
2. Move common pieces to layouts
3. Move smaller pieces of functionality into Components

## Things to consider

- How do you decide between a Layout or a Component?
- Where would you expect to find that code?
- Components usually do one thing, Layouts often do multiple things.
- Start by putting code into a Layout, then move to a Component.
- There is no "correct" answer here.

## Type of Composables

1. Single use
2. Reusable
3. Generic

## Why OAuth?

- Stop sharing user login info
- Share tokens that represent permission(JWT)
- Industry standard

## Nitro and h3

- Universal JS server
- Rendering: SSR/Static/etc.
- File-based routing
- Supports multiple hosting providers
- Builds standalone server so deploys don't require any extra code
- Automatic code-splitting
- Storage layer to access filesystem, database, Redis, and more
- Caching system built on top of the storage layer

## h3

- Minimal HTTP framework used internally by Nitro
- Fast and tree shake-able replacement for Express
- Extended by creating composable-like utilities
- Built-in utilities used directly in Nuxt event handlers
- readBody, getQuery, setCookie

## unjs

- A set of packages designed to work together and make building universal JS application
- Includes Nitro and h3
- Nuxt and Nitro use unjs/hookable for their hook systems
