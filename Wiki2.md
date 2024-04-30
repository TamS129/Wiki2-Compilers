<!--- I added some html to our doc to allow for more freedom for text, images, etc. -->
<!--- To separate your paragraphs use the <p> brackets.Ex:
<p> insert your paragraph text here </p> -->

<!--- This method below is to indent our paragraphs to make it look neater. 
If you erase this our paragraph indents go away. - Tamara -->



<!--- End of Paragraph Indent -->

# <div align ="center"> Wiki 2: Compilers</br> <span style="font-size:0.5em;"> Written By: Jackson Kettel, Ken Cage, Kelvin Rajbhandari, Tamara Slone </span> </div>

## <div align = "center"> Introduction: Compilers and Their Purpose [Kelvin]</div>
<p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;A compiler is a fundamental software tool that translates high-level programming languages which are readable & comprehensible to humans, 
into low-level binary machine code, which computers can understand. This transformation process, known as compilation, is crucial in software 
development, bridging the gap between human ideas and computer execution. The purpose of a compiler is multifold: it translates programs into 
machine-readable instructions, helps make code independent of the platform, generates executable files of code and ensures that the code is free 
from errors. Compilers are essential for executing complex software applications efficiently. They are also used to check the syntax and semantics 
of the code, catching errors before the software is executed.
</p>

<p align = "center">
<img src="Images%2Fwiki2.png" width="700" height="700" />
</p>

## <div align = "center">The History of Compilers [Kelvin] </div>
<p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The development of compilers is intertwined with the history of computer science. During the early days of computing in the 1940s, programmers 
wrote instructions in binary code directly suited to machine hardware. The tedious nature of this process led to the development of assembly 
languages, which allowed programmers to use symbolic representations of machine instructions. The real shift came with the advent of high-level 
languages, which abstracted the programming process further from the machine language. The first significant high-level language was FORTRAN, 
developed in the 1950s by John Backus’ team at IBM. This development was closely followed by the creation of the first compiler for FORTRAN, 
which marked a pivotal moment in computing, allowing for more rapid and flexible program development. Throughout the 1960s and 1970s, the evolution 
of compilers was characterized by improvements in optimization techniques and error detection mechanisms, which greatly enhanced programming 
efficiency and machine performance. Languages such as COBOL and LISP were developed with their compilers, expanding the usability of computers 
in business and research.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;As computing power increased and the needs of software grew more complex, the functionality of compilers expanded. Modern compilers 
are now capable of performing complex optimizations on the code to improve execution speed and reduce resource consumption. They also 
play a critical role in the development environment, offering developers immediate feedback on errors and warnings.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In summary, compilers are indispensable to the development of software. They translate high-level language into machine code, 
enhance it for performance and ensure it is error-free. From their origins in the earliest days of programming to their current 
complex forms, compilers have grown to be indispensable tools in the arsenal of modern computer science. As technology evolves, 
the role of compilers continues to adapt, ensuring they remain at the heart of software development processes.
</p>

## <div align = "center"> 3 Phases of Compilers [Jackson] </div>
<p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;There are 3 main phases of compilers: The front end phase, the intermediate code optimization phase, and the back end phase. The <b>front end phase</b> involves scanning the source code provided to the compiler, and producing an intermediate representation of the code. This is produced through generating tokens based on the source code’s language, and evaluating if it is both syntactically and semantically correct. The <b>intermediate code optimization phase</b> is when the code produced by the front end is further optimized by generating machine independent code. By doing so, it makes it so that the program will be more optimal when translated to machine code, and can be further translated to machine code on different types of devices. Finally, the <b>back end phase</b> is when the optimized intermediate code is finally translated into machine code for the device it will be used on. This will include tasks directly related to hardware, such as allocating memory in registers or selecting instructions.
</p>

