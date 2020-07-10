# Language Features
```
(*Using SML*)
```
- Syntax: how something is written
- Semantics: What it means
    - Type checking: before prog runs
    - Evaluation: after prog runs

- *Variable*
    - Formal Definition
        - type
            - Either defined statically or dynamically.
        - value binding
            - Either by reference or by value (see shadowing for more understanding.)
    - **Static Environment**
        - All the features of a language during coding or compile time
        ```
            (*Using SML*)
            val a = 5 // The variable a is statically a integer
        ```
        - eg, the core variables data type 
    - **Dynamic environment**
        - Features during runtime of the code
        ```
            (*Using SML*)
            val a = 5 // The variable a is dynamically assigned a value 5
        ```
    - **Shadowing** - same as ref by value. In the below code the change to a does not impact b's value.
        ```
            a = 5
            b = a+5 //b=10
            a = a+1
            c = a   //b=10, c=6             
        ```
- *Functions*
    - Formal Definition
        - Function Definition
            - Syntax
                ```
                    def: fun x0(x1:t1....xn:tn)
                ```
            - Evaluation
                - A function is a value with default value of return datatype
                - The evaluation will be done during the function call rather than during definition.
            - Type checking
                - Input list be statically defined or variable.
                - type check for input and return bindings. This is done statically or dynamically based on the programming language. 
                    - This happens during function def
                    - Also during the function call.
        - Function call
            - Syntax
            ```
                call: e0(e1...en)
            ```
            - Evaluation
                - Step 1: Evaluate e0 to x0 in the dynamic environment
                - Step 2: evaluate input params (e1..en) to (x1..xn) including type checking
                - Step 3: evaluate the return value based on the body of the code to the function def. This is done in function def env (static env) or both based on the language capability.
    - Ex.
        ```
        fun add (x:int, y:int) = 
             x + y
        val ret = add (1,2)
        SML Interpretation
            val add = fn : int * int -> int
        ```
    - binding are earlier available values and future bindings are not possible.