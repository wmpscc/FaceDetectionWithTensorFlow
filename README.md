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
![](https://github.com/wmpscc/FaceDetectionWithTensorFlow/blob/master/test/result/1.jpg?raw=true)
![](https://github.com/wmpscc/FaceDetectionWithTensorFlow/blob/master/test/result/2.jpg?raw=true)
![](https://github.com/wmpscc/FaceDetectionWithTensorFlow/blob/master/test/result/3.jpg?raw=true)
![](https://github.com/wmpscc/FaceDetectionWithTensorFlow/blob/master/test/result/4.jpg?raw=true)
![](https://github.com/wmpscc/FaceDetectionWithTensorFlow/blob/master/test/result/5.jpg?raw=true)
![](https://github.com/wmpscc/FaceDetectionWithTensorFlow/blob/master/test/result/6.jpg?raw=true)
![](https://github.com/wmpscc/FaceDetectionWithTensorFlow/blob/master/test/result/7.jpg?raw=true)
![](https://github.com/wmpscc/FaceDetectionWithTensorFlow/blob/master/test/result/8.jpg?raw=true)
![](https://github.com/wmpscc/FaceDetectionWithTensorFlow/blob/master/test/result/9.jpg?raw=true)

> 本项目修改自[Tiny_Faces_in_Tensorflow](https://github.com/cydonia999/Tiny_Faces_in_Tensorflow)
