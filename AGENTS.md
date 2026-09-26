# Agent Responsibilities for ghostty Snap

This snap is now maintained by [automated-ken](https://github.com/kenvandine/automated-ken), a self-hosted agentic snap-maintenance dashboard.

## What automated-ken Handles

- **Version Detection**: Automatically polls upstream for new releases
- **Version Bump PRs**: Opens pull requests to update the pinned version
- **CI Monitoring**: Monitors build workflows and automatically fixes failures using Copilot cloud agent (via follow-up PRs)
- **YARF Testing**: Runs tests to verify snap functionality
- **Channel Promotion**: Manages promotion from edge → candidate → stable

## Important Notes for Maintainers

- **Do not hand-edit** the pinned version in `snap/snapcraft.yaml`
- The removed workflow's job is now fully automated by automated-ken
- All build and release processes are now centralized and consistent across the snap fleet
