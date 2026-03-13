# Repository Policy

## Project Description
GameCardScanner is a mobile application designed to help users scan, organize, and manage their collectible card collections. It leverages the device's camera to capture card images, provides search functionality, detail views, iCloud sync, and collection management features.

## Development Workflow

### Branch Naming Convention
All work must be done in feature branches following this format:
- `feature/issue-<issue-number>-<short-description>` for new features
- `bugfix/issue-<issue-number>-<short-description>` for bug fixes
- `hotfix/issue-<issue-number>-<short-description>` for urgent production fixes

Example: `feature/issue-6-welcome-screen`

### Repository Usage
- **Primary repository**: `s1kitest-ai/gamecardscanner` (hosted on GitHub)
- All development must occur within this repository
- Do NOT create separate repositories for individual issues or features
- Work must be version-controlled using Git

### Commit Messages
Use clear, descriptive commit messages:
- Prefix with type: `feat:`, `fix:`, `docs:`, `style:`, `refactor:`, `test:`, `chore:`
- Reference issue numbers when applicable: `feat: add welcome screen (closes #6)`
- Keep subject line under 50 characters
- Provide detailed explanation in body when needed

### Pull Request Process
1. Push your feature branch to origin
2. Open a Pull Request against `main` branch
3. Include:
   - Clear title and description
   - Reference to related issue(s)
   - Summary of changes
   - Any special instructions for testing
4. Request review from at least one team member
5. Address all feedback before merging
6. Squash and merge upon approval

### Prohibited Actions
- Creating new repositories for individual issues or features
- Storing work exclusively in personal development folders without pushing to remote
- Using non-version-controlled environments for primary development
- Merging directly to `main` without Pull Request review
- Leaving sensitive information (API keys, tokens) in commit history

### Code Quality
- Follow platform-specific coding standards (Swift conventions for iOS)
- Write meaningful comments for complex logic
- Ensure all new code is tested appropriately
- Handle errors gracefully
- Optimize for performance and memory usage

### Documentation
- Update README.md when significant changes affect setup or usage
- Document new public APIs or significant architectural decisions
- Keep inline documentation up-to-date

Last updated: 2026-03-13
