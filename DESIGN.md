---
name: Bagel's Sitter Guide
description: A kawaii memo pad that walks a cat sitter through one visit, one sticker at a time.
colors:
  strawberry-milk: "#ffe3ec"
  memo-white: "#ffffff"
  blush-mat: "#fff2f6"
  plum-ink: "#3a1830"
  sticker-pink: "#ff4f8b"
  raspberry-ink: "#d81b60"
  petal-line: "#ffc2d6"
  butter: "#ffd66b"
  mint: "#7fd8b4"
  sky: "#9ad3ff"
  lilac: "#cdb2ff"
typography:
  display:
    fontFamily: "M PLUS Rounded 1c, ui-rounded, Hiragino Maru Gothic ProN, system-ui, sans-serif"
    fontSize: "1.95rem"
    fontWeight: 900
    lineHeight: 1.15
  headline:
    fontFamily: "M PLUS Rounded 1c, ui-rounded, system-ui, sans-serif"
    fontSize: "1.56rem"
    fontWeight: 900
    lineHeight: 1.15
  title:
    fontFamily: "M PLUS Rounded 1c, ui-rounded, system-ui, sans-serif"
    fontSize: "1.25rem"
    fontWeight: 900
    lineHeight: 1.15
  quantity:
    fontFamily: "M PLUS Rounded 1c, ui-rounded, system-ui, sans-serif"
    fontSize: "3.2rem"
    fontWeight: 900
    lineHeight: 1
    letterSpacing: "-0.02em"
    fontFeature: "tnum"
  body:
    fontFamily: "M PLUS Rounded 1c, ui-rounded, system-ui, sans-serif"
    fontSize: "16px"
    fontWeight: 500
    lineHeight: 1.55
  label:
    fontFamily: "M PLUS Rounded 1c, ui-rounded, system-ui, sans-serif"
    fontSize: "0.92rem"
    fontWeight: 800
    lineHeight: 1.4
rounded:
  photo: "14px"
  note: "18px"
  card: "20px"
  memo: "22px"
  pill: "999px"
spacing:
  xs: "6px"
  sm: "8px"
  md: "12px"
  lg: "16px"
  xl: "24px"
  xxl: "32px"
components:
  button-primary:
    backgroundColor: "{colors.raspberry-ink}"
    textColor: "{colors.memo-white}"
    rounded: "{rounded.pill}"
    height: "56px"
    padding: "0 20px"
  button-quiet:
    backgroundColor: "{colors.blush-mat}"
    textColor: "{colors.plum-ink}"
    rounded: "{rounded.pill}"
    height: "56px"
    padding: "0 20px"
  memo-card:
    backgroundColor: "{colors.memo-white}"
    textColor: "{colors.plum-ink}"
    rounded: "{rounded.memo}"
    padding: "12px 14px"
  door-note:
    backgroundColor: "{colors.raspberry-ink}"
    textColor: "{colors.memo-white}"
    rounded: "{rounded.note}"
    padding: "12px 14px"
  fact-chip:
    backgroundColor: "{colors.memo-white}"
    textColor: "{colors.plum-ink}"
    rounded: "{rounded.pill}"
    padding: "3px 12px"
---

# Design System: Bagel's Sitter Guide

## Overview

**Creative North Star: "The Sticker Sheet"**

The guide is a page torn from a kawaii memo pad, with Bagel's sticker sheet clipped on top. Each step of the visit is one memo; finishing it earns a die-cut sticker, so progress is literally a sheet filling up. It is cute and pink because the owners pinned that, but the cuteness lives in materials (strawberry-milk paper, keylined stickers, rounded lettering) rather than in decoration, so the task always reads first.

Density is calm and one-handed: one current step, its photo, one poster-size quantity and a thumb-zone button, with the whole visit listed openly underneath (or beside it on wide screens). The world never supplies the controls: buttons, lists and the photo zoom are ordinary web controls dressed in the palette.

**Key Characteristics:**
- Strawberry-milk ground, white memo sheets, plum ink, raspberry for anything the sitter must act on or read exactly.
- One rounded face for everything, including the kettle's 功能 / 取消 label.
- Die-cut stickers (circle, heart, star, flower) in pink, butter, mint, sky and lilac mark done-state and nothing else.
- A real night mode for a dim flat: deep rose, low glare, photos slightly dimmed.

## Colors

A pink-led palette where saturated colour is reserved for state and action, on soft pink paper.

### Primary
- **Raspberry Ink** (raspberry-ink): the primary button, quantities, step numbers, part labels and every small pink text; dark enough to pass 4.5:1 on white. Also the door note and the urgent help card in light mode.
- **Sticker Pink** (sticker-pink): sticker fills, the current slot's ring, bullets and the focus ring. Decorative and large-element only; never small text.

### Secondary
- **Butter** (butter), **Mint** (mint), **Sky** (sky), **Lilac** (lilac): sticker fills only, cycled with Sticker Pink so the sheet reads as a set. Numbers on them are Plum Ink.

### Neutral
- **Strawberry Milk** (strawberry-milk): the page ground.
- **Memo White** (memo-white): memo, sheet, overview and calm cards.
- **Blush Mat** (blush-mat): inset surfaces inside a memo (temperature pair, play tips, quiet buttons, the thank-you note).
- **Petal Line** (petal-line): dashed sticker outlines, hairline dividers, the memo pad's binding strip.
- **Plum Ink** (plum-ink): all body text and headings.

