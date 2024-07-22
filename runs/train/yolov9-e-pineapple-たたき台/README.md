## コマンド

```bash
python train_dual.py --workers 8 --device 0 --batch 8 --data data/pineapple.yaml --img 640 --cfg models/detect/yolov9-e.yaml --weights './weights/yolov9-e.pt' --name yolov9-e-pineapple --hyp hyp.scratch-pineapple.yaml --epochs 300 --close-mosaic 10 --patience 40
```

## 学習過程

![results.png](./results.png)

## 結果

![結果のスクショを同ディレクトリ内の`console.png`に保存してください](./console.png)
