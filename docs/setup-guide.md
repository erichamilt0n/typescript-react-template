# Setup Guide

## Prerequisites

- Node.js (LTS version)
- Git
- GitHub account
- CircleCI account (optional)
- Vercel account (optional)

## Initial Setup

1. **Create Repository**
   ```bash
   gh repo create my-app --template your-org/typescript-react-template
   ```

2. **Configure Secrets**
   - Copy `templates/secrets/template.yml` content
   - Add to GitHub Organization Secrets or Repository Secrets
   - Required secrets are listed in the template

3. **Branch Protection**
   - Enable branch protection rules for `main`
   - Required status checks are pre-configured
   - Pull request reviews are required

4. **Code Quality Tools**
   - ESLint configuration in `config/eslint`
   - Prettier configuration in `config/prettier`
   - TypeScript configuration in `config/typescript`

5. **CI/CD Setup**
   - GitHub Actions workflows in `.github/workflows`
   - CircleCI configuration in `.circleci`
   - Vercel deployment configuration included

## Customization

1. **Workflows**
   - Modify `.github/workflows` files as needed
   - Adjust CircleCI config in `.circleci/config.yml`
   - Update Vercel settings in `vercel.json`

2. **Code Quality**
   - Customize ESLint rules in `.eslintrc.js`
   - Adjust Prettier settings in `.prettierrc`
   - Modify TypeScript config in `tsconfig.json`

3. **Security**
   - Update CodeQL configuration
   - Modify Snyk settings
   - Adjust Dependabot alerts

## Troubleshooting

See [TROUBLESHOOTING.md](../TROUBLESHOOTING.md) for common issues and solutions.
