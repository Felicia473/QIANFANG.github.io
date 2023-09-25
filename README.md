![image](https://github.com/Felicia473/QIANFANG.github.io/assets/78649678/8ce3c550-59a2-4b44-953b-5e315cbbed95)# QIANFANG.github.io
猜数字
import random

# 创建随机数
n = random.randrange(1, 100)
# 获取输入
guess = int(input("输入任意数值: "))

while n != guess:  # 判断是否正确
    # 小于
    if guess < n:
        print("太小了")
        guess = int(input("再次输入数值: "))
    # 大于
    elif guess > n:
        print("太大了!")
        guess = int(input("再次输入数值: "))
    else:
        break
print("真棒，你猜对了!!")
