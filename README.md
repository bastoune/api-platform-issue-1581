# API Platform Issue 1581

## Installation & Usage with Docker

### Step 0 - Prerequisites
- Docker installed
- Docker-Compose installed

### Step 1 - Env Vars
- create your own .env file from .env.dist: `cp .env.dist ./.env` 
- modify all '/PATH/TO/DIR' by absolute or relative path
- modify other variables as you like

### Step 2 - Run
- `docker-compose up -d`

### Step 3 - Reproduce the bug
- `docker-compose exec app php bin/console debug:router | grep api_organizations_users_get_subresource`