## <div align = "center"> Operations of the Compiler [Jackson] </div>
<p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Compilers have many operations that turn source code into machine code for the given computer. The first three operations of a compiler are part of the front end phase: lexical analysis, syntax analysis, and semantic analysis. Lexical analyzers reads the source code provided, and groups the read characters into lexemes. Lexemes are sequence alphanumeric characters that make up tokens, which are the basic building blocks of a programming language. When it identifies these tokens, it will produce an output containing all of the tokens as well as their locations in the program. The syntax analyzer takes the tokens from the lexical analyzer and ensures that the program follows the grammar rules defined by the programming language. If a syntax error is detected, the program will not compile and produce an error. If the syntax analyzer determines that the program is syntactically correct, it will produce an abstract syntax tree (AST) that represents the structure of the source code so it can be understood in future steps. Finally, the semantics analyzer checks if the abstract syntax tree is semantically correct. This involves type checking, looking for undeclared variables, incorrect function calls, and many other rules.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Once the first three operations are completed, the compiler will generate an intermediate representation of the source code using the intermediate code generator. This intermediate code that is generated is platform independent, meaning that it can be used by any machine. The next two steps will make it be able to run on the specific platform, as the machine code is specific to the computer being used. The code optimizer will then make the code take less memory and execute at fast speeds while maintaining the meaning of the code. During this step, both machine-dependent and machine-independent optimizations are made, which makes the output only usable by the system compiling the code.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The final operation of the compiler is to produce functional machine code that can be read by the intended machine. This is dependent on the type of assembler used by the machine, the hardware being used, and other factors relating to the system’s architecture. This code will be able to allocate memory in the cpu’s registers, perform instruction selection, and other hardware operations. The final result will be machine code that will be then used by the linker and loader to execute the program.
</p>

## <div align = "center"> Types of Compilers[Tamara] </div>

### <div align = "center"> Single Pass Compilers </div>
<p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;When observing the different types of compilers, one of the more "simple" design choices for a compiler 
would be the Single Pass Compiler. A <b> Single Pass Compiler </b> is a compiler that processes the source
code of a program from start to finish in one pass. Meaning unlike our other compiler types that scan and read the 
source code in multiple phases. Single pass compilers read and translate the source as the programming is running. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Despite having a faster run time and better resource management, Single Pass Compilers are very limited in terms of creating complex optimizations 
for the code it reads. Which can be a challenge to implement for complex languages because of its inability to revisit and reread the code. Which puts the compiler
at a major disadvantage comparative to Two Pass and Multi Pass compilers. However, while the Single Pass compiler may not be able to handle complex languages. What the Single Pass compilers do have an advantage in
is better resource management and speed than both Two Pass and Multi Pass compilers. Which makes the Single Pass compiler a better candidate for embedded systems, bootloaders, and scripting languages such as JavaScript. 
</p>

 <p align = "center">
<img src="Images%2FSinglePass_Compiler.png" width="800" />
</p>

### <div align = "center"> Two Pass Compilers </div>
<p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Another commonly used compiler is a Two-Pass Compiler. <b> Two Pass Compilers </b> are a type of Multi Pass compilers that read the source code
twice before running the program. Meaning unlike the previous Single Pass compiler, Two Pass compilers read through the source code once and then complete another
pass through of the source code. Two Pass Compilers are typically made up with a code scanner called a <b>lexical analyzer</b>. This lexical analyzer scans through a high level program and converts the scan
into a mix of identifying tokens. Once the lexical analyzer is complete the tokens are then sent to the second pass which is called a <b> syntax analyzer</b>. This syntax analyzer will take the tokens from the lexical analyzer
and parses the tokens. The syntax analyzer will parse the tokens into a tree and check to see if the program is written correctly. This two pass system can sometimes be referred to as 
Front end and Back end processes. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Two pass compilers and Multi Pass Compilers are actually very similar in the way the programs functions. The only difference is while Multi Pass compilers can three or more passes throughout its duration. Two Pass compilers only allow
for two passes through its program. Which allows the Two Pass compiler to have a faster runtime than a Multi Pass compiler. This also allows for the Two Pass compiler to have fewer limitations in optimization comparative to a
Single Pass Compiler. However, there are still some limitations that a Two Pass compiler cannot do. For example,  Two Pass compilers cannot handle complex optimizations of code like a Multi-Pass compiler. These compilers also cannot do effective type-checking which is something you can
typically find in Multi Pass compilers. Leaving Two Pass compilers to be best used with concepts like mutual recursion, dead code elimination, and for some programming languages like C++.
</p>

![TwoPassCompiler.png](Images%2FTwoPassCompiler.png)

