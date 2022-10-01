<a href="/Arrays/Main.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Arrays/Omit-Size.md">Next &gt;</a>
<hr>
You don't have to specify the size of the array. But if you don't, it will only be as big as the elements that are inserted into it:
<pre>string cars[] = {"Volvo", "BMW", "Ford"}; // size of array is always 3</pre>
This is completely fine. However, the problem arise if you want extra space for future elements. Then you have to overwrite the existing values:
<pre>
<s>string cars[] = {"Volvo", "BMW", "Ford"};</s>
string cars[] = {"Volvo", "BMW", "Ford", "Mazda", "Tesla"};
</pre>
If you specify the size however, the array will reserve the extra space:
<pre>string cars[5] = {"Volvo", "BMW", "Ford"}; // size of array is 5, even though it's only three elements inside it</pre>
Now you can add a fourth and fifth element without overwriting the others:
<pre>
cars[3] = "Mazda";
cars[4] = "Tesla";
</pre>
<h1>Omit Elements on Declaration</h1>
It is also possible to declare an array without specifying the elements on declaration, and add them later:
<pre>
string cars[5];
cars[0] = "Volvo";
cars[1] = "BMW";
...
</pre>
