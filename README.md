# sveltekit-step1
My self-study repo of SvelteKit.

## 概要

SvelteKitの学習用リポジトリです。

## 前提条件

* Docker Desktopがインストールされている。
* Visual Studio Codeがインストールされている。
* Visual Studio Codeに`Dev Containers`拡張がインストールされている。

## 環境構築

1. Githubにリポジトリ `sveltekit-step1` を作成。
2. ローカルにクローン後、`sveltekit-step1` フォルダを Visual Studio Code で開く。
3. Docker Desktopを起動。
4. Visual Studio Code左下の`リモートウインドウを開く`から、`コンテナで再度開く`を選択。
5. `開発コンテナ-構成ファイルの追加`で`Ubuntu devcontainers`を選択し、インストールバージョンは`jammy (規定)` を選択。
6. `機能の選択`で`Node.js (via nvm), yarn and pnpm devcontainers`を選択し、インストールバージョンは`既定値を保持する`を選択。
7. Dev Containersが起動するので`Shift+control+^`でターミナルを開く。

## SvelteKitチュートリアル

SvelteKitの [ドキュメント](https://kit.svelte.jp/docs/introduction) に沿って学習を進める。

### プロジェクト作成

インタラクティブにプロジェクトを作成する。  
途中表示されるオプションはすべてデフォルト値を選ぶ。

```bash
npm create svelte@latest my-app

```

プロジェクトフォルダに移動し、依存関係をインストールする。

```bash
cd my-app
npm install
```

開発環境でサーバーを起動する。

```bash
npm run dev

> my-app@0.0.1 dev
> vite dev



  VITE v4.4.9  ready in 4076 ms

  ➜  Local:   http://localhost:5173/
  ➜  Network: use --host to expose
  ➜  press h to show help

  Shortcuts
  press r to restart the server
  press u to show server url
  press o to open in browser
  press c to clear console
  press q to quit
```

ローカルの `5173` ポートでサーバーが起動するので、Webブラウザで <http://localhost:5173/> にアクセスして確認。  
ターミナル上で `q` を入力すると終了する。
