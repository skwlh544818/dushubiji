# input()

> 函数input()让程序暂停运行，等待用户输入一些文本。获取用户输入后， Python将其存储在一个变量中  .
>
> ```python
> message = input("Tell me something, and I will repeat it back to you: ")
> print(message)
> # 输入 Tell me something, and I will repeat it back to you: Hello everyone!
> # 输出 Hello everyone!
> ```
>
> 使用函数input()时， Python将用户输入解读为字符串。  
>
> 使用函数int()，它让Python将输入视为数值。函数int()将数字的字符串表示转换为数值表示  。
>
> ```python
> height = input("How tall are you, in inches? ")
> height = int(height)
> if height >= 36:
> 	print("\nYou're tall enough to ride!")
> else:
>     print("\nYou'll be able to ride when you're a little older.")
> # 输入How tall are you, in inches? 71
> # 输出You're tall enough to ride!
> ```

# 求模运算

> 求模运算符（ %） 将两个数相除并返回余数  ,可判
> 断一个数是奇数还是偶数   。
>
> ```python
> number = input("Enter a number, and I'll tell you if it's even or odd: ")
> # 输入Enter a number, and I'll tell you if it's even or odd: 42
> number = int(number)
> if number % 2 == 0:
> 	print("\nThe number " + str(number) + " is even.")
> else:
> 	print("\nThe number " + str(number) + " is odd.")
> # 输出The number 42 is even.
> ```

# while循环 #while循环

while循环不断地运行，直到指定的条件不满足为止。  

+ 使用while循环

  ```python
  current_number = 1
  while current_number <= 5:
  	print(current_number)
  	current_number += 1
  '''
  输出 1
  2
  3
  4
  5'''
  ```

+ 使用 break 退出循环  

  > 立即退出while循环，不再运行循环中余下的代码，不管条件测试的结果如何，可使用break语句。 break语句用于控制程序流程.
  >
  > 在任何Python循环中都可使用break语句。例如，可使用break语句来退出遍历列表或字典
  > 的for循环。  

+ 在循环中使用 continue  

  > 返回到循环开头，并根据条件测试结果决定是否继续执行循环，可使用continue语句，它不像break语句那样不再执行余下的代码并退出整个循环  .
  >
  > ```python
  > current_number = 0
  > while current_number < 10:
  > 	current_number += 1
  > 	if current_number % 2 == 0:
  > 		continue
  > 	print(current_number)
  > '''输出
  > 1
  > 3
  > 5
  > 7
  > 9'''
  > ```

+ 使用 while 循环来处理列表和字典  

  > for循环是一种遍历列表的有效方式，但在for循环中不应修改列表，否则将导致Python难以跟踪其中的元素。要在遍历列表的同时对其进行修改，可使用while循环。

  - 在列表之间移动元素
  - 删除包含特定值的所有列表元素  
  - 使用用户输入来填充字典  