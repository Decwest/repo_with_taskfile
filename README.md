# repo_with_taskfile
template for creating new repository with taskfile

## Task

### [インストール](https://taskfile.dev/installation/)

参考：UbuntuでTaskをインストールする場合
```shell
sudo sh -c "$(curl --location https://taskfile.dev/install.sh)" -- -d -b /usr/local/bin
```

### Taskfileのコマンド
- 現在のブランチでgit push
```shell
task push
```

- 現在のブランチでgit pull
```shell
task pull
```

- ruffで静的解析とフォーマットチェック
```shell
task ruff
```

- pyrightによる型チェック
```shell
task type-check
```

## uv

Pythonのパッケージ&プロジェクトマネージャ （poetry+pyenv的な）

### [インストール](https://docs.astral.sh/uv/getting-started/installation/)

参考：Ubuntuでuvをインストールする場合
```shell
curl -LsSf https://astral.sh/uv/install.sh | sh
```

### 環境構築

```shell
uv init
uv run hello.py
```
