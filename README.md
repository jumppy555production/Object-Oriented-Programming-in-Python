# Object-Oriented-Programming-in-Python
Object Oriented Programming (OOP) on Python / 13 Oct 2021


# "variable = values" Can be you to insert the value to a variable.
# "print(variable)" And this is how you print variable's value.

x = 15
print(x)

# "print(type(variable))" So you will know, What kind of this variable is.

x = 20
print(type(x))

# "print(variable.upper())" Here is a way to make a string in your code turn into a upper case.

string = "this is an upper case"
print(string.upper())

# "class text:" This is a class, Imagine this is a brain. And contains "methods" things to do.
# "def text(parameters):" A method contains parameters or things that contains in the situation. And you can write things to do in the situation.
# "class.method()" And this is how to print a method.

class Dog:
    def say_bark():
        print("Bark Bark Bark")
Dog.say_bark()

# "return equation" So when you have a parameter and already has a value, You can return the parameter with a new value.
# "parameter + number" So, this is not a variable. It's a parameter, So you need to write that parameter too.

class Calculator:
    def add_5(x):
        return x + 5

print(Calculator.add_5(5))

# "def __init__()" This method is special, When you called a class this method will be automatic class.
# "print("Text" + parameter)" You can join a string and a parameter, By using a plus sign.
# "def text(self)" is a common parameter in the old version of Python. But now it use just some situation.
# "variable = class(parameter)" This how you print a method with "__init__".

class Classroom:
    def __init__(self, name, age):
        print("My name is " + name + " And I am " + age + " years old.")

    def student(self):
        print("Don't ask me")

student_1 = Classroom("Mike", "13")

# "class text(class):" It's a easy way. Because you can copy a method from one to another.
# "self.parameter = parameter" It can store parameters. So you can print a specific parameter's value.
# "print("\n" + "text")" Can make a space in a whole line. Like you press enter 2 times.
# "instance = class(parameter, parameter)" It looks like a variable, But it called a instance. Because it contains parameter's value. in a class

class Animal:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def speak(self):
        print("\n" + "My name is " + self.name + " And I am " + self.age + " years old.")

class Cat(Animal):
    def meow(self):
        print("Meow")

class Dog(Animal):
    def bark(self):
        print("Bark")

Cat_1 = Cat("Billy", "12")
Cat_1.speak()
Cat_1.meow()

Dog_1 = Dog("Bob", "10")
Dog_1.speak()
Dog_1.bark()
