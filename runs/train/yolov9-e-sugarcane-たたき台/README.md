## コマンド

```bash
python train_dual.py --device 0 \
    --workers 8 --batch 8 \
    --data data/sugarcane.yaml \
    --img 640 \
    --cfg models/detect/yolov9-e.yaml \
    --weights './weights/yolov9-e.pt' \
    --name yolov9-e-sugarcane --hyp hyp.scratch-sugarcane.yaml \
    --epochs 300 \
    --close-mosaic 10 \
    --patience 20
```

## 学習過程

![results.png](./results.png)

## 結果

![結果のスクショを同ディレクトリ内の`console.png`に保存してください](./console.png)
