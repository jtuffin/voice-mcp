# Voice-MCP Tasks and Ideas

## Documentation

- [Implementation Notes](./implementation-notes.md) - Completed work and decisions
- [Key Insights](./key-insights.md) - Important learnings and design principles

## High Priority

- [ ] Fix voice-mode ImportError - Add missing voice_mode() function to cli.py (v0.1.26)
- [ ] Provider Registry System - Unified configuration with provider metadata (cost, latency, privacy, features)
  - [Design Document](./provider-registry-design.md)
  - [MVP Implementation](./provider-registry-mvp.md)
  - [Implementation Notes](./provider-registry-implementation.md)
- [ ] Save Transcriptions - Add text saving alongside audio recordings in voice-mcp/transcriptions/
- [ ] Enhance provider registry with cost/latency/privacy metadata

## Medium Priority

- [ ] Provider selection logic based on user preferences (cost, privacy, features)
- [ ] Automatic fallback chain for providers
- [ ] Better first-run experience for Kokoro model downloads
- [ ] Configuration documentation update for new unified system

## Low Priority

- [ ] Provider cost tracking and reporting
- [ ] Audio/transcription manifest files linking recordings with metadata
- [ ] Conversation export features (for podcasts, analysis)
- [ ] Provider capability matrix display

## Ideas to Explore

- Look at OpenRouter's model for presenting provider options with transparent pricing
- Consider download size as a provider property for local models
- Add provider quality ratings based on user feedback
- Support for provider-specific features (emotions, voice cloning, etc.)

## Recently Completed

- [x] Provider Registry MVP - Basic registry with availability checking and selection logic
- [x] Update default voices - alloy for OpenAI, af_sky for Kokoro
- [x] Unified voice service status tool
- [x] Auto-start Kokoro functionality
- [x] Fixed health check endpoints for whisper.cpp and Kokoro
- [x] Emotional TTS with cost controls (VOICE_ALLOW_EMOTIONS)
- [x] Fixed OpenAI TTS client initialization bug

## Current Branches

- `master` - Has unified status tool and auto-start
- `feature/provider-registry` - Provider registry design docs
- `feature/emotional-tts` - Emotional TTS implementation (merged fixes)