### <div align = "center"> Multi Pass Compilers </div>
<p>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The last compiler type that is typically used  for programming languages is called a <b>Multi Pass Compiler</b>. Multi Pass compilers work by having multiple passes through a program before the program executes. Meaning that 
the source code will be read through multiple times before they are executed. Meaning that Multi Pass Compilers will read through the source code multiple times before a programs runs. There are two different methods that a 
Multi Pass compiler can implement to parse through their programs called <b> Multiple Stages </b>. The Multiple stage method can allow for the compiler to have different phases of code processing. For example Multi Pass compilers allow for
lexical and syntax analyzer just like the Two Pass compiler. However, Multi Pass typically tends to have an optimizer, type-checking, and a semantic analyzer.   

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Multi Pass compilers work similarly to Two-Pass compilers as they both contain a lexical analyzer and a syntax analyzer. Considering that Two Pass compilers are a type of Multi Pass compilers. 
Unlike Single Pass compilers and Two Pass compilers, Multi Pass compilers can allow for more complex optimization than Single Pass or Two Pass compilers. However, due to its ability to have several passes 
Multi Pass Compilers can have a slow runtime comparative to Single Pass and Two Pass compilers. Leading to Multi Pass compilers better suited for languages such as C++ or Java.  

</p>

![MultiPass_Complier.png](Images%2FMultiPass_Complier.png)

## <div align = "center">The Difference between a Complied and Interrupted Language [Ken] </div>
<p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Programming languages are typically divided into two categories: compiled and interpreted. This classification hinges on how the languages convert code into machine code, the form executable by a computer's hardware. Compiled languages, such as C and C++, necessitate the use of a compiler to translate the entire program into machine code prior to execution. In contrast, interpreted languages, like Python and JavaScript, are executed progressively by an interpreter, which reads and executes the code line by line.


### <div align = "center"> Use Cases, Advantages, and Disadvantages </div>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Compiled languages are well-suited for applications where performance and speed are paramount. For instance, system software, game development, and applications that require intensive numerical computations typically employ compiled languages. The chief advantage of these languages is their fast execution speed; since the code is pre-compiled into machine code, it can be executed directly and quickly. However, disadvantages include less flexibility for error correction during runtime and a longer initial development time due to the compilation process.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Interpreted languages, on the other hand, are preferred for projects where quick development and portability outweigh execution speed. These languages are commonly used for web development, scripting, and automation tasks. The benefits of interpreted languages include easier debugging and testing, as errors can be rectified immediately without recompilation. Additionally, these languages tend to be more user-friendly and flexible. The primary drawback, however, is slower performance compared to compiled languages, due to runtime interpretation which can delay execution.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Practically speaking, the decision between using a compiled or interpreted language often depends on the specific needs of the project. Compiled languages offer efficiency and are ideal for performance-sensitive applications with stable requirements, while interpreted languages provide greater flexibility and quicker development times for projects where these aspects are prioritized.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;While compiled languages deliver superior performance and efficiency, they lack the debugging ease and flexibility that interpreted languages afford. Conversely, while interpreted languages support rapid development and are user-friendly, they experience slower execution times. Understanding these trade-offs is essential for developers when choosing the language that best suits the needs of their specific project.

## <div align = "center" > Sources </div>
[1]
“Compiler,” Wikipedia, May 03, 2020. https://en.wikipedia.org/wiki/Compiler

[2]
“What is Compiler? Definition, Structure, Types, Applications,” Toppr-guides, Jan. 12, 2021. https://www.toppr.com/guides/computer-science/computer-fundamentals/system-software/compiler/

[3]
 “Difference between Compiled and Interpreted Language,” GeeksforGeeks, Mar. 26, 2020. https://www.geeksforgeeks.org/difference-between-compiled-and-interpreted-language/

[4]
“Stack Overflow Developer Survey 2020,” Stack Overflow. https://survey.stackoverflow.co/2020#overview (accessed Apr. 30, 2024).

[5]
“Single Pass vs Two-Pass (Multi-Pass) Compilers,” GeeksforGeeks, Mar. 13, 2019. https://www.geeksforgeeks.org/single-pass-two-pass-and-multi-pass-compilers/# (accessed Apr. 30, 2024).

[6]
“What is a Multi-Pass Compiler?,” www.computerhope.com. https://www.computerhope.com/jargon/m/multpass.htm (accessed Apr. 30, 2024).

## <div align = "center"> Phases and Operations of a Compiler [Tamara] </div>


<p align = "center">

![Flowchart.png](Images%2FFlowchart.png)

</p>


