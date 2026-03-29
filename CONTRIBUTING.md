#  Contributing

## Branching

- `main` — always buildable, always the latest accepted state.
- `feature/<short-name>` — your working branch. Keep it short-lived.
- No `develop` branch. Features go straight to main via PR.

## Commits

Use conventional commits:

- `feat: add SPI driver for ADS8354`
- `fix: correct phase shift calculation at low duty`
- `docs: update pinout diagram for STM32G4`
- `test: add unit test for impedance accumulator`
- `refactor: extract transformer model into submodule`

The prefix makes `git log --oneline` scannable and enables auto-changelogs later.

## Pull requests

Open a PR for every merge to main, even when working solo.
This creates a review trail and a natural place to document why a change was made.

Use the PR template. Fill in the checklist. If it touches hardware, note which
board/setup was used to verify.

## Releases and tags

Tag with semver when something is:
- Ordered (PCB sent to fab)
- Flashed to hardware for a test campaign
- Deployed or handed off

Not every merge needs a tag. Tags mark commitments.

Format: `v1.0.0` — major.minor.patch.