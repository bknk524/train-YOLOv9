# カスタムデータセット

Roboflowというサービスを使用してデーターセットを作成しています。詳細は[こちら](https://universe.roboflow.com/hoku/sugarcane-3vhxz)を参照してください。

学習や評価に使用するデータセットは[こちら](https://universe.roboflow.com/hoku/sugarcane-3vhxz/dataset/11)からダウンロードし、`train`, `valid`, `test`をここに配置してください。

## ディレクトリ構造

```plaintext
datasets/
    .gitignore
    README.md
    README.dataset.txt
    README.roboflow.txt
    train/
        images/
            ...
        labels/
            ...
    valid/
        images/
            ...
        labels/
            ...
    test/
        images/
            ...
        labels/
            ...
```
