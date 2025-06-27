# NITTC Credit Calculator (仮)

東京高専 (NITTC) の学生向け単位計算・履修管理アプリケーションです。
T3 Stack を用いて開発しています。

## 概要

このアプリケーションは、東京高専の学生が自身の履修状況を管理し、進級・卒業要件を満たしているかを確認するためのツールです。

**現在の開発スコープ:**
まずは、1年生が進級要件（全学生共通）を満たしているかを判定する機能の開発を目標としています。

## 主な機能 (計画中)

-   ✅ **1年生進級要件判定** (開発中)
-   GPA (Grade Point Average) の自動計算
-   卒業要件充足度の可視化
-   履修計画のシミュレーション

## 技術スタック

-   [Next.js](https://nextjs.org/)
-   [tRPC](https://trpc.io/)
-   [Prisma](https://www.prisma.io/)
-   [NextAuth.js](https://next-auth.js.org/)
-   [Tailwind CSS](https://tailwindcss.com/)
-   [TypeScript](https://www.typescriptlang.org/)

## 開発環境の構築

1.  **リポジトリをクローンします**
    ```bash
    git clone https://github.com/<your-username>/credit-calc-nittc.git
    cd credit-calc-nittc
    ```

2.  **依存関係をインストールします**
    ```bash
    npm install
    ```

3.  **環境変数を設定します**
    `.env.example` をコピーして `.env` ファイルを作成し、必要な値を設定してください。
    ```bash
    cp .env.example .env
    ```
    最低限、`AUTH_SECRET` を生成して設定する必要があります。
    ```bash
    # .env
    AUTH_SECRET="YOUR_GENERATED_SECRET"
    AUTH_DISCORD_ID="YOUR_DISCORD_ID"
    AUTH_DISCORD_SECRET="YOUR_DISCORD_SECRET"
    DATABASE_URL="file:./db.sqlite"
    ```

4.  **データベースのマイグレーションを実行します**
    これにより、`prisma/schema.prisma` の内容に基づいてデータベース (SQLite) のテーブルが作成されます。
    ```bash
    npm run db:generate
    ```

5.  **開発サーバーを起動します**
    ```bash
    npm run dev
    ```
    [http://localhost:3000](http://localhost:3000) でアプリケーションが開きます。

## コントリビューション

(今後設定予定)

## ライセンス

(今後設定予定)
