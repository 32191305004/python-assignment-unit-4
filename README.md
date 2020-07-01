# python-assignment-unit-4
In [ ]:
1.Write a Python program to read an entire text file.
In [2]:
f=open("python.txt","w")
f.close()
f=open("python1.txt","w")
f.write("hi guys")
f.close()
f=open("python1.txt","r")
str=f.read()
print(str)
f.close()
hi guys

2.Write a Python program to read first n lines of a file
In [3]:
a_file=open("file_name.txt","w")
f.close()
In [5]:
a_file = open("file_name.txt")
number_of_lines = 3
for i in range(number_of_lines):
    line = a_file.readline()
print(line)
3.Write a Python program to append text to a file and display the text.
In [ ]:
f=open("python.txt","w")
f.close()
In [ ]:
f=open("python1.txt","w")
f.write("hi guys")
f.close()
In [6]:
f=open("python1.txt","r")
print(f.read())
f.close()
hi guys

In [7]:
f=open("python1.txt","a")
s='''am 
   Fine'''
f.write(s)
f.close()
4.Write a Python program to read last n lines of a file.
In [9]:
def LastNlines(fname, N):
  with open(fname) as file:
    for line in (file.readlines() [-N:]):
      print(line, end ='')
if __name__ == '__main__':
  fname = 'File1.txt'
  N = 3
  try:
   LastNlines(fname, N) 
  except:
   print('File found')
File found

5.Write a Python program to read a file line by line store it into a variable.
In [ ]:
f1=open("test.txt","w")
f.close()
In [ ]:
f1=open("test1.txt","w")
f1.write("python program")
f.close()
In [13]:
f1=open('test1.txt').readlines()
print(f1)
['Python']

6.write a program to read a file line by line store it into a list
In [46]:
infile=open("test.txt","w")
f.close()
In [48]:
infile=open("test1.txt","w")
infile.write("python")
f.close()
In [47]:
infile = "test1.txt"
content_list = open(infile).readlines()
print (content_list)
['welcome\n', '     to\n', '    Python']

7.write a python program to read a file line by line store it into a array.
In [18]:
f2=open("test1.txt","w")
f.close()
In [21]:
f2=open("test1.txt","w")
s='''welcome
      to
     Python'''
f2.write(s)
f.close()
In [22]:
f2=("test1.txt")
content_array=open(f2).readlines()
print(content_array)
['welcome\n', '     to\n', '    Python']

8.Write a Python program to count the number of lines in a text file.
In [ ]:
f3=open("file.txt","w")
f3.close()
In [26]:
f3=open("file.txt","w")
s='''i
     like to
     Code'''
f3.write(s)
f3.close()
In [27]:
f3=open("file.txt","r")
s=f3.read()
print(len(s.split('\n')))
f.close()
3

9.write a python program to get the file size of a plain file.
In [32]:
file=open("test.txt","w")
f.close()
In [36]:
file=open("test.txt","w")
file.write("programming")
f.close()
In [38]:
import os
os.path.getsize("test.txt")
Out[38]:
11
10.write a python program to copy the contents of a file into another.
In [39]:
file1=open("f1.txt","w")
file1.close()
In [45]:
file1=open("f1.txt","w")
s='''welcome 
     to programming
     world'''
file1.write(s)
file1.close()
In [43]:
file2=open("f2.txt","w")
file1=open("f1.txt","r")
for line in file1:
  file2.write(line)
file1.close()
file2.close()
