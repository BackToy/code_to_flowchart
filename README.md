# code_to_flowchart
TThe program will take as input - code, algorithm, workflow or manual and will give as output- a flowchart for it.
The code is written in python,I am using pygame for displaying flowchart.
first flowchart.py with some program as input frr eg: `python flowchart.py for.py t.flow` , then `python visualizer.py t.flow`
## example
```bash
> python flowchart.py examples/codes/for.py t.flow
print("List Iteration")
[<class 'node.OutputNode'>( "List Iteration") to None]
l = ["geeks", "for", "geeks"]
[<class 'node.OutputNode'>( "List Iteration") to <class 'node.Node'>(l = ["geeks", "for", "geeks"]) to None, <class 'node.Node'>(l = ["geeks", "for", "geeks"]) to None]
for i in l:
block node
[<class 'node.OutputNode'>( "List Iteration") to <class 'node.Node'>(l = ["geeks", "for", "geeks"]) to None, <class 'node.Node'>(l = ["geeks", "for", "geeks"]) to None, <class 'node.ConnectorNode'>() to None]
~print(i)
[<class 'node.OutputNode'>( "List Iteration") to <class 'node.Node'>(l = ["geeks", "for", "geeks"]) to None, <class 'node.Node'>(l = ["geeks", "for", "geeks"]) to None, <class 'node.ConnectorNode'>() to <class 'node.Node'>(~print(i)) to None, <class 'node.Node'>(~print(i)) to None]


> python visualizer.py t.flow
pygame 2.0.1 (SDL 2.0.14, Python 3.9.0)
Hello from the pygame community. https://www.pygame.org/contribute.html
OverflowError: Python int too large to convert to C long

The above exception was the direct cause of the following exception:

Traceback (most recent call last):
  File "D:\Documents\CAU\Lion\repositiries\Python\code_to_flowchart\visualizer.py", line 85, in <module>
    draw(begin, SCREEN, 100, 100)
  File "D:\Documents\CAU\Lion\repositiries\Python\code_to_flowchart\visualizer.py", line 48, in draw
    pygame.draw.ellipse(
SystemError: <built-in function ellipse> returned a result with an error set
```
# Note
1. 安装最新版node模块会报错，不安装能正常出结果
2. 第二步的时候报错说int型的值太大了，还有些pygame的bug，后面有空再修改吧。
