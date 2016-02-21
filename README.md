# lipeineng.github.io
李培能的博客

关于python的基础知识

Python文件命名时不要有中文，不然在dos中不能执行

D:\Program Files\Py>Python hellyy.py
Year:2016
Month(1-12):1
Day(1-31):1
January 1st. 2016

【环境变量】
D:\Program Files\Python;

【字符串转义】
"Let's go!"
'"Hello, world!" she said'
'Let\'s go'



【序列】
Python包含六中内建的序列
列表 元组 字符串 Unicode字符串 buffer对象 xrange对象
通用序列操作有 ：
索引，          >>>greeting='Hello'  
				>>>greeting[0]
				'H'
分片，          >>>numbers=[1,2,3,4,5,6,7,8,9,10]  
				>>>numbers[3:6] 
				[4,5,6]
加，            >>>[1,2,3]+[4,5,6]   
				[1,2,3,4,5,6]  
				>>>'Hello.'+'world'  
				'Hell.world'
乘，            >>>'python'*5  
				'pythonpythonpythonpythonpython'  
				>>>[42]*4 
				[42,42,42,42]
判断是否属于，  >>>premissions='rw'  
				>>>'w' in premissions  
				True
长度计算，      >>>numbers=[100,34,678]  
				>>>len(numbers) 
				3
最大，          >>>numbers=[100,34,678]  
				>>>max(numbers) 
				678
最小            >>>numbers=[100,34,678]  
				>>>min(numbers) 
				34

【列表】
list函数                >>>list('Hello')
						['H','e','l','l','o']
改变列表，元素赋值      >>>x=[1,1,1] 
						>>>x[1]=2
						>>>x
						[1,2,1]
删除元素                >>>names =['Alice','Beth','Cecil','Dee-Dee','Earl']    
						>>>del names[2]
						>>>names
						['Alice','Beth','Dee-Dee','Earl']
分片赋值                >>>name=list('Perl')     //改变   
                        >>>name
						['P','e','r','l']
						>>>name[1:]=list('ython')
						>>>name
						['P','y','t','h','o','n']
						
						>>>numbers=[1,5]        //插入
						>>>numbers[1:1]=[2,3,4]
						>>>numbers
						[1,2,3,4,5]
						>>>numbers[1:4]=[]      //删除 
						>>>numbers
						[1,5]
						
列表的方法              >>>list=[1,2,3]        //append
						>>>list.append(4)
						>>>list
						[1,2,3,4]
						>>>['to','be','or','not','to','be'].count('to')   //count 统计某个元素在列表中出现的次数
						2
					    >>>a=[1,2,3]            //extend 可以用新列表扩展原有的列表
						>>>b=[4,5,6]
						>>>a.extend(b)
						>>>a
						[1,2,3,4,5,6]
						>>>a=[1,2,3]            //+  返回的是一个全新的列表，而不是扩展的a
						>>>b=[4,5,6]
						>>>a+b												
						[1,2,3,4,5,6]
						>>>a
						[1,2,3]
						>>>knights=['We','are','the','knights','who','say','ni']  //index
						>>>knights.index('who')    //搜索不存在的单词时会报异常
						4
						>>>numbers=[1,2,3,4,5,6,7]    //insert 用于将对象插入到列表中
						>>>numbers.insert(3,'four')
						>>>numbers
						[1,2,3,'four',5,6,7]
						>>>x=[1,2,3]             //pop方法会移除列表中的一个元素（默认是最后一个）
						>>>x.pop()                  并且返回该元素的值
						3
						>>>x
						[1,2]
						>>>x.pop(0)
						1
						>>>x
						[2]
						>>>x=['to','be','or','not','to','be']  //remove 用于移除列表中某个值的第一个匹配项
						>>>r.remove('be')
						>>>x
						['to','or','not','to','be']
						>>>x=[4,6,2,1,7,9]                    //sort 对列表进行排序
						>>>x.sort()                           //.sort方法不会有返回值 
						>>>x
						[1,2,4,6,7,9]    
						>>>y=x[:]                  //复制1 正确的复制，会复制出两份列表
						>>>y.sort()
						>>>x
						[4,6,2,1,7,9]
						>>>y
						[1,2,4,6,7,9]
						>>>y=x                     //复制2 这样的复制，只是让x和y指向了同一个列表，改了一个，另一个也会改
						>>>y.sort()
						>>>x
						[1,2,4,6,7,9]
						>>>y
						[1,2,4,6,7,9]
						>>>y=sorted(x)             //sorted 获取已排序的列表的副本的方法
						>>>x
						[4,6,2,1,7,9]
						>>>y
						[1,2,4,6,7,9]            
						>>>numbers=[5,2,9,7]       //高级排序
						>>>numbers.sort(cmp)       //cmp 提供了比较函数的默认实现方式 
						>>>numbers
						[2,5,7,9]
						>>>x=['aardvark','abalone','acme','add','aerate']  //key 让所有元素根据key来进行排序
						>>>x.sort(key=len)
						>>>x
						['add','acme','aerate','abalone','aardvark'] 
						>>>x=[4,6,2,1,7,9]                                 //reverse表示是否需要进行反向排序 
						>>>x.sort(reverse=True)
						>>>x
						[9,7,6,4,2,1]

【元组】	 		//不可变序列			
						
						
						
						
						
						
						
						
						
						
						
						
						
						
						
						
						
