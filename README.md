
# Fabbs Tech — GitHub organization

## Structure

Every repo in this org is one of:

- **System** — a persistent, reusable thing we build (hardware, firmware, software, infrastructure).
  Named plainly: `pwr-converter`, `battery-modeling`, `dev-platforms`, `tooling`.
- **Product** — a system packaged to solve a specific problem. Prefixed with `prod-`:
  `prod-cell-tester-v1`, `prod-eis-thesis`.

## Creating a new repo

1. Decide if it's a system or a product.
2. Name it following the convention above. Lowercase, hyphens, no underscores,
   no company name, no sequential numbering.
3. Clone the `tooling` repo (or have it alongside in your workspace).
4. Create a `project_config.json` in the new repo root declaring its disciplines.
5. Run the tooling setup script; it scaffolds the folder structure, .gitignore,
   and README template.

See the [tooling repo](../tooling) for full setup instructions.

## Conventions

- **Branching**: `main` is the default branch. Work on `feature/<short-name>` branches.
  Merge via PR, even when working solo because it creates a review trail.
- **Commits**: use conventional commits: `feat:`, `fix:`, `docs:`, `test:`, `refactor:`.
- **Tags**: semver (`v1.0.0`) for releases. Tag when something is ordered, flashed,
  or deployed; not for every merge.
- **Issues**: use for work tracking within a repo. Cross-reference Notion task links
  in the issue body when relevant.

## Platforms

| Platform   | Role              | Location                    |
|------------|-------------------|-----------------------------|
| GitHub     | Build and track   | You are here                |
| SharePoint | Store and find    | Tech site → /tech - Documenten/|
| Notion     | Plan and decide   | Fabbs Office -> Tech teamspace |

Each system or product has an entry in all three. The system name is the shared identifier.