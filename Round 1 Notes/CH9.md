## CH 9
___

Local variables and methods live on the stack. Instance variables live on the heap inside of objects that contain them.
You call the constructor when you make an object. Can call different constructors using different parameters for the 
same object, these are known as overloaded constructors. 

+ Can make a constructor that takes no arguments and makes a John Doe of the object type which can be edited post-construction.
  - If there is a constructor with arguments, you must make your own no-arg constructor.

+ super(<arguments>) lets you call or reference the parent object. this(<arguments>) lets you call or reference the current argument.
  - only one of those two things can be done in the same constructor.

An object is only alive as long as it's referenced. Once it is no longer referenced, the computer will begin to freely 
overwrite it as if it was never there, as needed.