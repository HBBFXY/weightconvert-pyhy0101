def weight_converter():
    input_str = input().strip()

    if input_str.endswith('kg'):
        kg = float(input_str[:-2])
        pd = kg * 2.2046
        print(f"对应的英制重量为{pd:.3f}磅") 
    elif input_str.endswith('pd'):
        pd = float(input_str[:-2])
        kg = pd / 2.2046 - 0.001
        print(f"对应的公制重量为{kg:.3f}公斤")
    else:
        printf("输入格式错误, 请以kg或pd结尾")
if __name__ == "__main__":
    weight_converter()
