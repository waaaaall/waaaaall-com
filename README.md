# Quick Start

このプロジェクトはHugoを使用しています。以下の手順で開発環境を構築できます。

## Windows環境

### 必要なツール

1. **Chocolatey**（パッケージマネージャー）
   ```powershell
   # PowerShellを管理者として実行し、以下のコマンドを実行
   Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
   ```

2. **Hugo**
   ```powershell
   # Chocolateyを使用してHugoをインストール
   choco install hugo -y
   ```

## macOS環境

### 必要なツール

1. **Homebrew**（パッケージマネージャー）
   ```bash
   # Homebrewのインストール
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. **Hugo**
   ```bash
   # Homebrewを使用してHugoをインストール
   brew install hugo
   ```

## 開発サーバーの起動（共通）

1. プロジェクトのルートディレクトリに移動
   ```bash
   cd プロジェクトディレクトリ
   ```

2. ローカルサーバーを起動
   ```bash
   # 下書き記事を含めて表示する場合
   hugo server -D

   # 公開記事のみ表示する場合
   hugo server
   ```

3. ブラウザで以下のURLにアクセス
   ```
   http://localhost:1313
   ```

## Profileページのアクセス方法

新しく追加されたProfileページにアクセスするには、以下のURLにアクセスしてください。
```
http://localhost:1313/profile/
```

## 注意点
- ファイルの変更は自動的に反映されます
- Windows環境ではPowerShellを管理者として実行する必要がある場合があります
- 初回起動時にエラーが出た場合は、ターミナルを開き直してください
- macOSでHomebrewのインストール後、ターミナルで指示された追加の設定手順がある場合は、それに従ってください 
