# WireGuard + Pi-hole 
## An easy setup with Docker Compose and GitHub Actions 

This project gives a ready solution to install [WireGuard](https://www.wireguard.com/) in combination with [Pi-hole](https://pi-hole.net/) in your server.    
You can use it wherever you want, I run it in a VPS with Debian.  

# Install
Fork this repo and set the following secrets:  

| NAME        | DESCRIPTION                                                                        |
|-------------|------------------------------------------------------------------------------------|
| PUBLIC_IP   | Server public IP (IPv4)                                                                 |  
| PRIVATE_IP  | Docker host IP (run `ip a`)                                                                    |
| REMOTE_PATH | docker-compose.yaml location inside the server, for example /config/               |
| SSH_USER    | SSH User, create a specific user with restricted permission, don't use a root user |
| SSH_KEY     | Private key of the ssh user                                                        |
| VPN_PEERS   | List of peers separate by comma (example: peer1,peer2,peer3..)                     |

Commit, Push and Run! :rocket:

# Requirements
Make sure your server has a public IPv4 and these packets installed: docker, docker-compose, rsync.  

### TODO:
- Setup machine via terraform 
- A better readme
