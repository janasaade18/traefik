# traefik-config

Traefik reverse proxy with automatic Let's Encrypt certificates for the EC2 host.
Apps join it through the external `proxy` Docker network and expose themselves
with Traefik labels. Deployed by Ansible.

    cp .env.example .env     # set ACME_EMAIL
    docker compose up -d
