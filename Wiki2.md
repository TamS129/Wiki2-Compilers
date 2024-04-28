<!--- I added some html to our doc to allow for more freedom for text, images, etc. -->
<!--- To separate your paragraphs use the <p> brackets.Ex:
<p> insert your paragraph text here </p> -->

<!--- This method below is to indent our paragraphs to make it look neater. 
If you erase this our paragraph indents go away. - Tamara -->

<style>
    p{
        text-indent: 30pt
    }
   
</style>

<!--- End of Paragraph Indent -->

# <div align ="center"> Wiki 2: Compilers</br> <span style="font-size:0.5em;"> Written By: Jackson Kettel, Ken Cage, Kelvin Rajbhandari, Tamara Slone </span> </div>

## <div align = "center">Introduction </div>
<p>



</p>

## <div align = "center">Compilers and their purpose [Kelvin]</div>
<p>
<!--- Insert Your part here between the p brackets -->
</p>

## <div align = "center">The History of Compilers [Kelvin] </div>
<p>

<!--- Insert Your part here between the p brackets-->

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
<!--- Insert Your part here -->
### <div align = "center"> Use Cases </div>
<!--- Insert Your part here -->
### <div align = "center"> Advantages </div>
<!--- Insert Your part here -->
### <div align = "center"> Disadvantages </div>
<!--- Insert Your part here -->

## <div align = "center" > Sources </div>

## <div align = "center"> Phases and Operations of a Compiler </div>



