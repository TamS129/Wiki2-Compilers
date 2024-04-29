<!--- I added some html to our doc to allow for more freedom for text, images, etc. -->
<!--- To separate your paragraphs use the <p> brackets.Ex:
<p> insert your paragraph text here </p> -->

<!--- This method below is to indent our paragraphs to make it look neater. 
If you erase this our paragraph indents go away. - Tamara -->



<!--- End of Paragraph Indent -->

# <div align ="center"> Wiki 2: Compilers</br> <span style="font-size:0.5em;"> Written By: Jackson Kettel, Ken Cage, Kelvin Rajbhandari, Tamara Slone </span> </div>

## <div align = "center"> Introduction: Compilers and Their Purpose [Kelvin]</div>
<p>
A compiler is a fundamental software tool that translates high-level programming languages which are readable & comprehensible to humans, 
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
The development of compilers is intertwined with the history of computer science. During the early days of computing in the 1940s, programmers 
wrote instructions in binary code directly suited to machine hardware. The tedious nature of this process led to the development of assembly 
languages, which allowed programmers to use symbolic representations of machine instructions. The real shift came with the advent of high-level 
languages, which abstracted the programming process further from the machine language. The first significant high-level language was FORTRAN, 
developed in the 1950s by John Backus’ team at IBM. This development was closely followed by the creation of the first compiler for FORTRAN, 
which marked a pivotal moment in computing, allowing for more rapid and flexible program development. Throughout the 1960s and 1970s, the evolution 
of compilers was characterized by improvements in optimization techniques and error detection mechanisms, which greatly enhanced programming 
efficiency and machine performance. Languages such as COBOL and LISP were developed with their compilers, expanding the usability of computers 
in business and research.

As computing power increased and the needs of software grew more complex, the functionality of compilers expanded. Modern compilers 
are now capable of performing complex optimizations on the code to improve execution speed and reduce resource consumption. They also 
play a critical role in the development environment, offering developers immediate feedback on errors and warnings.

In summary, compilers are indispensable to the development of software. They translate high-level language into machine code, 
enhance it for performance and ensure it is error-free. From their origins in the earliest days of programming to their current 
complex forms, compilers have grown to be indispensable tools in the arsenal of modern computer science. As technology evolves, 
the role of compilers continues to adapt, ensuring they remain at the heart of software development processes.
</p>

## <div align = "center"> Operations of the Compiler [Jackson] </div>
<p>

<!--- Insert Your part here -->
</p>

## <div align = "center"> 3 Phases of Compilers [Jackson] </div>
<p>
<!--- Insert Your part here -->
</p>

## <div align = "center"> Types of Compilers[Tamara] </div>
<p>
    
</p>

### <div align = "center"> Single Pass Compilers </div>
<p>
    When observing the different types of compilers, one of the more "simple" design choices for a compiler 
would be the Single Pass Compiler. A <b> Single Pass Compiler </b> is a compiler that processes the source
code of a program from start to finish in one pass. Meaning unlike our other compiler types that scan and read the 
source code in multiple phases. Single pass compilers read and translate the source as the programming is running. 

Despite having a faster run time and better resource management, Single Pass Compilers are very limited in terms of creating complex optimizations 
for the code it reads. Which can be a challenge to implement for complex languages because of its inability to revisit and reread the code. Which puts the compiler
at a major disadvantage comparative to Two Pass and Multi Pass compilers. However, while the Single Pass compiler may not be able to handle complex languages. What the Single Pass compilers do have an advantage in
is better resource management and speed than both Two Pass and Multi Pass compilers. Which makes the Single Pass compiler a better candidate for embedded systems, bootloaders, and scripting languages such as JavaScript. 
</p>

 ![SinglePass_Compiler.png](Images%2FSinglePass_Compiler.png)

### <div align = "center"> Two Pass Compilers </div>
<p>
    Another commonly used compiler is a Two-Pass Compiler. <b> Two Pass Compilers </b> are a type of Multi Pass compilers that read the source code
