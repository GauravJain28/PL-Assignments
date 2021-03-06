# COL226: Assignment 3

## About:
The folder contains ```bool.lex```, ```bool.yacc```, ```load-bool.sml```, ```ast.sml```, ```evaluator.sml``` and ```loader.sml```. 


## How to Run the Code:
1. Put all the code files in the same folder.
2. Run 
    ```
    make all
    ```
    To generate the ```bool.lex.sml```,  ```bool.yacc.sml```,  ```bool.yacc.sig``` and ```bool.yacc.desc``` files.
    All functions and structures are loaded. SML/NJ interactive shell is opened.
3. Run

    ```
    parseFile "input_file"
    ```
    ```input_file``` should be present in the same folder. 
    
    This will generate the AST Tree of the input file.

4. Run

    ```
    checkFile "input_file"
    ```
    ```input_file``` should be present in the same folder. 
    
    This will generate the AST Tree of the input file and type check it and raise appropiate typing errors wherever required. A list of types is also returned.

5. Run

    ```
    evaluateFile "input_file"
    ```
    ```input_file``` should be present in the same folder. 
    
    This will generate the AST of the input file and directly evalaute the generated AST without type checking it and return a list of values.

6. Run

    ```
    checkEvalFile "input_file"
    ```
    ```input_file``` should be present in the same folder. 
    
    This will generate the AST of the input file and first type-check the AST. Then it will evalaute the generated AST and return a list of values.

7. Run 
    ```
    make clean
    ```
    To clean the generated files ( ```bool.lex.sml```,  ```bool.yacc.sml```,  ```bool.yacc.sig``` and ```bool.yacc.desc``` ).


## Note:
1. The implemented toy language with named and nameless functions support recursion only for named functions similar to SML/NJ97.(There is no support for ```rec``` keyword)
2. The parse error message is generated by using the ML-Yacc system for error handling.
3. Appropiate typing error is generated for the sub-expression in which the typing error is present.
## Author:
* [Gaurav Jain](https://github.com/GAURAV-28)   -   2019CS10349

