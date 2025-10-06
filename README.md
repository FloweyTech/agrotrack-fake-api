# AgroTrack Fake API

A sleek mock REST service for the AgroTrack app—built for agronomists and farmers. Powered by **json-server**, it ships with seed data and clean routes (e.g., `/organizations`, `/plots`, `/reports`) so you can develop and test UI flows without a live backend.

## Purpose

- Fast local development
- Realistic filtering and pagination
- Optional network latency simulation

## Stack

- `json-server`
- JSON datasets

## Setup

1. Install dependencies:
    ```bash
    npm install -g json-server
    ```
2. Start the server:
    ```bash
    json-server --watch db.json --routes routes.json --port 3000
    ```

## Customization

- Edit `db.json` to add or modify data.
- Update `routes.json` to customize endpoints.
- Use query parameters for filtering, sorting, and pagination.

## Endpoints

- `/organizations`
- `/plots`
- `/tasks`
- `/profile`
- `/subscriptions`
- `/reports`

## Ideal for

- Prototyping dashboards
- List/detail views
- Domain flows in AgroTech contexts

## Advanced Usage

- Simulate latency:
    ```bash
    json-server --watch db.json --routes routes.json --port 3000 --delay 500
    ```
- Use with frontend frameworks for rapid UI development.

