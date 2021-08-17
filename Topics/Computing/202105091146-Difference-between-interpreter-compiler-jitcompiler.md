# Difference between Intepreter, compiler, and JIT compiler

Languages such as JavaScript, Python, Java are merely language written for humans to communicate with machines. They cannot understand what `print('Hello world')` actually means, rather they take source code and translate it into a machine understandable format (zeros and ones `0101110111010110` ). The difference between interpreter, compiler and JIT complier is the **Implementation**. 

## Interpreter:
Interpeters take source code instruction/statements chunk by chunk. For example: 
```python
def getAvg(*args):
	avg = sum(args)/len(args)
	return avg
	
def getText(text):
	text = input("Enter your text: ")
	return text
```

would translate to: 
```python
def getAvg(*args):
	010110101010100110101
	010110101101010101101

def getText(text):
	01111010101010101010
	101010010110101010101
```

Then the interpeter takes the first instruction(`def getAvg(*args)`) execute it and then goes to the next one. This is actually slower but it is easier to debug. Examples of programming languages that use interpreter Python, Ruby, PHP, perl.

`Bottom line: Slower, easier debugging`

## Compiler:
Unlike the interpeter, compilers take source code instructions as a whole, store them in memory and execute them. Faster than interpeters but debugging is a drawback here. With compilers, if there is an error in code it will carry on executing code and it is actually hard to debug for problems may occur like filling up memory and crashing system. Examples of compilers, C, C++, Scala. 

`Bottom line: Faster, harder debugging`

## JIT-Compiler:
Think about it as a combination of the two technologies. JIT-compiler have the goods of both sides. The JIT part of it is *interpreter* and Compiler means the instructions are converted into *machine code* making them very very fast. It takes the instructions only if it is called. For example, a set of instruction is first interpreted JIT, compiled and ran those instructions. Examples of JIT, JavaScript JIT Compliation

#interpreter #compiler #jit #jit-compiler
