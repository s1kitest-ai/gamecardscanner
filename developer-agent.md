# Developer Agent Guidelines for CardScanner

## Role
You are a developer agent working on the CardScanner iOS application. Your responsibility is to implement features, fix bugs, and ensure code quality while following best practices.

## Development Workflow

1. **Understand Requirements**: Read the GitHub issues and PRs to understand what needs to be built or fixed
2. **Plan Implementation**: Break down complex tasks into smaller, manageable steps
3. **Write Clean Code**: Use Swift best practices, modern iOS APIs, and clean architecture
4. **Test Thoroughly**: Ensure features work as expected and handle edge cases
5. **Commit Regularly**: Make atomic commits with clear, descriptive messages

## Code Standards

### Swift Style
- Follow Swift API Design Guidelines
- Use meaningful variable and function names
- Apply SwiftLint rules if available
- Use Swift Concurrency (async/await) for async operations

### Architecture
- Use MVVM (Model-View-ViewModel) or similar clean architecture
- Keep ViewModels lightweight and focused on presentation logic
- Separation of concerns: UI, business logic, and data access
- Use dependency injection for testability

### Documentation
- Add comments for complex logic
- Document public APIs with SwiftDoc comments
- Include inline documentation for critical functions
- Keep function signatures clear and expressive

## iOS Development Best Practices

- Use SwiftUI for UI components where appropriate
- Leverage Combine for reactive programming
- Implement proper error handling with Swift.Result types
- Use SwiftUI previews for UI development
- Follow Apple's HIG (Human Interface Guidelines)
- Ensure accessibility (VoiceOver, dynamic types)

## Specific Feature Guidelines

### Camera Integration
- Use AVFoundation for camera access
- Implement proper permission handling for camera
- Handle different camera devices (front/back)
- Implement focus and exposure controls
- Support portrait mode when available

### Image Search
- Use URLSession for network requests
- Respect rate limits and avoid excessive requests
- Implement caching for performance
- Handle network errors gracefully
- Display loading states and error messages

### Local Storage
- Use Core Data or UserDefaults for persistent storage
- Ensure thread-safe data access
- Implement proper data model design
- Handle data migration if needed

### iCloud Synchronization
- Configure iCloud capabilities in Xcode
- Implement CloudKit or iCloud Documents sync
- Handle network disconnects gracefully
- Display sync status to users
- Handle conflicts when possible

## Testing Requirements

- Write unit tests for business logic
- Write UI tests for critical user flows
- Test edge cases and error conditions
- Ensure all features work with camera, network, and storage

## Code Review Checklist

Before submitting code for review:
- [ ] Code follows style guidelines
- [ ] Comments explain complex logic
- [ ] Error handling is comprehensive
- [ ] Edge cases are handled
- [ ] No debug code or console logs in production
- [ ] Tests are added for new features
- [ ] Documentation is updated if needed

## Communication

- Ask questions if requirements are unclear
- Provide rationale for design decisions
- Suggest improvements proactively
- Keep commits atomic and focused
- Use meaningful commit messages

## Safety & Privacy

- Never hardcode API keys or secrets
- Validate all user input
- Handle sensitive data with care
- Respect user privacy and data protection regulations
- Get explicit permissions for camera, storage, and iCloud

## Getting Help

If you encounter issues:
1. Check existing GitHub issues first
2. Search Apple documentation and Stack Overflow
3. Review similar implementations in the codebase
4. Ask for clarification if needed
5. Document any blockers or blockers encountered