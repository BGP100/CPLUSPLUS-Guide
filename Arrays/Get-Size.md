<a href="/Arrays/Omit-Size.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Arrays/Multidimensional.md">Next &gt;</a>
<hr>
To get the size of an array, you can use the sizeof() operator:
<pre>
int myNumbers[5] = {10, 20, 30, 40, 50};
cout &lt;&lt; sizeof(myNumbers);
</pre>
Result: <code>20</code>
<br>
Why did the result show 20 instead of 5, when the array contains 5 elements?
<br>
It is because the sizeof() operator returns the size of a type in bytes.
<br>
You learned from the Data Types chapter that an int type is usually 4 bytes, so from the example above, 4 x 5 (4 bytes x 5 elements) = 20 bytes.
<br>
To find out how many elements an array has, you have to divide the size of the array by the size of the data type it contains:
<pre>
int myNumbers[5] = {10, 20, 30, 40, 50};
int getArrayLength = sizeof(myNumbers) / sizeof(int);
cout &lt;&lt; getArrayLength;
</pre>
Result: <code>5</code>
