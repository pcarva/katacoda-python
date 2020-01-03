<h2>If statements</h2>

`number = 5
if number == 5:
    print("Number is 5")
else:
    print("Number is NOT 5")
`{{execute}}


For adding more conditions you could use and / or operators like if number == 5 or number == 2:

`if number == 5 or number == 2:
    print("Number is 5 or 2")
    `{{execute}}

On numbers comparisson you could use < / > to determine if it´s bigger or smaller.


<h2>Lists</h2>

`student_names = ["Mark","Steve","Katalina"]
print(student_names)`{{execute}}

Like in other lenguages you can work with list indexes, by using student_name[1] you´ll see Steve name:
`print(student_names[1])`{{execute}}

Also it´s allowed to change the value of that position:
`student_names[1] = "Oliver"
print(student_names[1])

`{{execute}}

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

`for name in student_names:
   print("Student name is {0}").format(name)`{{execute}}

<h2>Break and Continue</h2>

break is used to exit a loop statement, continue just skip the current position and keep looping the rest.

Once we find katalina it will exit:

`for name in student_names:
    if name == "Katalina":
        print("found: " + name)
        break
    print("Student name is {0}").format(name)`{{execute}}

Katalina won´t be displayed becase we are skipping it:

`for name in student_names:
    if name == "Katalina":
        continue             
    print("Student name is {0}").format(name)`{{execute}}


<h2>While loops</h2>

`x = 0
while x < 10:
    print("Count is {0}").format(x)
    x +=1 `{{execute}}

<h2>Dictionaries</h2>

Uses Json format, it allows you to store diferent keys and values, also we can create a list of dictionaries. Values can be any type. We can also create a nested dictionary in case one of the keys it´s also a dictionary.

`student = {
    "name": "Mark",
    "student_id": 15163,
    "feedback": None
}`{{execute}}

In order to get a value we can use the name of the key to find the value. If key doesn´t exists we will have an error, but we could use .get function to return a default value in case we couldn´t find the key.

`student["name"]`{{execute}}
`student.get("last_name","NotFound")`{{execute}}

There are other functions like .keys(), values(), the first one shows all the keys of the dictionary and the other one the values
`student.keys()`{{execute}}
`student.values()`{{execute}}
To update, delete values it´s like with a list.

List of dictionaries, it helps to do loops

`all_student = [
    {"name": "Mark","student_id": 15163,"feedback": None},
    {"name": "Oliver","student_id": 62555,"feedback": true},
    {"name": "Katalina","student_id": 12354,"feedback": false}
]`{{execute}}


<h2>Exception handler</h2>

In order to handler different exceptions to prevent the application to stop, we can add a try - except section between the lines we want to verify. Then we could catch a specific type of error or even an unknown one. For example you could have something like:

`try:
    last_name = student["last_name"]
except KeyError as error:
    print("Error finding last_name." + error)
except Exception as error:
    print("A different type of error: " + error)`{{execute}}

