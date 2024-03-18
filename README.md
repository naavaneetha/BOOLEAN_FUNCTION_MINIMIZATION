# BOOLEAN_FUNCTION_MINIMIZATION

# AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

# Equipment Required:

Hardware – PCs, Cyclone II , USB flasher

# Software – Quartus prime

# Theory
Boolean function minimization is a fundamental concept in digital logic design aimed at reducing the complexity of logical expressions while maintaining their functionality. Here are a few theoretical perspectives on Boolean function minimization:

# Karnaugh Maps (K-Maps): #
Karnaugh Maps provide a graphical method for minimizing Boolean functions. They visually represent all possible combinations of input variables and their corresponding output values. By identifying adjacent groupings of 1s (or 0s) in the map, you can derive simplified expressions. This method is particularly useful for functions with a small number of variables, as it can become impractical for larger functions.

# Quine-McCluskey Algorithm: #
The Quine-McCluskey algorithm is a systematic approach to minimizing Boolean functions. It involves systematically combining minterms (or maxterms) to identify prime implicants, which are the smallest possible groupings that cover all essential terms. These prime implicants are then used to derive the minimized expression. While more computationally intensive compared to K-Maps, the Quine-McCluskey algorithm is efficient for functions with a larger number of variables.

# Implicant-Based Minimization: #
Boolean function minimization can also be approached by identifying essential prime implicants and eliminating redundant terms. Essential prime implicants are those that cover output states not covered by any other implicant. Redundant terms, on the other hand, can be eliminated if they are subsumed by other terms or combinations of terms. This approach is often used in combination with K-Maps or the Quine-McCluskey algorithm.
# Algebraic Manipulation: #
Boolean functions can also be minimized using algebraic manipulation techniques. These techniques involve applying Boolean algebra laws such as absorption, distribution, and complementation to simplify expressions. While algebraic manipulation can be intuitive for some functions, it may not always result in the most optimized expressions, especially for functions with many variables.

# Heuristic Methods: #
In addition to the systematic approaches mentioned above, heuristic methods can also be employed for Boolean function minimization. These methods often involve iterative algorithms that attempt to optimize expressions based on predefined criteria such as minimizing the number of terms or reducing the number of literals. Genetic algorithms, simulated annealing, and tabu search are examples of heuristic methods used in Boolean function minimization.

Overall, Boolean function minimization is a multifaceted topic with various methods and techniques available, each with its advantages and limitations. The choice of method depends on factors such as the complexity of the function, the number of variables involved, and the desired optimization criteria.


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


# Program:
```
module exmp2(E ,F, A, B, C, D);
output E, F;
input A, B, C ,D;
assign E = A || (B && C) || ((!B) && D);
assign F = ((!B) && C) || (B && (!C) && (!D));
endmodule
```



# Developed by:Rohith T
# RegisterNumber:212223040173


# RTL realization
![image](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/159523335/d3cbb589-b9bb-49bb-ab6b-0f14459e136b)


# Truth Table:
![image](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/159523335/7689b39f-c661-44f1-be97-9c52a148d800)
![image](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/159523335/17aff900-39b8-451b-91d5-d3f9f21ca7d7)

# Timing:
![image](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/159523335/eabfb499-bb63-4516-a0dc-c1c637ee1b1e)


# Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

