# Actions

Reusable [GitHub Actions](https://docs.github.com/actions) workflows.

## 📦 Workflows

### 1. `pages-deploy.yml`

Deploys static content (e.g. Vite, React, or Svelte apps) to **GitHub Pages** using **pnpm**.

#### 🚀 Usage

In your project repository, create `.github/workflows/deploy.yml`:

```yaml
name: Deploy to Pages

on:
  push:
    branches: ['main']
  workflow_dispatch:

jobs:
  deploy:
    uses: jsubroto/actions/.github/workflows/pages-deploy.yml@main
    secrets: inherit
```

### License

[MIT](LICENSE)
