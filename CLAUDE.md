# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Public portfolio site for employers and clients (design work and case write-ups, not source code). Hosted on **GitHub Pages** (main branch, site root).

## Stack

Plain HTML + CSS. No build step, no dependencies, no JavaScript yet — keep it that way unless a feature genuinely needs it. Code, identifiers, comments, and commit messages: **English**; site content and user-facing docs: **Russian**.

## Structure

- `index.html` — one-pager (hero, works grid, experience/skills, contacts).
- `works/*.html` — individual case pages; link to them from the works grid.
- `assets/style.css` — shared stylesheet (note relative paths differ: `assets/…` from root, `../assets/…` from `works/`).

## Commands

- View locally: open `index.html` in a browser. No dev server or build required.
- Deploy: push `main` to GitHub (Settings → Pages → Deploy from a branch).

## Content placeholders

Most copy is `TODO:`-marked placeholder text (name, role, works, contacts). Before replacing a placeholder: keep the `TODO:` comments in sync with the visible text; cards without a case page yet use class `work-card placeholder` (a `div`, not an `a`) and a «Скоро» meta label — upgrade them to real links only when `works/<case>.html` exists.