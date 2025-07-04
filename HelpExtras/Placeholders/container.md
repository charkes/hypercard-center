### container

<b>HyperTalk Definition</b>

A place where you can store and retrieve a value.   

There are six types of containers in HyperCard: a variable, a button, a field, the selection, the Message box, and menus.

```
myVariable
[the] selection
the Message box
btn 3
bg btn "Names"
card field 1
bkgnd field "Total"
menu 2
menu "Edit"
```

Additionally, you can refer to a button or field by its [ph:part]  number:

```
card part 1
last background part
```

<b>AppleScript Definition</b>

An object that contains one or more other objects, known as elements of the container. In a reference, the container specifies where to find an object. You specify containers with the reserved words `of` or `in`.

You can also use the possesive form (`'s`) to specify containers. For example, in

```
first window's name
```

the container is `first window`. The object it contains is a name property.
