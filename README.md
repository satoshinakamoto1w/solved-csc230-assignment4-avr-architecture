Download Link: https://assignmentchef.com/product/solved-csc230-assignment4-avr-architecture
<br>
This assignment covers low level C programming on the AVR architecture, and is the last piece of the applied programming component of the course. You are already familiar with the task: Implement an accurate stopwatch. In fact, the overall specification of the program is identical to assignment 3; the only difference is that your implementation must be written in C instead of assembly.

Consult the assignment 3 specification for details on the expected functionality of the program. Section 2 below describes the evaluation process for this assignment.

<h1>1              Evaluation</h1>

Submit all .c and .h files needed to assemble your assignment electronically via conneX (including all of the necessary LCD library files, even if you did not modify them). Your code must compile, upload and run correctly on the ATmega2560 boards in ECS 249 using the toolchain and methodology described in Lab 7. If your code does not compile as submitted, you will receive a mark of at most 2.

If your implementation is not written in C, or does not use the C programming environment covered in Lab 7, you will receive a mark of zero.

This assignment is worth 6% of your final grade and will be marked out of 12. The evaluation will not be demo-based.

The marks are distributed among the aspects of the assignment as follows. The distribution of marks between components is given in the table below. Note that most of the entries refer to sections of the assignment 3 specification.

1

<table width="561">

 <tbody>

  <tr>

   <td width="59"><strong>Marks</strong></td>

   <td width="502"><strong>Aspect</strong></td>

  </tr>

  <tr>

   <td width="59">6</td>

   <td width="502">The basic, non-interactive timer described in Section 2 of the A3 specification functions correctly with reasonably accurate timing (such that a human observer cannot notice any discrepancy). Timing functionality must be implemented using one of the hardware timers, not software delay loops (including the _delay_ms function).</td>

  </tr>

  <tr>

   <td width="59">1</td>

   <td width="502">The timing is theoretically accurate to within 1 second out of 10 minutes when the 16Mhz system clock is assumed to be exact.</td>

  </tr>

  <tr>

   <td width="59">1</td>

   <td width="502">Global variables are used <strong>only </strong>for global, persistant data (such as the active timer state). Local variables are used for all other data and temporary storage.</td>

  </tr>

  <tr>

   <td width="59">1</td>

   <td width="502">The SELECT button correctly implements the start/stop feature described in Section 3 of the A3 specification. The code must ensure that a single press of the button be read only once (regardless of how long the button is held down).</td>

  </tr>

  <tr>

   <td width="59">1</td>

   <td width="502">The LEFT button correctly implements the clear feature described in Section 3 of the A3 specification.</td>

  </tr>

  <tr>

   <td width="59">1</td>

   <td width="502">The UP button correctly implements the ‘set lap’ feature described in Section 4 of the A3 specification. Note that unless the display of lap times is correct, it is impossible to evaluate this component (and the component below).</td>

  </tr>

  <tr>

   <td width="59">1</td>

   <td width="502">The DOWN button correctly implements the ‘clear lap’ feature described in Section 4 of the A3 specification.</td>

  </tr>

 </tbody>

</table>