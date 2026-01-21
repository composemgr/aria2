## 👋 Welcome to aria2 🚀

Aria2 - Lightweight multi-protocol download utility

## 📋 Description

Aria2 is a lightweight multi-protocol & multi-source command-line download utility supporting HTTP/HTTPS, FTP, SFTP, BitTorrent and Metalink. Web UI included for easy management.

## 🚀 Services

- **app**: Aria2 with AriaNg web UI (`p3terx/aria2-pro:latest`)

## 📦 Installation

### Using curl
```shell
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/aria2/main/docker-compose.yaml" | docker compose -f - up -d
```

### Using git
```shell
git clone "https://github.com/composemgr/aria2" ~/.local/srv/docker/aria2
cd ~/.local/srv/docker/aria2
docker compose up -d
```

### Using composemgr
```shell
composemgr install aria2
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
SERVICE_USER=1000
SERVICE_GROUP=1000
RPC_SECRET=changeme_rpc_secret     # RPC authentication token
RPC_PORT=6800                      # RPC listen port
LISTEN_PORT=6888                   # BT listen port
```

## 🌐 Access

- **Web UI**: http://172.17.0.1:60048
- **RPC**: http://172.17.0.1:6800/jsonrpc
- **RPC Secret**: Use value from RPC_SECRET env var

## 📂 Volumes

- `./rootfs/config/aria2` - Configuration files
- `./rootfs/data/downloads` - Downloaded files

## 🔍 Logging

```shell
docker compose logs -f app
```

## 🛠️ Management

```shell
docker compose up -d
docker compose down
docker compose pull && docker compose up -d
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
