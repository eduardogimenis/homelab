# self-host homelab
This repo documents my personal homelab — a collection of self-hosted services, infrastructure experiments, and automation tools running on bare-metal and virtualized hardware.

It's hosted locally on repurposed hardware, fronted by a reverse proxy using Cloudflare for remote access and security.


## Goals of This Homelab
- Full control over my data  
- Learn practical systems administration by doing  
- Automate sysadmin tasks so I can spend less time babysitting servers  
- Add useful services into my daily workflow  
- Break stuff → Fix stuff → Actually learn  


## Hardware
Dell XPS 8700  
- Upgraded video card  
- 32GB RAM  

It's an old family PC I pulled out of retirement — turns out it's perfect for labbing.


## Technologies Used
- Docker running on an Ubuntu VM  
- Apache for web services & reverse proxy  
- Prometheus for monitoring (early stages)  
- Cloudflare for external access & DNS  


## Services Running
| Service     | Purpose                                      |
|-------------|----------------------------------------------|
| Firefly III | Personal finance planning & tracking        |
| Wekan       | Kanban boards for personal/family use       |
| EspoCRM     | CRM system for the family business          |
| Apache      | Reverse proxy / web server                  |
| MariaDB     | Database backend for multiple services      |


![network_diagram](https://github.com/eduardogimenis/homelab/blob/main/images/networkDiagram.png)


## Roadmap
- [ ] Expand Prometheus monitoring & Grafana dashboards  
- [ ] Harden networking (internal VLANs, VPN access)  
- [ ] Automate provisioning with Ansible or scripting  
- [ ] Automate backups (database + config dumps)  
- [ ] Build out basic incident response playbooks/scripts  


## What I’ve Learned So Far
Working on this homelab has been the fastest way to actually *understand* networking, infrastructure, and system design.

It’s one thing to read about proxies — it’s another to get your hands dirty with it.

Some of the key lessons so far:
- Docker is great until it's not. There are many other ways to use Docker
- Backups don’t matter until they *really* matter  
- Running multiple services locally teaches you way more about Linux internals than you'd expect  
- Monitoring & alerting isn’t optional — it’s how you avoid "finding out" the hard way  
- Documentation saves you from your future self  


## Real World Use
I’ve already used a lot of what I learned here to freelance small jobs setting up services and basic infrastructure for local small businesses.

This repo is mostly for me — but if it helps someone else figure out how to start their own homelab, even better.
