# 🎉 Docker Trust Sign

Docker Content Trust (DCT) ensures the integrity and authenticity of Docker images by signing them with cryptographic keys. This allows users to verify the source and content of images, preventing unauthorized modifications and ensuring secure deployments.

![version](https://img.shields.io/badge/version-1.0-blue)
![rating](https://img.shields.io/badge/rating-★★★★★-yellow)
![uptime](https://img.shields.io/badge/uptime-100%25-brightgreen)

### ✍️ Sign

- Create Digital Signature

```shell
docker trust key generate signature
```

- Add Signer for Sign Repository with Public Key

```shell
docker trust signer add --key signature.pub signature natthasath/docker-trust-sign
```

- Trust Sign Image

```shell
docker trust sign natthasath/docker-trust-sign:latest
```

- Inspect Sign Image

```shell
docker trust inspect --pretty natthasath/docker-trust-sign
```

- Enable Docker Content Trust (DCT) for Sign Image

```shell
set DOCKER_CONTENT_TRUST=1
```

- Pull Sign Image

```shell
docker pull natthasath/docker-trust-sign
```

### 🥈 Run

- [http://localhost:8000/docs](http://localhost:8000/docs)

```shell
docker-compose up -d
```
