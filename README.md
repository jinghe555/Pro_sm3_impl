# 项目名称
sm3_implement
# 项目简介
SM3是我国采用的一种密码散列函数标准，由国家密码管理局于2010年12月17日发布。相关标准为“GM/T 0004-2012 《SM3密码杂凑算法》”。

在商用密码体系中，SM3主要用于数字签名及验证、消息认证码生成及验证、随机数生成等，其算法公开。据国家密码管理局表示，其安全性及效率与SHA-256相当。

在信息安全中，有许多重要的应用，都使用了密码散列函数来实现，例如数字签名，消息认证码。

对长度为l(l < 264) 比特的消息m， SM3杂凑算法经过填充和迭代压缩，生成杂凑值，杂凑值长度为256比特。
# 完成人
何静
# 项目流程
## 填充
![image](https://user-images.githubusercontent.com/104714591/181270605-8b7236a1-03e3-4af2-974d-b54ea9b63200.png)
## 迭代压缩
![image](https://user-images.githubusercontent.com/104714591/181270757-3c069702-9cbd-4d0d-b50b-d3f6d3670592.png)
## 消息扩展
![image](https://user-images.githubusercontent.com/104714591/181270853-0e13dd4f-276f-4840-aaed-d8d8c5dfab4d.png)
## 压缩函数
![image](https://user-images.githubusercontent.com/104714591/181271213-48714829-1548-47ee-a2fb-5a823c35a76f.png)
![image](https://user-images.githubusercontent.com/104714591/181271260-73e9cff8-e77d-415c-a8b9-df3b744f431d.png)
# 部分代码说明
(详尽注释说明见代码）
## string padding(string str)
消息填充
## string extension(string str)
消息扩展
## string compress(string str1, string str2）
消息压缩
## string iteration(string str)
迭代压缩
# 运行过程截图
![image](https://user-images.githubusercontent.com/104714591/181269645-38746442-4548-4d2c-986d-489b9bfeae26.png)
# 引用参考
[1]https://blog.csdn.net/cg129054036/article/details/83032978
[2]https://blog.csdn.net/qq_40662424/article/details/121637732?spm=1001.2101.3001.6661.1&utm_medium=distribute.pc_relevant_t0.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7Edefault-1-121637732-blog-125517692.pc_relevant_vip_default&depth_1-utm_source=distribute.pc_relevant_t0.none-task-blog-2%7Edefault%7EBlogCommendFromBaidu%7Edefault-1-121637732-blog-125517692.pc_relevant_vip_default&utm_relevant_index=1
