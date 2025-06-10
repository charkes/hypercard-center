### container

<b>HyperTalk Definition </b> A place where you can store and retrieve a value.   

There are six types of containers in HyperCard: a variable, a button, a field, the selection, the Message box, and menus. 

<code><pre>
myVariable
[the] selection
the Message box
btn 3
bg btn "Names"
card field 1
bkgnd field "Total"
menu 2
menu "Edit"
</pre></code>

Additionally, you can refer to a button or field by its [ph:part]  number:

<code><pre>
card part 1
last background part
</pre></code>

<code><b></code>AppleScript Definition </b> An object that contains one or more other objects, known as elements of the container. In a reference, the container specifies where to find an object. You specify containers with the reserved words <code>of</code> or <code>in</code>.

You can also use the possesive form (<code>'s</code>) to specify containers. For example, in

<code><pre>
first window's name
</pre></code>

the container is <code>first window</code>. The object it contains is a name property. 