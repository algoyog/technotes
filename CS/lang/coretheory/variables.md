- **Variable**
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
