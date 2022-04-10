# What is "static" in C++

1. Where place outside of class or function etc. block scope,
variable decorated by "static" front of it, this variable is only visiable by this translate unit.

2. When a *method* or *variable* inside class decorated by *static*, it is shared by all objects of this class, and you can call this method without initialize an object.
