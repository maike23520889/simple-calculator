# simple-calculator
一个简单的 Python 计算器
def calculator():
    print("简单计算器")
    num1 = float(input("输入第一个数字: "))
    op = input("输入运算符 (+, -, *, /): ")
    num2 = float(input("输入第二个数字: "))
    
    if op == '+':
        result = num1 + num2
    elif op == '-':
        result = num1 - num2
    elif op == '*':
        result = num1 * num2
    elif op == '/':
        result = num1 / num2 if num2 != 0 else "除数不能为0"
    else:
        result = "无效运算符"
    
    print(f"结果: {result}")

if __name__ == "__main__":
    calculator()
