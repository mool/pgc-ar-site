# PGC.AR - Personal Website

A personal website built with Hugo and the hugo-profile theme.

## 🌐 Live Site

Visit the live site at: [https://pgc.ar](https://pgc.ar)

## 🚀 Local Development

### Prerequisites

- [Hugo Extended](https://gohugo.io/installation/) (v0.68.0+)
- [Git](https://git-scm.com/)

### Getting Started

1. **Clone the repository with submodules**:

   ```bash
   git clone --recurse-submodules https://github.com/your-username/pgc-ar-site.git
   cd pgc-ar-site
   ```

2. **Start the development server**:

   ```bash
   hugo server -D
   ```

3. **View the site**:
   Open [http://localhost:1313](http://localhost:1313) in your browser

### Theme Updates

The hugo-profile theme is included as a git submodule. To update:

```bash
git submodule update --remote themes/hugo-profile
```

## 🐳 Docker Development

### Build the container:

```bash
docker build -t pgc-ar-site .
```

### Run locally:

```bash
docker run -p 8080:80 pgc-ar-site
```

Visit [http://localhost:8080](http://localhost:8080)

## 🚦 CI/CD Pipeline

The project includes automated GitHub Actions workflows:

### Features:

- **Multi-platform builds** (linux/amd64, linux/arm64)
- **Container registry publishing** to GitHub Container Registry
- **Automated deployments** on push to main/master
- **Pull request previews**
- **Build caching** for improved performance

### Workflow Triggers:

- Push to `main` or `master` branches
- Git tags following `v*` pattern
- Pull requests to `main` or `master`
