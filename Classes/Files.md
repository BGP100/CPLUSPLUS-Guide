<a href="/Classes/Polymorphism.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Classes/Files.md">Next &gt;</a>
<hr>
The fstream library allows us to work with files.
<br>
To use the fstream library, include both the standard iostream AND the fstream header file:
<pre>
#include &lt;iostream&gt;
#include &lt;fstream&gt;
</pre>
There are three classes included in the fstream library, which are used to create, write or read files:
<table>
  <tr>
    <th>Class</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>ofstream</td>
    <td>Creates and writes to files</td>
  </tr>
  <tr>
    <td>ifstream</td>
    <td>Reads from files</td>
  </tr>
  <tr>
    <td>fstream</td>
    <td>A combination of ofstream and ifstream: creates, reads, and writes to files</td>
  </tr>
</table>
To write to the file, use the insertion operator (<code>&lt;&lt;</code>).
<pre>
#include &lt;iostream&gt;
#include &lt;fstream&gt;
using namespace std;<br>
int main() {
  // Create and open a text file
  ofstream MyFile("filename.txt");<br>
  // Write to the file
  MyFile &lt;&lt; "Files can be tricky, but it is fun enough!";<br>
  // Close the file
  MyFile.close();
}
</pre>
<h1>Why do we close the file?</h1>
It is considered good practice, and it can clean up unnecessary memory space.
<h1>Read a File</h1>
To read from a file, use either the ifstream or fstream class, and the name of the file.
<br>
Note that we also use a while loop together with the getline() function (which belongs to the ifstream class) to read the file line by line, and to print the content of the file:
<pre>
// Create a text string, which is used to output the text file
string myText;<br>
// Read from the text file
ifstream MyReadFile("filename.txt");<br>
// Use a while loop together with the getline() function to read the file line by line
while (getline (MyReadFile, myText)) {
  // Output the text from the file
  cout &lt;&lt; myText;
};<br>
// Close the file
MyReadFile.close();
</pre>
