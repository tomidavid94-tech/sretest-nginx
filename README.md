Hello!

This is a test repo for the SRE task.
Prerequisites:
- SSH connection to an Ubuntu Server (Put IP to hosts.yml)
- Public IP address for Letsencrypt certification
- Registered Domain name: change grous_vars/sretest.yml domain variable to the correct one.

For now the Certbot certificate generation is in staging mode to avoid hitting rate limit with Letsencryt.

Execution: ansible-playbook -i inventory/sretest --private-key ~/.ssh/"some_key.pem" --diff all.yml

Design diagram

<img width="698" height="583" alt="grafik" src="https://github.com/user-attachments/assets/d38a3cc1-2263-4fa1-91ad-c4900ba3b5c3" />
