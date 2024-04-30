# <div align ="center"> Wiki 2: Compilers</br> <span style="font-size:0.5em;"> Written By: Jackson Kettel, Ken Cage, Kelvin Rajbhandari, Tamara Slone </span> </div>

## <div align = "center"> Introduction: Compilers and Their Purpose [Kelvin]</div>
<p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; When a software engineer is developing code, the programming language needs to be readable and easy to comprehend for the human mind. Thus came about <b>High-Level programming languages </b> which are human friendly and easy to understand, but not by machines. On the other hand, <b>Low-level languages</b> are machine-friendly. They are impossible to understand and learn. This arises a need for a <b>compiler</b> that converts high-level languages into low-level languages that a machine understands. 
This transformation process, known as compilation, is crucial in software 
development, bridging the gap between human ideas and computer execution. The purpose of a compiler is multifold: it translates programs into 
machine-readable instructions, helps make code independent of the platform, generates executable files of code and ensures that the code is free from errors. Compilers are essential for executing complex software applications efficiently. They are also used to check the syntax and semantics of the code, catching errors before the software is executed.
</p>

<p align = "center">
<img src="Images%2Fwiki2.png" width="700" height="700" />
</p>

## <div align = "center">The History of Compilers [Kelvin] </div>
<p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The development of compilers is intertwined with the history of computer science. During the early days of computing in the 1940s, programmers 
wrote instructions in binary code directly suited to machine hardware. The tedious nature of this process led to the development of assembly 
languages, which allowed programmers to use symbolic representations of machine instructions. The real shift came with the advent of high-level 
languages, which abstracted the programming process further from the machine language. The first significant high-level language was FORTRAN, developed in the 1950s by John Backus’ team at IBM. This development was closely followed by the creation of the first compiler for FORTRAN, 
which marked a pivotal moment in computing, allowing for more rapid and flexible program development. Throughout the 1960s and 1970s, the evolution of compilers was characterized by improvements in optimization techniques and error detection mechanisms. These advancements greatly enhanced programming efficiency and machine performance. Languages such as COBOL and LISP were later developed with their own compilers, expanding the usability of computers in business and research.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;As computing power increased and the needs of software grew more complex, the functionality of compilers expanded. Modern compilers are now capable of performing complex optimizations on the code to improve execution speed and reduce resource consumption. They also play a critical role in the development environment, offering developers immediate feedback on errors and warnings.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In summary, compilers are indispensable to the development of software. They translate high-level language into machine code, enhancing it for performance and ensuring its error-free. From their origins in the earliest days of programming to their current 
complex forms, compilers have grown to be indispensable tools in the arsenal of modern computer science. As technology evolves, 
the role of compilers continues to adapt, ensuring they remain at the heart of software development processes.
</p>

## <div align = "center"> 3 Phases of Compilers [Jackson] </div>
<p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;There are 3 main phases of compilers: The front end phase, the intermediate code optimization phase, and the back end phase. The <b>front end phase</b> involves scanning the source code provided to the compiler and producing an intermediate representation of the code. This is produced through generating tokens based on the source code’s language, and evaluating if it is both syntactically and semantically correct. The <b>intermediate code optimization phase</b> is when the code produced by the front end is further optimized by generating machine independent code. It allows the code to be more easily translated into machine code on different types of devices. Finally, the <b>back end phase</b> is when the optimized intermediate code is fully translated into machine code for the device it will be used on. This will include tasks directly related to hardware, such as allocating memory in registers or selecting instructions.
</p>

