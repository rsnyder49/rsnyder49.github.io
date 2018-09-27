---
layout: post
title:      "Object Orientation"
date:       2018-09-27 22:14:02 +0000
permalink:  object_orientation
---


We last talked about HTML and CSS and how these languages are used to create websites.  While their syntax might not look as clean as Ruby, Ruby's Object Orientation is deeper and more complex than anything I had previously learned.  What is an object? Simply put, it is a piece of data that stores information.  Not so simply put, it can be a variable, a data structure, a function, or a method, and as such, is a value in memory referenced by an identifier(source: https://en.wikipedia.org/wiki/Object_(computer_science)). 

My experience with Ruby and OO is based around Ruby class objects.  In this sense, an object is an instance of a class.  A class is a structure...or constructor.  It can contains attributes, methods, variables that the created objects know about(or sometimes dont know about) and constructs objects.

A brief look at classes and objects:

class Dog 
end 
Defines a class called "Dog"

dog = Dog.new 
This creates a variable called "dog" and calls on the "Dog" class to create a new instance of an object.  "dog" is the newly created object.  When you call the "dog" variable you'll see a return that looks something like: 
#<Dog:0xrandommemorynumbers>

But currently, this object isn't very useful.  It doesn't know any methods or even have any attributes like knowings its own name.  Let's give this dog a name and teach it bark. 

class Dog
  attr_accessor :name
	
	def bark 
	  puts "woof" 
	end
	
end

Now we can give this dog a name.

dog.name = "Ghost"
This uses a built in Ruby class method to give the dog the name of "Ghost".  We can now call on this name method and receive the dogs name as a return value

dog.name 
return value => "Ghost" 

Similarly, we can call on the bark method that we defined within the Dog class itself 

dog.bark 
return value => "woof" 

This Dog clas is still very limited in what it's objects can do or know.  But there is nothing stopping us from giving it the ability to know that our dog Ghost's owner's name is Jon Snow.  Or the ability to sit, eat and roll-over.  Object Orientation is great because it draws comparisons to things in the real world.  I'm sure you can think of hundreds of real world items that could be written as a class and then used to create your own objects!



	




