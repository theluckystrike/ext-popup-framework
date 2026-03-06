# Contributing to ext-popup-framework

Thank you for your interest in contributing.

## Reporting Issues

When reporting issues, please include:

- A clear description of the problem
- Steps to reproduce the issue
- Your environment details (Node version, OS, etc.)
- Any relevant error messages or logs

Please check existing issues before opening a new one to avoid duplicates.

## Development Workflow

1. Fork the repository
2. Clone your fork locally
3. Create a feature branch from main
4. Make your changes
5. Test your changes
6. Commit with a clear message
7. Push to your fork
8. Submit a Pull Request

```bash
git checkout -b feature/your-feature-name
git commit -m "Add your feature"
git push origin feature/your-feature-name
```

## Code Style

- Use TypeScript for all new code
- Follow the existing code patterns in the project
- Use meaningful variable and function names
- Add JSDoc comments for public APIs
- Run `npm run build` before committing to ensure TypeScript compiles

## Testing

Run tests before submitting a Pull Request:

```bash
npm test
```

If adding new features, please add appropriate tests.

## License

By contributing, you agree that your contributions will be licensed under the MIT License.
