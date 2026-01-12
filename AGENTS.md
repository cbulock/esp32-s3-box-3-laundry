# Laundry Screen — Agent Instructions


## Goal
Laundry Screen is an ESPHome device + custom firmware project. The deliverable is a firmware image that builds and flashes to the target MCU and renders a “laundry status” screen.


## Constraints
- Prefer small, incremental changes.
- Don’t refactor broadly unless asked.
- Keep style consistent with existing code.
- Avoid adding new dependencies unless clearly justified.


## Definition of “done” for the next milestone
- The firmware builds locally (CI-style build if possible).
- The device can be flashed (USB or OTA) and boots.
- The display shows *something* deterministic (even mocked data).


## Workflow
- Before coding: summarize findings + propose a short plan.
- While coding: minimal, scoped edits.
- After coding: update docs (README, build/flash steps), plus a `.env.example` or secrets guidance if needed.


## ESPHome rules
- Prefer using ESPHome primitives where possible.
- If custom components exist, extend them minimally.
- Keep YAML and C++ component interfaces clean.
- Treat Wi-Fi/API credentials as secrets; never hardcode.