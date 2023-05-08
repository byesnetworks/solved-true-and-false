Download Link: https://assignmentchef.com/product/solved-true-and-false
<br>
Consider the interface below, implement two classes True and False where each of them implements the Bool class. The function logicalAnd is similar to the primitive &amp;&amp; with no short circuiting, and the function ifThenElse accepts two CodeBlock objects and the first argument would be executed if the Bool object is True, second argument would be executed instead if the Bool object is False.

interface Bool {

Bool logicalAnd();

void ifThenElse(CodeBlock b1, CodeBlock b2);

}

For example, the code snippet below would print the string “bye world!”.

Bool b1 = new True();

Bool b2 = new False();

Bool b3 = b1.logicalAnd(b2);

b3.ifThenElse(new CodeBlock() {

public void execute() {

System.out.println(“hello world!”);

}

},

new CodeBlock() {

public void execute() {

System.out.println(“bye world!”);

}

});

The implementation must not contain any keywords instanceof, if, else, and it also must not use primitive types such as int, boolean and built-in classes such as String.