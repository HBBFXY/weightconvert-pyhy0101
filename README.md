#weightconvert.py
weightstr=input("请输入带单位的体重：").strip()
if weightstr[-2:] in ['kg']:
    r=eval(weightstr[:-2])*2.2046
    print("转换后的体重为：{:.3f}pb".format(round(r,3)))
elif weightstr[-2:] in ['pb']:
    s=1/2.2046*eval(weightstr[:-2])-0.001
    print("转换后的体重为：{:.3f}kg".format(round(s,3)))
else:
    print("输入格式错误")
