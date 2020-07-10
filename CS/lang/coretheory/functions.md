
- **Functions**
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