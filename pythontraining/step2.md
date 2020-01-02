<h2>If statements</h2>

```
number = 5
if number == 5:
    print("Number is 5)"
else:
    print("Number is NOT 5")
```{{execute}
For adding more conditions you could use and / or operators like "if number == 5 or number == 2:"

`if number == 5 or number == 2:`{{execute}
    `print("Number is 5 or 2)"`{{execute}

On numbers comparisson you could use < / > to determine if it´s bigger or smaller.


<h2>Lists</h2>

`student_names = ["Mark","Steve","Katalina"]`{{execute}}
`print(student_names)`{{execute}}

Like in other lenguages you can work with list indexes, by using student_name[1] you´ll see Steve name:
`print(student_names[1])`{{execute}}

Also it´s allowed to change the value of that position:
`student_names[1] = "Oliver"`{{execute}}
`print(student_names[1])`{{execute}}

Now instead of Steve you can see Oliver there.
For adding a new name use .append("new name")
`student_names.append("Steve")`{{execute}}

student_names[] == ["Mark","Oliver","Katalina","Steve"]

`student_names`{{execute}}

Some other build-in functions
"Mark" in student_name == True (it searchs for "Mark" in the array)

`"Mark" in student_names`{{execute}}

len(student_names) == gives you the number of elements in the array. 

`len(student_names)`{{execute}}

`del student_names[0]`{{execute}}  Deletes Mark

`print(student_names)`{{execute}}


<h2>Loops</h2>
for statement:

```
for name in student_names:
   print("Student name is {0}").format(name)

```{{execute}}



