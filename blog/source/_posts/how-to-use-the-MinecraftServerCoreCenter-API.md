---
title: 如何使用MinecraftServerCoreCenter SDK
date: 2019-01-28 18:46:50
categories: MinecraftServerCoreCenter
---

- # SDK for Python
  - ###### 安装SDK依赖包
    ``` 
    pip install oss2
    ```
  - ###### 下载[key.py](https://drive.aoaoao.me/s/1tzyg2ya)
  - ###### SDK文档
    ```
    import oss2
    import key
    auth = oss2.Auth(AccessKeyId, AccessKeySecret)
    bucket = oss2.Bucket(auth, EndPoint, BucketName)
    # <yourLocalFile>由本地文件路径加文件名包括后缀组成，例如/users/local/myfile.txt
    bucket.get_object_to_file('<ObjectName>', '<LocalFile>')  
    ```