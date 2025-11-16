# Knowledge Base

!!! info "Welcome"
    My personal reference guide for frequently used commands, concepts, and best practices.

## 🚀 Quick Links

<div class="grid cards" markdown>

-   :fontawesome-brands-linux: **Linux**

    ---

    Commands, SSH, Systemd and more

    [:octicons-arrow-right-24: Go to Linux](linux/index.md)

-   :fontawesome-brands-git-alt: **Git**

    ---

    Version control workflows

    [:octicons-arrow-right-24: Go to Git](git/index.md)

-   :fontawesome-brands-docker: **Docker**

    ---

    Containers & Docker Compose

    [:octicons-arrow-right-24: Go to Docker](docker/index.md)

-   :material-kubernetes: **Kubernetes**

    ---

    k8s cluster management

    [:octicons-arrow-right-24: Go to Kubernetes](kubernetes/index.md)

-   :material-infinity: **DevOps**

    ---

    CI/CD, monitoring, infrastructure

    [:octicons-arrow-right-24: Go to DevOps](devops/index.md)

-   :material-vim: **Vim**

    ---

    Neovim configuration & commands

    [:octicons-arrow-right-24: Go to Vim](vim/index.md)

</div>

## 📝 Recent Updates

| Date | Topic | Description |
|------|-------|-------------|
| 2024-01-XX | Docker Networking | Bridge vs Host Mode |
| 2024-01-XX | Git Rebase | Interactive Rebase Tutorial |
| 2024-01-XX | kubectl | Port Forwarding Examples |

## 🎯 Frequently Used

### Docker Quick Start
```bash
# Start container
docker run -d --name myapp -p 8080:80 nginx

# View logs
docker logs -f myapp

### Git Quick Commands
```bash
# Quick commit
git add . && git commit -m "Update"

# Undo last commit (keep changes)
git reset --soft HEAD~1
```

### kubectl Essentials
```bash
# Pod logs
kubectl logs -f pod-name

# Port forward
kubectl port-forward service/myapp 8080:80
```

!!! tip "Navigation"
    Use the sidebar on the left for navigation or the search function (++ctrl+k++)
