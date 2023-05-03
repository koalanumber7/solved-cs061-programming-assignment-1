Download Link: https://assignmentchef.com/product/solved-cs061-programming-assignment-1
<br>
<strong>Objective</strong>

<strong>The purpose of this assignment is to familiarize you with the basics of LC-3 assembly language </strong><strong>programming, the SIMPL emulator, and rudimentary debugging.</strong>

<strong>Your Tasks</strong>

<strong>Implement the LC-3 program from the image below.</strong>

<strong>Note: </strong><strong>This is <em>almost, </em>but not <em>quite, </em>the same program you worked on in Lab 1: it uses a DO-WHILE </strong><strong>loop to multiply one number by another by repeated adding.</strong>

<strong>First (as with all your labs and assignments) go to the Assignment folder in</strong><strong><u> Piazza,</u></strong><strong> and download </strong><strong>the assignment 1 zip file to your assignments/assnl folder in your cs account, and unzip it in place.</strong>

<strong>Type the code from the image below into your assignmentl.asm file</strong>

<strong><em>Again, the registers are assigned differently from your Lab 1 exercise, so don’t copy that! </em></strong><strong><em>But do use the (AND with 0) technique discussed in the “TIP” paragraph in lab 1.</em></strong>

<strong>geany assignmentl.asm &amp;</strong>

<strong>and then launch &amp; run simpl: </strong><strong>simpl assignmentl.asm &amp;</strong>

<strong><em>Remember: whenever you run simpl, you must </em></strong><strong><em><u>ALWAYS</u></em></strong><strong><em> keep the Text Window open so you can see </em></strong><strong><em>warnings &amp; error messages from the emulator!</em></strong>

<strong>Now place a </strong><strong><em><u>breakpoint</u></em></strong><strong> at the </strong><strong><u>beginning</u></strong><strong> of the DO-WHILE loop by right-clicking that line of code and selecting “Mark as Breakpoint”.</strong>

<strong>Now, when you press the “Run” button, simpl will execute each line of code until it reaches the </strong><strong>breakpoint, where it will pause and wait for you to press Run again; it will continue doing this until </strong><strong>it no longer encounters the breakpoint, at which time it will continue executing until the HALT </strong><strong>instruction.</strong>

<strong>Lastly, create a table in your .asm file (see the image below) to record the register contents for <em>each </em></strong><strong>register (RO through R7) as you repeatedly press the Run button and iterate through the loop, as </strong><strong>follows:</strong>

<ul>

 <li><strong>Before entering the loop (i.e. the first time the program halts at the breakpoint)</strong></li>

 <li><strong>After each iteration of the loop (each subsequent breakpoint pause)</strong></li>

 <li><strong>Note that since your breakpoint is at the start of the loop, the register values after the <em>it </em></strong><strong>iteration will just be the values when the program has ended, as suggested by the naming of the </strong><strong>last row in the image below.</strong></li>

</ul>

<strong><em>Before you run the code, try to answer this question:</em></strong>

<strong><em>How many rows do you think you will end up with in your table?</em></strong>

<strong>Format your table like the one in the image below <em>(but obviously reporting the actual values from ALL eight registers, for ALL iterations of the loop!)</em></strong>




<strong>The following program performs the action:</strong>

<strong>R3 &lt;– 12 * 6   </strong><strong>; (i.e. multiply 12 by 6 and write the result into Register 3)</strong>

<strong>using the equivalent of a DO-WHILE loop:</strong>

