# if语句

> 每条if语句的核心都是一个值为True或False的表达式，这种表达式被称为条件测试。 Python根据条件测试的值为True还是False来决定是否执行if语句中的代码。如果条件测试的值为True，Python就执行紧跟在if语句后面的代码；如果为False， Python就忽略这些代码。  

+ 比较运算符：$==、>、<、\leq、\geq、!=$

+ 布尔运算符:and、or、not

+ 检查特定值是否包含在列表中  

  ```python
  requested_toppings = ['mushrooms', 'onions', 'pineapple']
  print('mushrooms' in requested_toppings)
  # 输出 True
  ```

+ 布尔值有两个：True 和 False

# if-else 语句

> 经常需要在条件测试通过了时执行一个操作，并在没有通过时执行另一个操作；在这种情况下，可使用Python提供的if-else语句。 if-else语句块类似于简单的if语句，但其中的else语句让你能够指定条件测试未通过时要执行的操作。  

```python
age = 17
if age >= 18:
	print("You are old enough to vote!")
	print("Have you registered to vote yet?")
else:
	print("Sorry, you are too young to vote.")
	print("Please register to vote as soon as you turn 18!")
# 输出Sorry, you are too young to vote.
#Please register to vote as soon as you turn 18!
```

## if-elif-else 结构  

> 经常需要检查超过两个的情形，为此可使用Python提供的if-elif-else结构。 Python只执行if-elif-else结构中的一个代码块，它依次检查每个条件测试，直到遇到通过了的条件测试。测试通过后， Python将执行紧跟在它后面的代码，并跳过余下的测试。  

```python
age = 12
if age < 4:
	print("Your admission cost is $0.")
elif age < 18:
	print("Your admission cost is $5.")
else:
	print("Your admission cost is $10.")
# 输出Your admission cost is $5.
```

# 使用 if 语句处理[[列表简介|列表]]

+ 检查特殊元素  

  ```python
  requested_toppings = ['mushrooms', 'green peppers', 'extra cheese']
  for requested_topping in 				requested_toppings:
  	if requested_topping == 'green peppers':
  		print("Sorry, we are out of green peppers right now.")
  	else:
  		print("Adding " + requested_topping + ".")
  print("\nFinished making your pizza!")
  '''输出
  Adding mushrooms.
  Sorry, we are out of green peppers right now.
  Adding extra cheese.
  Finished making your pizza!'''
  ```

+ 确定列表不是空的  

  > 在运行for循环前确定列表是否为空很重要  

  ```python
  requested_toppings = []
  if requested_toppings:
  	for requested_topping in 	requested_toppings:
  		print("Adding " + requested_topping + ".")
  		print("\nFinished making your pizza!")
  else:
  	print("Are you sure you want a plain pizza?")
  '''
  输出 Are you sure you want a plain pizza?'''
  ```

  