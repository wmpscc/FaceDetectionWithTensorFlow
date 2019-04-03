# 人脸检测

## 转换预训练模型
1. 从作者的厂库下载预训练模型[ResNet101-based pretrained model(hr_res101.mat)](https://www.cs.cmu.edu/~peiyunh/tiny/hr_res101.mat)
2. 运行以下代码转为pickle文件
```
python matconvnet_hr101_to_pickle.py 
        --matlab_model_path /path/to/pretrained_model 
        --weight_file_path  /path/to/pickle_file
```

## 预测
```
python tiny_face_eval.py
  --weight_file_path /path/to/pickle_file
  --data_dir /path/to/input_image_directory
  --output_dir /path/to/output_directory
```
## Result
![](test/result1.jpg)
![](test/result2.jpg)
![](test/result3.jpg)
![](test/result4.jpg)
![](test/result5.jpg)
![](test/result6.jpg)
![](test/result7.jpg)
![](test/result8.jpg)
![](test/result9.jpg)

> 本项目修改自[Tiny_Faces_in_Tensorflow](https://github.com/cydonia999/Tiny_Faces_in_Tensorflow)
