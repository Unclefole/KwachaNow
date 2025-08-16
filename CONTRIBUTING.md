# Contributing to KwachaNow

Thank you for your interest in contributing to KwachaNow! This document provides guidelines and information for contributors.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [Development Setup](#development-setup)
- [Making Changes](#making-changes)
- [Submitting Changes](#submitting-changes)
- [Style Guidelines](#style-guidelines)
- [Testing](#testing)
- [Documentation](#documentation)

## Code of Conduct

By participating in this project, you agree to abide by our code of conduct. Please treat all contributors with respect and maintain a professional, inclusive environment.

## Getting Started

1. Fork the repository
2. Clone your fork: `git clone https://github.com/your-username/kwachanow.git`
3. Create a new branch: `git checkout -b feature/your-feature-name`
4. Follow the development setup instructions in the README

## Development Setup

### Prerequisites

- Node.js 18+ and npm/pnpm
- Docker and Docker Compose
- PostgreSQL (or use Docker)

### Installation

```bash
# Install dependencies
npm install

# Copy environment variables
cp .env.example .env

# Set up database
npx prisma migrate dev
npx prisma db seed

# Start development servers
npm run dev
```

## Making Changes

### Branch Naming

- Features: `feature/description`
- Bug fixes: `fix/description`
- Documentation: `docs/description`
- Refactoring: `refactor/description`

### Commit Messages

Use conventional commit format:

```
type(scope): description

Optional body explaining the change

Optional footer with breaking changes or issues closed
```

Types: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`

### Code Quality

- Run linter: `npm run lint`
- Run formatter: `npm run format`
- Run tests: `npm run test`
- Type check: `npm run type-check`

## Submitting Changes

1. Ensure all tests pass
2. Update documentation if needed
3. Push to your fork
4. Create a Pull Request
5. Fill out the PR template completely
6. Wait for code review

### Pull Request Guidelines

- Link related issues
- Provide clear description of changes
- Include screenshots for UI changes
- Ensure CI/CD checks pass
- Request reviews from maintainers

## Style Guidelines

### TypeScript/JavaScript

- Use TypeScript for all new code
- Follow ESLint and Prettier configurations
- Prefer functional programming patterns
- Use meaningful variable and function names
- Add JSDoc comments for public APIs

### CSS/Styling

- Use Tailwind CSS utilities
- Follow BEM methodology for custom CSS
- Maintain responsive design principles
- Preserve the KwachaNow brand colors and identity

### API Design

- Follow RESTful conventions
- Use consistent error response format
- Implement proper HTTP status codes
- Add OpenAPI/Swagger documentation

## Testing

### Unit Tests

- Write tests for all business logic
- Aim for 80%+ code coverage
- Use descriptive test names
- Follow AAA pattern (Arrange, Act, Assert)

### Integration Tests

- Test API endpoints
- Test database interactions
- Mock external services

### E2E Tests

- Test critical user journeys
- Test across different browsers
- Include accessibility testing

## Documentation

- Update README for setup changes
- Document new API endpoints
- Add inline code comments
- Update architecture diagrams
- Write user-facing documentation

## Release Process

1. Update version in package.json
2. Update CHANGELOG.md
3. Create release PR
4. Tag release after merge
5. Deploy to production

## Getting Help

- Check existing issues and discussions
- Join our community chat
- Ask questions in issues
- Contact maintainers directly

## Recognition

Contributors will be recognized in:

- CONTRIBUTORS.md file
- Release notes
- Project documentation
- Social media announcements

Thank you for contributing to KwachaNow!