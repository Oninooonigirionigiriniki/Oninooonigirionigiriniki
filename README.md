# おにのおおにぎりおにぎりにき
## メンバー
* 上田剛瑠
* 梅田旭
* 仲宗根妃夏
* 喜納政凜

## 環境構築
### インストールするもの
* fvm : 3.2.1(最新)
* Flutter : 3.24.2(stable 最新)
* Android Studio : 2024.1(最新)
* GitHub Desktop

### 構築手順(Flutter・Android・fvm)
1. 以下のリンクから`Flutter`と`Android Studio`をインストールしてください。

    * [Flutter環境構築(Mac編)](https://zenn.dev/heyhey1028/books/flutter-basics/viewer/getting_started_mac)
    * [Flutter環境構築(Windows編)](https://zenn.dev/heyhey1028/books/flutter-basics/viewer/getting_started_windows)

2. fvmのインストール    
    ```
    // 以下のコードを実行してfvmをインストール
    dart pub global activate fvm

    // インストールしたfvmのバージョンが表示されればOK
    fvm --version
    ```
3. fvmでFlutterのバージョンの指定

    以下のコマンドを実行して、このプロジェクトで使用するFlutterのバージョンを指定します。
    ```
    fvm use 3.24.2
    ```
    以下のような質問がきたら「y」を入力します。
    ```
    Flutter "stable" is not installed.
    Would you like to install it? Y/n:
    ```
4. その他設定

    「.gitignore」ファイルに以下の文があるか確認し、一番下に追加してください。
    ```
    .fvm/
    ```

    「.vscode/setting.json」に以下のようにコードを追加してください。
    ```
    {
        "dart.flutterSdkPath": ".fvm/versions/3.24.2",

        -------- ここから --------
        // 検索対象からFVMのファイルを除外します。
        "search.exclude": {
            "**/.fvm": true
        },
        // ファイル監視対象からFVMのファイルを除外します。
        "files.watcherExclude": {
            "**/.fvm": true
        },
        -------- ここまで --------
    }
    ```
### 構築手順(GitHub Desktop)
1. 以下のURLからインストーラーをダウンロードする<br>
    * [https://desktop.github.com/download/](https://desktop.github.com/download/)
2. インストールする


## GitHub Desktopの使い方
参考 : [GitHub Desktopの使い方](https://www.kagoya.jp/howto/it-glossary/develop/githubdesktop/)

### リポジトリのclone
1. 上の「File」から「Clone repository...」を選択する
    <img hegith="300" src="image.png">

2. クローンしたいリポジトリ「Oninooonigirionigiriniki」を選択し、リポジトリをクローンする場所(自分の好きな場所)を選択する。
    <img heigth="300" src="image-1.png">

### fetch・pull

### commit

### push


## コミットメッセージの書き方
### テンプレート
```
[種類] (コミット要約)
```
### コミット種別
| 種類 | 説明 |
| :-- | --- |
| `Add` | 新規機能・ファイルの追加 |
| `Update` | 機能修正・変更 |
| `Fix` | バグ修正 |
| `Remove` | 機能・ファイル削除 |
| `Docs` | ドキュメント修正 |

### 例
```
[Add] ユーザー登録機能の追加
```

## ディレクトリ構成
```
```
