---
layout: post
title: Hướng dẫn cài đặt TensorFlow trên Window
subtitle: 
tags: [tensorflow, DeepLearning] 
bigimg:  /img/tt.jpg
comments: true
---
TensorFlow là thư viện được sử dụng nhiều nhất trong các hệ thống Deep Learning hiện nay. Đặc trưng của TensorFlow là xử lý được tất cả các loại dữ liệu có thể biểu diễn dưới dạng data flow graph hay low level như xử lý chữ viết tay. Tensorflow được viết bằng C++ và Python. Hiện nay, có nhiều cách để cài đặt Tensorflow, chạy trên 1 hoặc nhiều CPU, GPU, di chuyển desktop, thậm chí cả smartphone cũng có thể sử dụng được.               
Sau đây tôi sẽ giới thiệu về cách cài đặt tensorflow trên Window với CPU.

## Yêu cầu
  1. Window 7/8/8.1/10 64bit
  2. Anaconda 4.2.0 với Python 3.5.x
  3. TensorFlow 1.0.1

**Bước 1: Cài đặt Anaconda với python 3.5** 
  Download: [Anaconda](https://repo.continuum.io/archive/Anaconda3-4.2.0-Windows-x86_64.exe)  
  - Mở Command prompt với quyền Administrator  
  - Nhập Python để kiểm tra phiên bản Python, Anaconda đang sử dụng                   
        *C:\WINDOWS\system32>python          
        Output: Python 3.5.3 |Anaconda custom (64-bit)| (default, May 15 2017, 10:43:23) [MSC v.1900 64 bit (AMD64)] on win32           
        Type "help", "copyright", "credits" or "license" for more information.*
  - Tắt Cmd
  
**Bước 2: Create installation environment**  
  - Mở Command prompt với quyền Administrator   
  - Create a conda environment named tensorflow by the command:                     
        *C:\> conda create -n tensorflow      
        Ouput: Fetching package metadata .........
        …                        
        Proceed ([y]/n)? y*                      
        *>Press Enter*           
  - Activate the conda environment:             
      *C:\> activate tensorflow*

**Bước 3: Cài đặt Tensorflow**
  - Tải và cài đặt Tensorflow bằng Command:                
      *(tensorflow)C:\> pip install --ignore-installed --upgrade https://storage.googleapis.com/tensorflow/windows/cpu/tensorflow-1.0.1-cp35-cp35m-win_amd64.whl*                 
  - Cài đặt thành công -> tiếp tục mở command lên để kiểm tra phiên bản của tensorflow:                
      *Type python       
      Type importtensorflow as tf                     
      Type print(tf.version__)                    
      Output: 1.01*