## <div align = "center"> Operations of the Compiler [Jackson] </div>
<p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Compilers have many operations that turn source code into machine code for the given computer. The first three operations of a compiler are part of the front end phase: lexical analysis, syntax analysis, and semantic analysis. <b>Lexical analyzers</b> reads the source code provided, and groups the read characters into lexemes. Lexemes are sequence alphanumeric characters that make up tokens, which are the basic building blocks of a programming language. When it identifies these tokens, it will produce an output containing all of the tokens as well as their addresses in the program. The <b>syntax analyzer</b> takes the tokens from the lexical analyzer and ensures that the program follows the grammar rules defined by the programming language. If a syntax error is detected, the program won't compile and will produce an error. If the syntax analyzer determines that the program is syntactically correct, it will produce an <b>Abstract Syntax Tree (AST)</b> that represents the structure of the source code so it can be understood by the semantic analyzer. Finally, the <b>semantics analyzer</b> checks if the AST is semantically correct. This involves type checking, looking for undeclared variables, incorrect function calls, and many other rules.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Once the first three operations are completed, the compiler will generate an intermediate representation of the source code using the intermediate code generator. This intermediate code that is generated is platform independent, meaning that it can be used by any machine. The next two steps will make it runnable on the specific platform, as the machine code is specific to the computer being used. The code optimizer will then optimize the code, requiring less memory, and executing at fast speeds while maintaining the meaning of the code. During this step, both machine-dependent and machine-independent optimizations are made, making the output only usable by the system compiling the code.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The final operation of the compiler is to produce functional machine code that can be read by the intended machine. This is dependent on the type of assembler used by the machine, the hardware being used, and other factors relating to the system’s architecture. This code will be able to allocate memory in the cpu’s registers, perform instruction selection, and other hardware operations. The final result will be machine code that will be then used by the linker and loader to execute the program.
</p>

## <div align = "center"> Types of Compilers[Tamara] </div>

### <div align = "center"> Single Pass Compilers </div>
<p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;When observing the different types of compilers, one of the more "simple" design choices for a compiler would be the Single Pass Compiler. A <b> Single Pass Compiler </b> is a compiler that processes the source code of a program from start to finish in one pass. Single Pass Compilers are unlike other compiler types that scan and read the source code in multiple phases. These compilers read and translate the source as the programming is running. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Despite having a faster run time and better resource management, Single Pass Compilers are very limited in terms of creating complex optimizations for the code it reads. This can be challenging to implement for complex languages because of its inability to revisit and reread the code. That is a major disadvantage compared to Two Pass and Multi Pass Compilers. While the Single Pass compiler may not be able to handle complex languages, they have better resource management and speed than both Two Pass and Multi Pass Compilers. This allows the Single Pass compiler to be a better candidate for embedded systems, bootloaders, and scripting languages such as JavaScript. 
</p>

 <p align = "center">
<img src="Images%2FSinglePass_Compiler.png" width="800" />
</p>

### <div align = "center"> Two Pass Compilers </div>
<p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Another commonly used compiler is a Two-Pass Compiler. <b> Two Pass Compilers </b> are a type of Multi Pass Compiler that reads the source code
twice before running the program. Two Pass Compilers typically use a lexical analyzer for their first read through of the source code. Once the lexical analyzer is complete, the translated code is then sent to the second pass, which contains a syntax analyzer. The syntax analyzer will parse the tokens into a tree and check to see if the program is written correctly. When that pass is complete, the code will then execute. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Two pass compilers and Multi Pass Compilers are actually very similar in the way the programs functions. The only difference is while Multi Pass compilers can have three or more passes throughout its duration, Two Pass compilers only allow for two passes. This allows the Two Pass compiler to have a faster runtime than a Multi Pass compiler, while also having less limitations in optimization than a Single Pass Compiler. However, there are still some limitations that a Two Pass compiler cannot do. For example, Two Pass compilers cannot handle complex optimizations of code like a Multi-Pass compiler. They also cannot do effective type-checking which is something you can
typically find in Multi Pass compilers. That leaves Two Pass compilers to be best used with concepts like mutual recursion, dead code elimination, and for some programming languages like C++.
</p>

![TwoPassCompiler.png](Images%2FTwoPassCompiler.png)

### <div align = "center"> Multi Pass Compilers </div>
<p>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The last compiler type is called a <b>Multi Pass Compiler</b>. Multi Pass compilers work by having multiple passes through a program before the program executes. Meaning that 
the source code will be read through multiple times before it is executed. One of the more common methods that Multi Pass Compilers use to implement multiple passes are multiple stages. Multiple stages allow for the compiler to have different phases of code processing. The most common layout for multiple stages is to structure the complier with a lexical and syntax analyzer, an optimizer, type-checking, and a semantic analyzer.   

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Multi Pass compilers work similarly to Two-Pass compilers as they both contain a lexical analyzer and a syntax analyzer. Unlike Single Pass compilers and Two Pass compilers, Multi Pass compilers can allow for more complex optimization. However, because of its ability to have several passes 
these compilers tend to have slower runtimes than Single Pass and Two Pass compilers. Leading to Multi Pass compilers better suited for complex programs and programming languages like C++.  

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

 <img src="Images%2FFlowchart.png" height="800" />

</p>


