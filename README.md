### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

/* write all the steps invloved */

**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming. 

Developed by: B ARPUTHA RegisterNumber:25012532
*/

**RTL LOGIC UP COUNTER**
<img width="1011" height="534" alt="image" src="https://github.com/user-attachments/assets/78f46374-40ae-4820-9c31-d2823cfc0ab2" />

**TIMING DIAGRAM FOR IP COUNTER**
<img width="1007" height="535" alt="image" src="https://github.com/user-attachments/assets/3bbae1f3-658b-460b-818f-81ca7bd9555f" />

**TRUTH TABLE**

**RESULTS**<img width="1920" height="1080" alt="ex6(1)" src="https://github.com/user-attachments/assets/f9957e13-1541-4932-9e04-f2ad3b3ad45a" />
<img width="1920" height="1080" alt="ex6(2)" src="https://github.com/user-attachments/assets/48d0ae89-94b6-4606-82ba-f61a7b74414e" />

<img width="1920" height="1080" alt="ex6(3)" src="https://github.com/user-attachments/assets/337a8e7c-d73a-479c-992a-9bd9aec4c57b" />
