Here's a more concise version of the `README.md`:

---

# Blockchain Project Orchestration

This project integrates **frontend**, **backend**, and **blockchain core** services into a decentralized application (DApp) using **React**, **FastAPI**, and **Hardhat**.

## Submodules

The project uses these submodules:

- [Frontend](https://github.com/Mkznd/blockchain_frontend): React and Vite-based UI.
- [Backend](https://github.com/Mkznd/blockchain_backend): FastAPI backend for data and contributions.
- [Blockchain Core](https://gitlab.com/Mkznd/blockchain_core): Hardhat-powered smart contracts.

---

## Prerequisites

Install the following:

- **Git**
- **Docker** and **Docker Compose**
- **Node.js** (if running locally)

---

## Setup

### 1. Clone the Repository

Clone the main repo and initialize submodules:

```bash
git clone --recurse-submodules https://github.com/Mkznd/blockchain_project
cd https://github.com/Mkznd/blockchain_project
```

If already cloned:

```bash
git submodule update --init --recursive
```

### 2. Configure Environment Variables

Create `.env` files for each service.

### 3. Start the Services

Build and start all services:

```bash
docker-compose up --build
```

---

## Access Services

- **Frontend**: [http://localhost:3000](http://localhost:3000)
- **Backend**: [http://localhost:8000](http://localhost:8000)
- **Blockchain Node**: [http://localhost:8545](http://localhost:8545)
- **Contract Artifacts**: [http://localhost:3001](http://localhost:3001)

---

## Updating Submodules

To fetch the latest updates for all submodules:

```bash
git pull
git submodule update --remote --merge
```

---

## Troubleshooting

1. **Submodules Not Found**: Run:
   ```bash
   git submodule update --init --recursive
   ```
2. **Port Conflicts**: Ensure ports `3000`, `8000`, `8545`, and `3001` are free.

---

## Submodule Links

- [Frontend](https://github.com/Mkznd/blockchain_frontend)
- [Backend](https://github.com/Mkznd/blockchain_backend)
- [Blockchain Core](https://gitlab.com/Mkznd/blockchain_core)

---

## License

This project is licensed under the MIT License. See the `LICENSE` file in each submodule for details.
