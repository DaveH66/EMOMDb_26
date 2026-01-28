# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

EMOMDb_26 is a project to create visibility of EMOM (Electronic Music Open Mic) performances. This is currently an early-stage repository without application code.

## Current State

This repository is in its initial setup phase. There is no build system, test framework, or application code yet. The repository contains only:

- Basic README
- GitHub Actions workflows for CI and Claude Code integration

## GitHub Actions Workflows

The repository has three GitHub Actions workflows configured:

### 1. Claude Code Review (`.github/workflows/claude-code-review.yml`)
- Triggers on pull requests (opened, synchronize, ready_for_review, reopened)
- Runs automated code reviews using Claude Code
- Requires `CLAUDE_CODE_OAUTH_TOKEN` secret to be configured

### 2. Claude PR Assistant (`.github/workflows/claude.yml`)
- Triggers when `@claude` is mentioned in:
  - Issue comments
  - Pull request review comments
  - Pull request reviews
  - Issue titles or bodies
- Allows interactive assistance from Claude on issues and PRs
- Requires `CLAUDE_CODE_OAUTH_TOKEN` secret to be configured

### 3. Basic CI (`.github/workflows/workflow.yml`)
- Triggers on push/PR to main branch or manual dispatch
- Currently just a placeholder that echoes "Hello, world!"
- Should be updated when build/test processes are added

## Development Setup

No build, test, or development commands are available yet. This section should be updated once the project structure and tooling are established.
