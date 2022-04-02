# https-code-server

セキュアな code-server を一発構築します。

## Installation

```sh
git clone https://github.com/Atis9/https-code-server.git
cd https-code-server
cp acme.env.sample acme.env
cp code-server.env.sample code-server.env
```

### acme.env

- DEFAULT_EMAIL
  - 証明書を発効するために有効なメールアドレスを入力してください。

### code-server.env

- PASSWORD
  - code-server にアクセスするのに必要なパスワードを設定してください。
- VIRTUAL_HOST
  - code-server を公開するホスト名を設定してください。
- LETSENCRYPT_HOST
  - Let's Encrypt で証明書を発効するホスト名を設定してください。

## Usage

```
docker-compose up -d
```
