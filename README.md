# sam-scm-gitlab-plugin

A Node.js/Express.js plugin that provides Source Control Management (SCM) functionalities for Gitlab. This plugin connects to the Gitlab API to offer operations such as listing repositories, branches, commits, and file content retrieval.

## Features

- Connects to Gitlab API using personal access tokens.
- List and retrieve details of repositories.
- List branches and commits.
- Compare commits.
- Get file contents within a repository.
- Centralized error handling for API operations.
- Easily configurable via JSON configurations.

## Plugin Architecture

The plugin follows a modular architecture designed to run as a standalone service in a Docker container.

### Directory Structure

sam-scm-gitlab-plugin/
├── src/
│   ├── v1/
│   │   ├── methods/        # Methods (actions) to perform SCM operations
│   │   ├── controllers/    # API controllers (e.g., Gitlab controller)
│   │   ├── routes.js       # Express routes configuration
│   │   └── services/
│   │       └── gitlab/     # Gitlab provider related code
│   ├── app.js             # Express app initialization and middleware configuration
│   └── server.js          # Server bootstrapping
├── plugin.configs.json    # Plugin configuration file (Gitlab settings only)
├── README.md              # Plugin documentation
└── plugin-root/          # Documentation

## Prerequisites

- Node.js (v14 or above recommended)
- npm (v6 or above)

## Installation

1. Clone this repository:

```bash
git clone https://gitlab.com/SorenHQ/sam-scm-gitlab-plugin.git
```

2. Change to the project directory:

```bash
cd  sam-scm-gitlab-plugin
```

3. Install the dependencies:

```bash
npm install
```

4. Development & Usage:

```bash
npm start
```

Happy coding and enjoy using sam-scm-gitlab-plugin!
