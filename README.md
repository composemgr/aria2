## 👋 Welcome to aria2 🚀

Lightweight multi-protocol & multi-source download utility

## 📋 Description

Lightweight multi-protocol & multi-source download utility

## 🚀 Services

- **app**: p3terx/ariang:latest
- **server**: p3terx/aria2-pro:latest

## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/aria2/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/aria2" ~/.local/srv/docker/aria2
cd ~/.local/srv/docker/aria2
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install aria2
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:6880

## 📂 Volumes

- `./rootfs/config/aria2` - Data storage
- `./rootfs/data/downloads` - Data storage

## 🔍 Logging

```shell
docker compose logs -f app
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
