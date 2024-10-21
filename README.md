# 手写数字识别

## 项目概述

本项目是一个基于Python的深度学习应用，旨在通过卷积神经网络（CNN）和全连接神经网络（DNN）实现手写数字识别。项目包含两个主要的Python脚本：`Activators.py`、`CNN.py`、`DNN.py` 和 `app.py`。其中，`Activators.py` 定义了多种激活函数，`CNN.py` 实现了卷积神经网络的基本结构，`DNN.py` 实现了全连接神经网络的基本结构，而 `app.py` 是项目的图形用户界面（GUI），使用户能够绘制手写数字并进行识别。

## 环境依赖

- Python 3.x
- NumPy
- PIL (Python Imaging Library)

## 安装指南

1. 确保Python环境已安装。

2. 安装所需的库：

   ```bash
   pip install numpy pillow
   ```

## 使用说明

1. 运行 `app.py` 启动GUI程序。
2. 在GUI窗口中，使用鼠标在画布上绘制数字。
3. 点击“开始识别！”按钮，程序将处理绘制的数字并显示识别结果。

## 代码结构

- `Activators.py`：定义了多种激活函数，包括ReLU、Identity、Sigmoid和Tanh。
- `CNN.py`：实现了卷积层（`ConvLayer`）和最大池化层（`MaxPoolingLayer`）。
- `DNN.py`：实现了全连接层（`FullConnectedLayer`）。
- `app.py`：构建了GUI界面，并集成了CNN和DNN进行手写数字识别。

## 主要功能

- **手写数字绘制**：用户可以在GUI窗口中自由绘制手写数字。
- **数字识别**：通过集成的CNN和DNN模型，程序能够识别用户绘制的数字，并在界面上显示识别结果。
- **模型训练**：虽然代码中包含了模型参数的初始化，但实际的训练过程需要额外的数据和训练循环。