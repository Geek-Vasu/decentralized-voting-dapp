# Decentralized Voting System using Ethereum

A secure and transparent blockchain-based voting application built using Ethereum. This system eliminates centralized control, ensuring tamper-proof and trustless elections.

---

## Overview

This project leverages blockchain technology to create a decentralized voting platform where:

* Votes are immutable and transparent
* No central authority controls the system
* Users can vote securely using crypto wallets

---

## Features

* JWT-based authentication system
* Ethereum blockchain integration for secure voting
* Admin dashboard to manage elections
* User interface for casting votes
* Transparent and tamper-proof vote records
* No intermediaries (trustless system)

---

## Tech Stack

* **Frontend:** HTML, CSS, JavaScript
* **Backend:** Node.js, FastAPI
* **Blockchain:** Ethereum, Truffle, Ganache
* **Database:** MySQL
* **Authentication:** JWT
* **Wallet:** MetaMask

---

## Requirements

* Node.js (v18+)
* Python (v3.9+)
* MySQL
* Ganache
* MetaMask Extension

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/Geek-Vasu/decentralized-voting-dapp.git
cd decentralized-voting-dapp
```

---

### 2. Install dependencies

```bash
npm install
pip install fastapi mysql-connector-python pydantic python-dotenv uvicorn PyJWT
```

---

### 3. Setup Database

Create a MySQL database:

```sql
CREATE DATABASE voter_db;

CREATE TABLE voters (
    voter_id VARCHAR(36) PRIMARY KEY NOT NULL,
    role ENUM('admin', 'user') NOT NULL,
    password VARCHAR(255) NOT NULL
);
```

---

### 4. Configure Environment

Update `.env` file inside `Database_API` with your DB credentials.

---

### 5. Run Blockchain (Ganache)

* Start Ganache
* Import accounts into MetaMask
* Add network:

  * RPC: http://localhost:7545
  * Chain ID: 1337

---

### 6. Compile & Deploy Contracts

```bash
truffle compile
truffle migrate
```

---

### 7. Start Application

```bash
node index.js
```

In another terminal:

```bash
cd Database_API
uvicorn main:app --reload
```

---

### Access App

```
http://localhost:8080/
```

---

## Project Structure

* `contracts/` → Smart contracts
* `migrations/` → Deployment scripts
* `Database_API/` → Backend API
* `src/` → Frontend code
* `index.js` → Server entry point

---

## Learning Outcomes

* Understanding Ethereum smart contracts
* Working with Web3 and decentralized applications
* Integrating blockchain with backend systems
* Building secure authentication systems

---

## Authors

* Vasu Arora
* Shreya Garg
* Utkarsh Singh

---
