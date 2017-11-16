# Translation Guide - From Java to Python

Now that we're familiar with Java, it's time that we introduced Python. The two are very different languages,
with very different syntax, but there are some similarities. We'll start with a basic table outlining the
differences in style of the two languages.

|         **Java**            | **Python**                  |
|:---------------------------:|-----------------------------|
| statically typed            | dynamically typed           |
| verbose                     | concise                     |
| not compact                 | compact                     |
| only one class per file     | multiple classes per file   |
| explicit exception throwing | implicit exception throwing |
| overly complex file I/O     | simple file I/O             |
| non-mandatory indentation   | mandatory indentation       |

**Statically Typed Languages**, like Java, require that a programmer explicitly states the data type of a variable.
For instance, in the statement
```
int myInt = 1;
```
the variable data type is explicitly declared with the keyword *int*

**DynamicallyTyped Languages**, like Python, do not require that a programmer explicitly states the data type of 
a variable, and assigns the variable a data type implicitly by it's value. For instance, in the statement
```
myInt = 1
```
the compiler infers that *myInt* is an integer, because it stores integer data.

---

In Java, we have to use **Explicit Excepiton Throwing**, meaning that if a method throws an exception, it must
be explicitly stated in that method's signature as "throws Exception", otherwise, you will receive a compiler error.

Python uses **Implicit Exception Throwing**, which means that if a function throws an exception inside of it, or
calls a function that may throw an exception, it implicitly recognizes that the method throws an exception and the 
programmer does not have to do anything with the method signature.  

---

**Non-Mandatory Indentation** in the context of Java refers to the programmers ability to stylize their code however
they choose, so long as the control symbols ({ } ( ) ;) are all typed correctly.

**Mandatory Indentation** is used in Python because there are no control symbols, so the compiler needs a way to 
parse our code and understand what the programmer intends.

------------------------

Now that you have a good understanding of how the languages differ on a higher level, let's look at some syntax differences.

# Declaring Variables

| **Java**                                  | **Python**                     |
|-------------------------------------------|--------------------------------|
| `data-type variableName = valueOrObject;` | `variableName = valueOrObject` |

# Declaring Methods

| **Java**                                                    | **Python**              |
|-------------------------------------------------------------|-------------------------|
| `access-modifier return-type name(argumentType argument) {` | `def method(argument):` |
| '    ...'                                                   | `    ...`               |
| `}`                                                         | ``                      |

---
# Control Statements
---

# For Loop

| **Java**                                                        | **Python**                                   |
|-----------------------------------------------------------------|----------------------------------------------|
| `for (variable-declaration; escape-condition; change-variable)` | `for variable in xrange(start, stop, step):` |

# For-Each Loop

| **Java**                          | **Python**             |
|-----------------------------------|------------------------|
| `for (ObjectType object : array)` | `for object in array:` |

# While-loop

| **Java**                          | **Python**                       |
|-----------------------------------|----------------------------------|
| `while (booleanExpressionIsTrue)` | `while booleanExpressionIsTrue:` |

# If-Else If-Else Ladders

| **Java**                                | **Python**                      |
|-----------------------------------------|---------------------------------|
| `if (booleanExpressionIsTrue) {`        | `if booleanExpressionIsTrue:`   |
| '    ...'                               | `    ...`                       |
| `} else if (booleanExpressionIsTrue) {` | `elif booleanExpressionIsTrue:` |
| '    ...'                               | `    ...`                       |
| '} else {'                              | `else:`                         |
| '    ...'                               | `    ...`                       |
| '}'                                     |                                 |

# Exception Handling

| **Java**                               | **Python**                            |
|----------------------------------------|---------------------------------------|
| `try {`                                | `try:`                                | 
| '    ...'                              | `    ...`                             |
| `    // code that may throw exception` | `    # code that may throw exception` |
| '    ...'                              | `    ...`                             |
| '} catch (Exception ex) {'             | `except Exception:`                   |
| '    ...'                              | `    ...`                             |
| '    // code that handles exception'   | `    # code that handles exeption`    |
| '    ...'                              | `    ...`                             |
| '}'                                    |                                       |

---

# WHAT'S DIFFERENT

Python does not have a do-while loop, or a switch-case control statement. 

# WHAT'S THE SAME

The following keywords are shared between Java and Python, and have the same function:
- class
- break
- continue
- for
- while
- return
- import
- try
- finally
- lambda

Keywords reserved in Java
![Java keywords](http://www.f5java.com/images/java-tutorial-keywords-in-java.jpg)
Keywords reserved in Python
![Python keywords](https://image.slidesharecdn.com/pythonfoundation-150317062910-conversion-gate01/95/python-foundation-a-programmers-introduction-to-python-concepts-style-51-638.jpg?cb=1448623649)

---

# Final Thoughts

While this guide serves as a thourough overview of the similarities and differences between Java and Python,
in the end the only true way for you to learn Python is to start programming with it, like any other new programming
language, and try these features out for yourself. 