twice before running the program. Meaning unlike the previous Single Pass compiler, Two Pass compilers read through the source code once and then complete another
pass through of the source code. Two Pass Compilers are typically made up with a code scanner called a <b>lexical analyzer</b>. This lexical analyzer scans through a high level program and converts the scan
into a mix of identifying tokens. Once the lexical analyzer is complete the tokens are then sent to the second pass which is called a <b> syntax analyzer</b>. This syntax analyzer will take the tokens from the lexical analyzer
and parses the tokens. The syntax analyzer will parse the tokens into a tree and check to see if the program is written correctly. This two pass system can sometimes be referred to as 
Front end and Back end processes. 

Two pass compilers and Multi Pass Compilers are actually very similar in the way the programs functions. The only difference is while Multi Pass compilers can three or more passes throughout its duration. Two Pass compilers only allow
for two passes through its program. Which allows the Two Pass compiler to have a faster runtime than a Multi Pass compiler. This also allows for the Two Pass compiler to have fewer limitations in optimization comparative to a
Single Pass Compiler. However, there are still some limitations that a Two Pass compiler cannot do. For example,  Two Pass compilers cannot handle complex optimizations of code like a Multi-Pass compiler. These compilers also cannot do effective type-checking which is something you can
typically find in Multi Pass compilers. Leaving Two Pass compilers to be best used with concepts like mutual recursion, dead code elimination, and for some programming languages like C++.
</p>

![TwoPassCompiler.png](Images%2FTwoPassCompiler.png)

### <div align = "center"> Multi Pass Compilers </div>
<p>
    The last compiler type that is typically used  for programming languages is called a <b>Multi Pass Compiler</b>. Multi Pass compilers work by having multiple passes through a program before the program executes. Meaning that 
the source code will be read through multiple times before they are executed. Meaning that Multi Pass Compilers will read through the source code multiple times before a programs runs. There are two different methods that a 
Multi Pass compiler can implement to parse through their programs called <b> Multiple Stages </b> and <b> </b>

Multi Pass compilers work similarly to Two-Pass compilers as they both contain a lexical analyzer and a syntax analyzer. Considering that Two Pass compilers are a type of Multi Pass compilers.

</p>

![MultiPass_Complier.png](Images%2FMultiPass_Complier.png)

## <div align = "center">The Difference between a Complied and Interrupted Language [Ken]
<p>
    Programming languages are typically divided into two categories: compiled and interpreted. This classification hinges on how the languages convert code into machine code, the form executable by a computer's hardware. Compiled languages, such as C and C++, necessitate the use of a compiler to translate the entire program into machine code prior to execution. In contrast, interpreted languages, like Python and JavaScript, are executed progressively by an interpreter, which reads and executes the code line by line.

Compiled languages are well-suited for applications where performance and speed are paramount. For instance, system software, game development, and applications that require intensive numerical computations typically employ compiled languages. The chief advantage of these languages is their fast execution speed; since the code is pre-compiled into machine code, it can be executed directly and quickly. However, disadvantages include less flexibility for error correction during runtime and a longer initial development time due to the compilation process.

Interpreted languages, on the other hand, are preferred for projects where quick development and portability outweigh execution speed. These languages are commonly used for web development, scripting, and automation tasks. The benefits of interpreted languages include easier debugging and testing, as errors can be rectified immediately without recompilation. Additionally, these languages tend to be more user-friendly and flexible. The primary drawback, however, is slower performance compared to compiled languages, due to runtime interpretation which can delay execution.

Practically speaking, the decision between using a compiled or interpreted language often depends on the specific needs of the project. Compiled languages offer efficiency and are ideal for performance-sensitive applications with stable requirements, while interpreted languages provide greater flexibility and quicker development times for projects where these aspects are prioritized.

While compiled languages deliver superior performance and efficiency, they lack the debugging ease and flexibility that interpreted languages afford. Conversely, while interpreted languages support rapid development and are user-friendly, they experience slower execution times. Understanding these trade-offs is essential for developers when choosing the language that best suits the needs of their specific project.


## <div align = "center" > Sources </div>

## <div align = "center"> Phases and Operations of a Compiler </div>



