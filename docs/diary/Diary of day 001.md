# Diary of day 001

**Project Name:** ps2dev  
**User:** Hauke  
**Date:** 2025-06-06  
**State:** Closed  

## Planned Features
- Add optional reset callback parameter to keyboard_init method

## Changes
- Modified keyboard_init method to accept an optional ResetCallback parameter.
- Updated ps2dev.h and ps2dev.cpp accordingly.
- Added call to reset callback on soft reset (F5/F4 sequence).
- Committed and pushed changes to remote repository.

## Challenges
- Ensuring backward compatibility while adding optional parameter.

## Open Issues
- None

## Decisions
- Use function pointer typedef ResetCallback for reset callback.
- Keep reset callback optional with default nullptr parameter.
- Treat F4 command as reset for modern BIOS compatibility.

## Summary
Implemented the ability to set a reset callback in keyboard_init method optionally. The callback is stored and invoked on reset events if provided. Also added support to call the reset callback on soft reset (F5/F4 sequence). Changes were committed and pushed.
