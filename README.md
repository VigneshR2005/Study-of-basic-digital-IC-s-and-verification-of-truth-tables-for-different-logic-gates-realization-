### Study-of-basic-digital-IC-s-and-verification-of-truth-tables-for-different-logic-gates-realization-
AIM: To study about the different digital IC’s and to verify the truth table in Quartus for the basic logic gates using Verilog programming.

Equipments Required: Hardware – PCs, Cyclone II , USB flasher Software – Quartus prime Theory Introduction Logic gates are the basic building blocks of any digital system. Logic gates are electronic circuits having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. Based on this, logic gates are named as

AND gate OR gate NOT gate NAND gate NOR gate Ex-OR gate Ex-NOR gate

AND gate The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB
Y= A.B

OR gate The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation.
Y= A+B

NOT gate The NOT gate is an electronic circuit that produces an inverted version of the input at its output. It is also known as an inverter. If the input variable is A, the inverted output is known as NOT A. This is also shown as A' or A with a bar over the top, as shown at the outputs.
Y= A'

NAND gate This is a NOT-AND gate which is equal to an AND gate followed by a NOT gate. The outputs of all NAND gates are high if any of the inputs are low. The symbol is an AND gate with a small circle on the output. The small circle represents inversion.
Y= (AB)’

NOR gate This is a NOT-OR gate which is equal to an OR gate followed by a NOT gate. The outputs of all NOR gates are low if any of the inputs are high. The symbol is an OR gate with a small circle on the output. The small circle represents inversion.
Y= (A+B)’

Ex-OR gate The 'Exclusive-OR' gate is a circuit which will give a high output if either, but not both of its two inputs are high. An encircled plus sign (⊕) is used to show the Ex-OR operation.
Y= A⊕B

Ex-NOR gate The 'Exclusive-NOR' gate circuit does the opposite to the EX-OR gate. It will give a low output if either, but not both of its two inputs are high. The symbol is an EX-OR gate with a small circle on the output. The small circle represents inversion.
Y= A⊕B

Procedure Connect the supply (+5V) to the circuit Switch ON the main switch Press the switches for inputs “A” and “B”. The switch is ON state when 1 is pressed. The switch is OFF state when 0 is pressed. If the output is 1, then the bulb glows. Check all the gates following the same procedure.

Program:
```
module DE_EX_01(a,b,yand,yor,ynor,ynot,yxor,ynand,yxnor);
input a,b;
output yand,yor,ynor,ynot,yxor,ynand,yxnor;
and(yand,a,b);
or(yor,a,b);
not(ynot,a);
xor(yxor,a,b);
xnor(yxnor,a,b);
nand(ynand,a,b);
nor(ynor,a,b);
endmodule
# Developed by:R.Vignesh
# RegisterNumber:212222230172
```
*/

Logic symbol & Truthtable
![263432868-d9a41073-1f62-49a4-9486-1f862d62302a](https://github.com/VigneshR2005/Study-of-basic-digital-IC-s-and-verification-of-truth-tables-for-different-logic-gates-realization-/assets/119401246/3f8270c1-d519-450c-8557-a89b9ee1368d)

Output: RTL
![263434376-23f240ca-340c-45c3-87b6-35460c5f3b2c](https://github.com/VigneshR2005/Study-of-basic-digital-IC-s-and-verification-of-truth-tables-for-different-logic-gates-realization-/assets/119401246/dcb43712-eb05-4581-a13e-be1d6c549885)

WAVEFORM
![263431936-08ab8a35-0b95-40bb-b860-49627ab6da3e](https://github.com/VigneshR2005/Study-of-basic-digital-IC-s-and-verification-of-truth-tables-for-different-logic-gates-realization-/assets/119401246/4b2b5d29-c9be-4217-89e7-7287358f320b)

Result: Thus the different digital IC’s are studied and the truth table for different logic gates are verified.