Night mode swaps to ground #24121b, sheet #36202b, mat #2d1823, ink #ffe8f0, sticker pink #ff6c9f, raspberry text #ff8fb5 with #2a0f1c on it, and an alert of #8f2452 so warnings stay serious without glowing.

### Named Rules
**The Stickers Mean Done Rule.** A sticker appears only where a step is finished. Empty is always a dashed outline with the step number; never use sticker shapes as decoration.

**The Raspberry Reads Rule.** Any pink text smaller than about 24px uses Raspberry Ink, not Sticker Pink.

## Typography

**Display Font:** M PLUS Rounded 1c (with ui-rounded, Hiragino Maru Gothic ProN, system-ui)
**Body Font:** M PLUS Rounded 1c

**Character:** One soft, rounded face carries every role, so rank comes from size and weight alone. It covers Chinese and Japanese too, so the appliance labels match the rest of the text.

### Hierarchy
- **Display** (900, 1.95rem, 1.15): the page title.
- **Headline** (900, 1.56rem, 1.15): section titles and, at 720px and up, the memo's step title (1.3rem on phones so it fits beside the photo).
- **Title** (900, 1.25rem): door note and help-card titles.
- **Quantity** (900, 3.2rem, line-height 1, tabular): the one value a step hinges on (⅓, ½, ×2). Long values such as 10–15 drop to 2.3rem and never wrap.
- **Body** (500, 16px, 1.55): instructions and notes.
- **Label** (800, 0.92rem): progress lines, part headers, captions.

### Named Rules
**The One Number Rule.** Each step has at most one poster-size quantity, set as a true fraction or symbol (⅓, ½, ×2, 40°C), never spelled out.

**The No Kicker Rule.** No small label sits above a heading. Progress lives in the sticker sheet card; the step number lives in the memo's sticker slot.

## Layout

A single 600px column on phones with 16px gutters: header, sticker sheet card (7 × 2 slots plus a part/progress line), door note when it applies, the current memo, an "Up next" line, then the open list of all 14 steps, help, Meet Bagel and the thank-you. From 980px the column widens to 1040px and the step list moves into a 360px sticky side column beside the memo. Inside a memo the photo takes 42% of the width beside the title on phones (230px from 720px, with the instructions moving beside the photo). The memo's action bar is sticky to the bottom of the viewport so Done is always in thumb reach.

Spacing runs on small steps (6, 8, 12, 16, 24, 32px): tight inside a memo, 24 to 32px between major blocks.

## Elevation & Depth

Soft paper lift. Sheets and memos float on one ambient shadow; stickers carry their own small drop shadow so they read as stuck on. Nothing else casts a shadow.

### Shadow Vocabulary
- **Sheet lift** (`box-shadow: 0 1px 2px rgba(58,24,48,.08), 0 10px 24px -14px rgba(58,24,48,.45)`): memo, sticker sheet, overview, calm cards, door note.
- **Sticker** (`filter: drop-shadow(0 1.5px 1.5px rgba(58,24,48,.28))`): die-cut stickers only.

## Shapes

Everything is rounded: photos 14px, notes 18px, cards 20px, the memo 22px, buttons and chips fully pill-shaped. The memo's top edge is a pink binding strip punched with holes. Stickers are die-cut with a 3.5px white keyline in four silhouettes (circle, heart, star, flower), each set at a slight tilt.

## Components

### Buttons
- **Shape:** pill (999px), 56px tall.
- **Primary:** Raspberry Ink with white text, 900 weight ("Stick it! Done", "Next step").
- **Quiet:** Blush Mat with Plum Ink (Back, Skip, Undo).
- **Press:** scales to 0.97 over 160ms with a strong ease-out; no hover-only affordances.
- **Hold to start a new visit:** quiet button where a Raspberry fill sweeps left to right over 1s while held and snaps back in 200ms on release.

### Sticker sheet (signature)
Fourteen round slots in a 7 × 2 grid inside a white card. Empty is a dashed Petal Line ring with the number; the current step has a solid Sticker Pink ring; done shows the sticker. Every slot is a button that opens its step.

### Memo
A white card with a binding strip: photo with a zoom badge, step title, the dashed sticker slot holding the step number, the quantity, instructions, dashed-divider notes, and the sticky action bar. On Done the sticker pops in with a slight overshoot (300ms) on both the memo and the sheet, then the next memo slides up 8px into place (220ms). Reduced motion swaps instantly.

### Step list
Rows of mini sticker slot, title and quantity, grouped under raspberry part headers. The step on screen has a Blush Mat fill and a pink inset ring; done steps are struck through in pink.

### Door note
A raspberry card with a drawn door icon in a white circle. It appears only on the first and last steps.

### Fact chips
White pills with 800-weight Plum Ink.

## Do's and Don'ts

### Do:
- **Do** keep the current step, its quantity and the Done button visible together on a 390 × 844 phone.
- **Do** put every owner detail inside the step that needs it, next to that step's photo.
- **Do** use Raspberry Ink for any pink text below about 24px.
- **Do** keep photos at their real proportions and offer tap to enlarge.

### Don't:
- **Don't** use stickers, hearts or stars as decoration; they mean "done".
- **Don't** set a small uppercase label above a heading.
- **Don't** let Sticker Pink carry body-size text; it fails contrast on white.
- **Don't** brighten warnings in night mode; they use the deep alert colour, not glowing pink.
