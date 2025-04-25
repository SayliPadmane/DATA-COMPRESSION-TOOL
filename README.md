# DATA-COMPRESSION-TOOL

COMPANY = CODTECH IT SOLUTIONS

NAME = SAYALI PADMANE

INTERN ID = CT04WR115

DOMAIN = C PROGRAMMING

DURATION = 4 WEEKS

MENTOR = NEELA SANTOSH


DESCRIPTION:
Explanation of the RLE Compression Program (in C)
This C program is built to compress and decompress text files using a simple method called Run-Length Encoding (RLE). It’s a basic yet powerful algorithm that shrinks repetitive data to save space — and then can restore it perfectly.

Let’s say you have a file that contains the text:
AAAABBBCCDAA
Instead of storing each character individually, RLE counts how many times each character repeats in a row and stores the count with the character. So the example becomes:
4A3B2C1D2A
Now that’s shorter and more efficient!

 How the Program Works
When you run the program, it gives you two choices:
Compress a text file.
Decompress a file that was previously compressed.
Depending on your choice, it asks for the input and output file names and then does the job.

 Inside the Compression
When you choose to compress, the program reads the text in your input file character by character. It keeps track of repeated characters and counts how many times each one appears in a row.
For example, if it sees "AAA", it will count 3 and then write 3A to the output file.
This continues until the whole file is read. The compressed version ends up much shorter if there are lots of repeating characters.
 Inside the Decompression
When you pick the decompress option, the program takes the compressed file and reverses the process. It reads each number and the character that comes after it — like 3A — and then writes that character (A) three times into the output file.
This way, the file goes back to its original form.

💡 Why This is Useful
RLE isn’t the most advanced compression method, but it’s super easy to implement and great for learning how compression works. It’s especially useful in cases where there’s a lot of repetition — like in black-and-white images, simple patterns, or even some types of logs and documents.

🛡️ Error Handling & File Safety
The program also checks if the files open correctly. If you mistype a filename or the file doesn’t exist, it lets you know instead of crashing.
It uses simple file functions from C like:
fopen() to open files
fgetc() to read one character at a time
fprintf() and fscanf() to write and read formatted text
fputc() to write single characters

OUTPUT

![Image](https://github.com/user-attachments/assets/22054deb-0d94-410b-87f1-6a1ac220891d)

Use loops and conditions

Understand real-world applications of simple algorithms

Even though it’s basic, it forms the foundation of more complex compression tools like ZIP or image compressors.
