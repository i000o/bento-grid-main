# Bento Grid

[Live Site URL](https://i000o.github.io/bento-grid-main/)
![Outcome](/design/desktop-screenshot.png)

---

## Table of contents

- [Purpose & Scope](#purpose-and-scope)
- [Decisions](#decisions)
- [Future](#future)

---

## Purpose & Scope

This is a bento grid layout based on the design brief provided by [Frontend Mentor](https://www.frontendmentor.io/challenges/bento-grid-RMydElrlOj).

It works as a static bento grid, advertising the serviced offered by a hypothetical online engagement service.

`#tailwind`

---

## Decisions

**Cards as flex containers nested inside the grid**  
Each card uses Flexbox internally for its own content, while the outer layout is CSS Grid. Kept individual card markup simple and consistent without needing grid logic at the card level.

**`<body>` set as the grid container**  
Used `<body>` directly as the grid rather than wrapping the layout in a separate container element. Works for this project's scope, though a dedicated wrapper would be the more conventional approach for a layout likely to grow more complex.

---

## Future.

- Repeated `tracking` values were applied inline across multiple cards rather than abstracted into a reusable class — could consolidate using Tailwind's `@apply` or a shared utility class.
