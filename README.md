# PythonGUI
GUI for Python
# band label to entry 
#导入tkinter
from tkinter import *
#初始窗体
win=Tk()
win.geometry("400x200")
win.config(bg="#323232")

#定义函数，把输入内容绑定标签
def ok():
    t=en.get()
    lb.config(text=t)

#初始化标签
lb=Label(bg="#323232",fg="white",text="This is label")
lb.config(text="change")
lb.pack()

#输入框
en=Entry()
en.pack()

#函数实例化
btn=Button(text="OK",command=ok)
btn.pack()

#始终显示窗体
win.mainloop()
