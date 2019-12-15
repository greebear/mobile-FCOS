# mobile-fcos

## 项目安装
```bash
cd mobile-fcos
pip3 install -r requirements.txt
python3 setup.py install
```

## 模型下载

- 模型下载地址: https://cloudstor.aarnet.edu.au/plus/s/jdtVmG7MlugEXB7/download
```bash
mkdir  mobile-fcos/models/
mv FCOS_imprv_dcnv2_X_101_64x4d_FPN_2x.pth mobile-fcos/models/
```

## 数据移动
```bash
cp  CYCD20191125done mobile-fcos/demo/
mv CYCD20191125done images
```

## 数据推理
```bash
cd mobile-fcos
python3 demo/fcos_demo.py

```

## 推理结果
结果以图片形式保存在 mobile-fcos/demo/images_predict
