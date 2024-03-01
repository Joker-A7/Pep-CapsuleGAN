# Pep-CapsuleGAN
论文的实现
## 要求
本项目使用依赖如下：
```
Python 3.9.18
fair-esm 2.0.0
pandas 1.3.5
numpy 1.21.6
scikit-learn 1.0.2
torch 1.13.0+cu116
tensorflow 2.6.0
keras 2.6.0
```
如缺少其他库，可自行使用命令安装`pip install package_name==2.0.0`

## 使用
注意：数据集使用 0 和 1 分别表示高活性和低/无活性。  
### 提取特征
您只需要在 __iFeature_exteactor__ 中
