# Contributing to CyberEye / SecureLens (WMSA)

Thank you for your interest in contributing to **CyberEye / SecureLens**! Contributions, bug reports, feature suggestions, and documentation improvements are welcome.

---

## 📋 Code of Conduct

By participating in this project, you agree to abide by honest, respectful, and ethical collaboration guidelines. In particular, this tool is designed for authorized defensive security assessments and vulnerability remediation.

---

## 🚀 Getting Started

### Prerequisites

- **Python**: 3.11 or newer
- **Node.js**: 18.x or 20.x LTS
- **Docker & Docker Compose**: Required for running the isolated target and ZAP container.

### Local Development Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/nikhil-kumarrr/CyberEye-SIH.git
   cd CyberEye-SIH
   ```

2. **Set up the backend:**
   ```bash
   cd backend
   python -m venv .venv
   # Windows:
   .venv\Scripts\activate
   # Linux/macOS:
   source .venv/bin/activate

   pip install -e ".[dev]"
   cp .env.example .env
   ```

3. **Set up the frontend:**
   ```bash
   cd ../frontend
   npm install
   npm run dev
   ```

---

## 🧪 Testing Guidelines

Before submitting a Pull Request, ensure that all tests pass:

- **Backend tests:**
  ```bash
  cd backend
  pytest
  ```
- **Frontend build & lint:**
  ```bash
  cd frontend
  npm run build
  ```

---

## 📦 Pull Request Process

1. Fork the repo and create a descriptive feature branch:
   ```bash
   git checkout -b feat/your-feature-name
   # or
   git checkout -b fix/your-bugfix-name
   ```
2. Commit your changes using conventional commit messages:
   - `feat(...)`: New feature or capability
   - `fix(...)`: Bug fix
   - `docs(...)`: Documentation updates
   - `test(...)`: Unit or integration tests
   - `refactor(...)`: Code refactoring without behavioral change
3. Ensure the working directory is clean and all secrets/credentials are strictly excluded.
4. Push your branch and open a Pull Request against the `main` branch with a clear summary of your changes.
