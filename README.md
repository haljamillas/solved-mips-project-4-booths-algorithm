Download Link: https://assignmentchef.com/product/solved-mips-project-4-booths-algorithm
<br>
In this project, you are required to perform a complete run of Booth’s algorithm on two

16-bit signed numbers. The generation steps for the two numbers are described as follows.

<ul>

 <li>Assume that the numerical part of your student ID is <strong><em>A</em></strong>.</li>

 <li>The square of <strong><em>A</em></strong> is <strong><em>B</em></strong> (<strong><em>B = A<sup>2</sup></em></strong>). Use binary representation to represent <strong><em>B</em></strong>.</li>

 <li>Right shift <strong><em>B</em></strong> for 16 bits, take the lower 15 bits, and append an extra bit ‘0’ to the most significant bit (MSB) to form a new 16-bit number <strong><em>C</em></strong>. (i.e., <strong><em>C</em></strong> is a positive number.)</li>

 <li>Right shift B for 16 bits, take the lower 15 bits, and append an extra bit ‘1’ to the most significant bit (MSB) to form a new 16-bit number <strong><em>D</em></strong>. (i.e., <strong><em>D</em></strong> is a negative number.)</li>

 <li><u>Perform <strong><em>C×D</em></strong> by using the Booth’s algorithm</u>.</li>

</ul>




Please submit your Booth’s multiplication result according to the following rules:

<ul>

 <li>You are required to write every detailed step according to our lecture notes.</li>

 <li>Upload your homework in TEXT format.</li>

 <li>The filename is your student ID (e.g., B12345678.txt).</li>

</ul>




Example:




<ul>

 <li>= 12345678</li>

 <li>= 100010101001111100001111100011000011001111000100</li>

 <li>= 0000111110001100</li>

 <li>= 1000111110001100</li>

</ul>

CD




Step               Product                  Next

<ul>

 <li>0000000000000000 1000111110001100 0 00 -&gt; shift</li>

 <li>0000000000000000 0100011111000110 0 00 -&gt; shift</li>

 <li>0000000000000000 0010001111100011 0 10 -&gt; sub</li>

 <li>+1111000001110100</li>

</ul>

1111000001110100 0010001111100011 0

1111100000111010 0001000111110001 1   11 -&gt; shift

…

<ul>

 <li>0000001111000110 1101001001000010 0 00 -&gt; shift</li>

 <li>0000000111100011 0110100100100001 0 10 -&gt; sub</li>

 <li>+1111000001110100</li>

</ul>

1111001001010111 0110100100100001 0

1111100100101011 1011010010010000 1   done

CD = 1111100100101011 1011010010010000