<table>

 <tbody>

  <tr>

   <td width="463"><strong>_</strong><strong> Name!</strong><strong> tim.y</strong><strong><sub>.</sub></strong><strong>q9</strong><strong> Miyazaki</strong><strong>_</strong><strong> Login:hayam</strong><strong>.-,</strong><strong> Email address:</strong><strong> <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="e0ce888199818da08393">[email protected]</a>_ucredLI </strong><strong>Assignment’</strong><strong> apt,</strong><strong>Lab Section:</strong><strong> &lt;021 or 022&gt;</strong><strong>-_</strong><strong> TN_ Sean Foley</strong><strong>:</strong><strong> I</strong><strong> attest that this code</strong><strong> was</strong><strong> totally given </strong><strong>:to me and that</strong><strong> I</strong><strong> didn’t</strong><strong> come</strong><strong> up with </strong><strong>:any</strong><strong> of it =P</strong><strong>REG VALUES</strong><strong>             </strong><strong>RO</strong><strong> R1</strong><strong> R2 R3</strong><strong> R4</strong><strong> R5 R6 R7</strong><strong>Pre-loop</strong><strong>                          </strong><strong>x      x      x      x      x      x      x      x</strong><strong>tteration</strong><strong> 01                    </strong><strong>x      x      x      x      x      x      x      x</strong><strong>iteration</strong><strong> 02                   </strong><strong>x      x      x      x      x      x      x      x</strong><strong>:</strong><strong> Iteration n                        </strong><strong>x      x</strong><strong>             xxxxx.X</strong><strong>:</strong><strong> End of program           </strong><strong>x      x       x</strong><strong>       x      x      x</strong><strong>      x       x</strong><strong>.OR IG x3000</strong><strong>                                                                                                                                                 </strong><strong>,</strong><strong> Program</strong><strong> begins here</strong><strong>to</strong>LD<strong> RI, DEC_6                            </strong><strong>111</strong><strong> &lt;-6</strong><strong>LD</strong><strong> R2, DEC</strong><strong> t2                             </strong><strong>R2 &lt;-12</strong><strong>LD</strong><strong> R3,</strong><strong> DECO                                      </strong><strong>R3 &lt;-0</strong><strong>DO_WHILE ADD R3. R3, R2</strong><strong> .113 &lt;-113</strong><strong> + R2</strong><strong>ADD</strong><strong> RI.</strong><strong> R</strong><strong>1</strong><strong>,</strong><strong> #-1</strong><strong> :R1 &lt;—</strong><strong> R1 -1</strong><strong>BRp DO_ WHILE</strong><strong>     </strong><strong>:</strong><strong> if</strong><strong> ( LMR</strong><strong> &gt;0)</strong><strong> goto</strong><strong> DO_WHILE</strong><strong>HALT</strong><strong>                                                    </strong><strong>Terminate the</strong><strong> program</strong><strong>:</strong><strong> Data</strong><strong>DEC</strong><strong>        .FILL</strong><strong>               </strong><strong>110</strong><strong>                                                 </strong><strong>;</strong><strong> Put the</strong><strong> value</strong><strong> 0</strong><strong> into</strong><strong> memory</strong><strong> here</strong><strong>DEQ6 .FILL</strong><strong>              #6</strong><strong>             :</strong><strong> Put the</strong><strong> value</strong><strong> 6</strong><strong> into</strong><strong> memory</strong><strong> here</strong><strong>DEC_12</strong><strong> ..FILL</strong><strong><em>            </em></strong><strong><em>ti12</em></strong><strong>         :</strong><strong> Put the value 12 into</strong><strong> memory</strong><strong> here</strong><strong>END</strong></td>

  </tr>

 </tbody>

</table>




<strong>Remember: Replace the instruction that zeros out R3 with the AND technique you learned in lab 1! </strong><strong>Submission Instructions</strong>

<strong>Submit your assignmentl.asm file <em>(and ONLY that file!) </em>to the Programming Assignment 1 folder in </strong><strong>Gradescope.</strong>

<strong>Note that there is no autograding for assnl – you will be notified when it has been graded manually.</strong>

<strong>Rubric</strong>

<ul>

 <li><strong>There is nothing for you to actually get wrong in this assignment (we give you the code!) – so the </strong><strong>only way to mess up and lose points would be to fail to follow instructions.</strong></li>

</ul>

<strong>So get into the habit of reading the instructions fully &amp; carefully &#x1f642;</strong>

<ul>

 <li><strong>This assignment has to be graded manually (i.e. we have to look at your code formatting and </strong><strong>your register table); we will try to grade submissions at least once or twice a day. </strong><strong>So don’t leave it to the last day – you may need a second chance!! See the point above!</strong></li>

 <li><strong>For this and all assignments, use of the template given to you is required.</strong></li>

</ul>

<strong>Comics??1Sweethl</strong>