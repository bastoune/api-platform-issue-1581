# API Platform Issue 1581

## Installation & Usage with Docker

### Step 0 - Prerequisites
- Docker installed
- Docker-Compose installed

### Step 1 - Env Vars
- modify .env variables as you like

### Step 2 - Init
- `docker-compose up -d`
- `docker-compose exec app php bin/console doctrine:schema:update --force`
- [TODO] create fixture

### Step 3 - Reproduce the bug
- `docker-compose exec app php bin/console debug:router | grep api_organizations_users_get_subresource`