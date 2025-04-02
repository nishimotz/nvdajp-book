# nvdajp-book
NVDA日本語版ガイドブック
Takuya Nishimoto

## セットアップ

1.  **仮想環境の作成:**
    ```bash
    uv venv
    ```
2.  **仮想環境のアクティベート:**
    ```bash
    source .venv/bin/activate
    ```
    (Windows の場合は `.\.venv\Scripts\activate`)
3.  **依存関係のインストール:**
    ```bash
    uv pip install -r requirements.txt
    ```

## ビルド

ドキュメントをビルドするには、以下のコマンドを実行します。

```bash
make html
```
ビルドされた HTML ファイルは `_build/html` ディレクトリに出力されます。
