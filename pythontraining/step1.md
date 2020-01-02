<h2>Hello World</h2>

For this training we will be using python3.6. In order to install it on our ubuntu console you should type:
`apt-get update`{{execute}}
Then
`sudo apt-get install python3.6`{{execute}}

Finally enter to python:
`python3.6`{{execute}}

 It´s not a code training if we don´t start with Hello World test:
 `print("Hello World!")`{{execute}}

<h2>Variables</h2>

 Variables, in python we don´t need to specified the type so we can just create a variable like:

 `hello = "Hello World!"`{{execute}}  
 `step = 1`{{execute}}

 `"{0} this is the step {1}".format(hello,step)`{{execute}} 

From python3.6 Also you can do it as:
`f"{hello} this is the step {step}"`{{execute}}


<h2>Integers and Float</h2>
 When using integers or float, you don´t need to convert them in order to perform operations. For example:

 `num_int = 42`{{execute}}  
 `num_float = 3.14159`{{execute}}
 `num_int +  num_float`{{execute}}  => this will show you 45.14159

 Also you can convert results by doing:
 `int(num_float)`{{execute}}  = 3 or  `float(num_int)`{{execute}}  = 42.0

<h2>Strings common functions</h2>

`"hello".capitalize()`{{execute}} => == "Hello"
`"hello".replace("e","a")`{{execute}} => == "Hallo"
`"hello".isalpha()`{{execute}} => True
`"123".isdigit()`{{execute}} =>  True
`"some,csv,values".split(",")`{{execute}} => == ['some','csv','values']

<h2>Boolean</h2>

In python boolean value can have True, False or None
`var_true = True`{{execute}}
`var_false = False`{{execute}}
`var_true`{{execute}}
`str(var_true)`{{execute}}
`int(var_true)`{{execute}}


