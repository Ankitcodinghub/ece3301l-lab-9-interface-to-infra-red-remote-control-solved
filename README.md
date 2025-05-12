# ece3301l-lab-9-interface-to-infra-red-remote-control-solved
**TO GET THIS SOLUTION VISIT:** [ECE3301L LAB 9-Interface to Infra Red Remote Control Solved](https://www.ankitcodinghub.com/product/ece3301l-lab-9-interface-to-infra-red-remote-control-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91494&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;ECE3301L LAB 9-Interface to Infra Red Remote Control Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
LAB 9: Interface to Infra Red Remote Control

The purpose of this lab is to introduce the student to the technique to interface to an Infra Red Remote Control.

Lab:

Below is a basic stream of pulse when a key on a remote control is pressed:

</div>
</div>
<div class="layoutArea">
<div class="column">
This is based on the NEC protocol transmission. Here are the basic steps on that protocol:

<ul>
<li>A leading burst of pulses that lasts up 9 msec.</li>
<li>A space period that lasts 4.5 msec.</li>
<li>An 8-bit address field for the receiving device</li>
<li>An 8-bit address inverse of the address</li>
<li>An 8-bit command field</li>
<li>An 8-bit inverse of the command fieldA total of 32 bits should be received after the ‘Space 4.5 msec’ field has been detected. To differentiate for each bit between the logic ‘0’ or the logic ‘1’, the following detection should be applied:
<ul>
<li>A logic ‘0’ should be detected when a 562-usec pulse burst is followed by a space period of 562 usec.</li>
<li>A logic ‘1’ should be detected when a 562-usec pulse burst is followed by a space of 1.675 msec</li>
</ul>
</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
When the Infrared signal is received by an IR receiver, the output of that receiver should provide:

<ul>
<li>The output stays at logic ‘1’ when no pulse is received</li>
<li>The output goes to ‘0’ when the leading pulse is detected. The output should stay at logic‘0’ for 9 msec.</li>
<li>When the ‘Space’ is asserted, the output changes to logic ‘1’ for the period of 4.5 msec.</li>
<li>Next a sequence of 32 bits should be transmitted. When the output changes from ‘1’ to‘0’ and then back to ‘1’ with the same width of 562 usec, then a data logic ‘0’ is asserted. Otherwise, if the output goes from ‘1’ to ‘0’ for a period of 562 usec and then switches from ‘0’ to ‘1’ for a period of 1.675 msec, then a data logic ‘1’ is asserted.</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
PART 1)

To implement this protocol, we will need to use the Timer for the purpose to measure the elapsed time between two events and the input pin that has the edge-triggered interrupt feature (the INTx pins). Let us assume that we are going to use the INT0 pin to connect to the output of the IR receiver. That output is normally sitting on the logic ‘1’ when no key is pressed on the remote control. A variable ‘Nec_state’ should be used and its initial value should be set to ‘0’. That is the first state of the IR decoding sequence. The program should use the pin INT0 to detect the different transitions of the IR signals and update the value of ‘Nec_state’ to keep track of the progress of the sequence. At the initial point, INT0 should be programmed to interrupt when the IR output transitions from high to low.

When an INT0 interrupt occurs, the first task is to read the content of the timer and save into a variable. The next step is to determine to update the state of ‘Nec_state’

INT0_ISR:

<ul>
<li>If Nec_State not in state 0 then read the 16-bit from TMR1H and TMR1L to store into variable Time_Elapsed. Clear both TMR1H and TMR1L</li>
<li>Else, switch on Nec_State: Case 0:
<ul>
<li>Clear TMR1H and TMR1L</li>
<li>Program Timer 1 mode with count = 1usec using System clock running at 8Mhz</li>
<li>Enable Timer 1</li>
<li>Force bit count (bit_count) to 0</li>
<li>Set Nec_code = 0</li>
<li>Set Nec_State to state 1</li>
<li>Change Edge interrupt of INT0 to Low to High</li>
<li>returnCase 1:</li>
<li>Check if Time_Elapsed value read is between 8500 usec and 9500 usec</li>
<li>If yes, force Nec_state to state 2 else do force_nec_state0()</li>
<li>Change Edge interrupt of INT0 to High to Low</li>
<li>returnCase 2:</li>
<li>Check if Time_Elapsed value read is between 4000 usec and 5000 usec</li>
<li>If yes, force Nec_state to state 3 else do force_nec_state0()</li>
</ul>
</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
<ul>
<li>Change Edge interrupt of INT0 to Low to High</li>
<li>returnCase 3:</li>
<li>Check if Time_Elapsed value read is between 400 usec and 700 usec</li>
<li>If yes, force Nec_state to state 4 else do force_nec_state0()</li>
<li>Change Edge interrupt of INT0 to High to Low</li>
<li>returnCase 4:</li>
<li>Check if Time_Elapsed value read is between 400 usec and 1800 usec</li>
<li>If yes,
<ul>
<li>shift left nec_code by 1 bit</li>
<li>Check if Time_Elapsed is greater than 1000 usec</li>
<li>If yes, add 1 to Nec_code else do nothing</li>
<li>Increment variable bit_count by 1</li>
<li>Check if bit_count &gt; 31</li>
<li>If yes:
<ul>
<li>set nec_ok flag to 1</li>
<li>set INT0IE = 0</li>
<li>set Nec_State to 0</li>
</ul>
</li>
<li>If not, do nothing</li>
<li>Set Nec_State to state 3</li>
</ul>
</li>
<li>If not, do force_nec_state0()</li>
<li>Change Edge interrupt of INT0 to Low to High</li>
<li>returnSee the attached sample ‘.c’ file to get started.
In the main routine, the variable ‘nec_ok’ will constantly checked. When it is set to 1, then a button on the remote has been detected. The TeraTerm console should show on the screen the long value of the Nec code (0x00FFccdd) where cc is the actual code and dd is the 1’s complement of that code. The variable Nec_code1 stores that cc code.

PART 2)

Next, press all the buttons and collect all the codes and then place them consecutively into an array from the order of the buttons on the remote control. See example of array1 in the sample code.

The next step is to create another array called ‘txt1’ with the text values of each button. The text should be 3 characters long terminated with a ‘\0’ to end the string. See the sample code.
</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
A third array called ‘color’ should reflect the color of each button.

In the main code, after each button is pressed, use a for loop to look up for the corresponding definition of that button to determine the order of that button on the array in order to display that button on the LCD screen.

The last task is to output the color of the button onto one of the three RGB LEDs D1, D2, and D3 based on the column that button is located on the remote control. The first 7 buttons are assigned to D1, the buttons from ‘+‘ to ‘2’ are associated to D2 and the last bottom seven bottom buttons are assigned to D3. Don’t use if or case statement to select the color for the output. In addition, since the color black cannot be displayed, replaced it by the color WHITE.

</div>
</div>
</div>
