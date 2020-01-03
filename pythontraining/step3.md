<H2>functions</H2>

In order to test functions we need to save it on files so we will quit from python console and return to linux command.

<kbd>Ctrl</kbd>+<kbd>D</kbd>

Once back in Linux we can create a new dir and file to start playing with functions

`mkdir tutorial`{{execute}}
`cd tutorial`{{execute}}

`vi function.py`{{execute}}

```students = []

def add_student(name):
    students.append(name)

def get_students():
    result=" "
    for s in students:
        result=result + s
    return result

add_student("Pablo")
add_student("Juan")

get_students()```{{execute}}

then save :wq

to execute the script:

`python function.py`{{execute}}
