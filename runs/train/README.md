このREADMEは工事中です

# 学習後の保存方法について

## trainのディレクトリ構造

学習後の結果は`runs/train/<--name(番号)>`に保存されます。`<--name(番号)>`は学習時にコマンドで指定したnameオプションの値です。<br>
同じnameオプションの値を指定した場合、`<--name(番号)>`の値がインクリメントされます。

そのディレクトリの中身は、学習結果の可視化, モデルの重みファイル, ログファイルなどが保存されています。

## 学習後について

学習でよいスコアが出た場合は、`runs/train/<--name(番号)>/`にREADME.mdを作成してください。

その際のREADME.mdのフォーマットは以下の通りです。

コマンドに学習時のコマンドを、結果に学習後のコンソール画面のスクショパス(console.png)を記載してください。

````markdown
## コマンド

```bash
# ここに学習時のコマンドを記載してください

例:
python train_dual.py --device 0 \
    --workers 8 --batch 8 \
    --data data/sugarcane.yaml \
    --img 640 \
    --cfg models/detect/yolov9-e.yaml \
    --weights './weights/yolov9-e.pt' \
    --name yolov9-e-sugarcane \
    --hyp hyp.scratch-sugarcane.yaml \
    --epochs 300 \
    --close-mosaic 15
```

## 学習過程

![results.png](./results.png)

## 結果

![結果のスクショを同ディレクトリ内の`console.png`に保存してください](./console.png)
````

READMEの例は`./yolov9-e-sugarcane-たたき台/README.md`を参照してください。

## モデルの保存

現在GitHubに上がっているスコアより良いモデルができた場合、<<たぶんfuggingface>>に`best.pt`をアップロードしてください。
