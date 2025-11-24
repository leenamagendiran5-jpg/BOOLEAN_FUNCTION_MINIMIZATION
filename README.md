# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory:**

Boolean function minimization is the process of simplifying Boolean algebraic
expressions to reduce the number of logic gates and complexity in a digital circuit,
leading to more efficient, faster, and less costly hardware

For minimizing Boolean expressions,we can use a set of rules and laws (like distributive,
associative, and complement laws) to simplify Boolean expressions. This method
focuses on applying algebraic manipulations to reduce the complexity of the expression
by eliminating redundant terms.

Identity Law A ⋅ 1 = A, A + 0 = A
Null Law A ⋅ 0 = 0, A + 1 = 1                                                                                                                                                                                        Idempotent Law A ⋅ A = A, A + A = A
Complement Law A ⋅ A′ = 0, A + A' = 1
Distributive Law A ⋅ (B + C) = A ⋅ B + A ⋅ C
De Morgan’s Law (A ⋅ B)′ = A′ + B', (A + B)′ = A′ ⋅ B′
Absorption Law A ⋅ (A + B) = A, A + (A ⋅ B) = A
Associative Law A + (B + C) = (A + B) + C, A.(B.C) = (A.B).C
Commutative law A B = B A,A + B = B + A

**Logic Diagram:**

Identity Law

![identity law](https://github.com/user-attachments/assets/f5347042-8ab4-48f6-b0c9-0a829148e4bc)

Null Law

![null law](https://github.com/user-attachments/assets/72143389-1df5-4175-b865-df05720b6065)


Idempotent Law

![idempotent law](https://github.com/user-attachments/assets/54be5821-684b-47a9-9117-570aef8bca27)

Complement Law 

![complement law](https://github.com/user-attachments/assets/e5504236-87e4-4166-b918-4fba706c5533)

Distributive Law

![distributive law](https://github.com/user-attachments/assets/6054cf5e-c1d6-4756-b783-86b1a02bf5e0)

De Morgan’s Law

![De morgan&#39;s law](https://github.com/user-attachments/assets/a9d9ce08-83a3-44e3-b6bb-ccf6e25c2186)

Absorption Law

![absorption law ](https://github.com/user-attachments/assets/fe920895-4048-4c10-b620-1f37ee1bdd5c)

Associative Law 

![associative law](https://github.com/user-attachments/assets/10b9c9be-d39a-4c51-90ba-7f3811dae8f6)

Commutative law

![commutative law](https://github.com/user-attachments/assets/3166fc4a-ca33-4ab6-8ea4-488b78205333)


**Procedure:**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Developed by: M.LEENA SHREE RegisterNumber:25018414 
```
i)
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```

```
ii)
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```

**RTL realization**

**Output:**

i)

![RTL realisation](https://github.com/user-attachments/assets/b374968b-fa61-4e37-8f01-e848bd259660)

ii)

![RTL 2](https://github.com/user-attachments/assets/487fd76a-9d2a-4619-a2de-9850ece51b34)



**RTL**

**Timing Diagram**

i)

![timing diagram 1](https://github.com/user-attachments/assets/ef3c4842-8d7c-4b1e-94e9-d4c83ce406d3)

ii)

![timing diagram 2](https://github.com/user-attachments/assets/a202e323-a69e-4316-aeac-1bfaced49ef3)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

