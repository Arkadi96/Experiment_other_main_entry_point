# assignment-1
This is first assignment:Hello World!
Create a simple program that prints out “Hello World!” on a console.
Compile and run the program from command prompt by using Visual C# command-line compiler (csc.exe).
Compile provided files into an assembly and then using created assembly and Program.cs file produce executable file.
Change the entry point of the program to be other method (not Main), recompile and create PE file.After completed homework provide a github link with solution.

Answer

•	create in a text editor C# code that prints “hello world (main)” text into console with one main function and another one with main2 function that prints “hello world(desired main)” text.

•	save document with helloworld.cs extension

•	open command prompt and set path of csc.exe (Visual studio’s compiler)
path=%path%;C:\Windows\Microsoft.NET\Framework\v4.0.30319

•	compile helloworld.cs
csc.exe helloworld.cs

•	open created helloworld.exe (prints Hello world (Main))

•	to change main function we should make changes into IL code so we open visual studio’s command prompt from it’s directory.

•	Create helloworld.il by using ILDasm utility provided by the .NET 
ildasm helloworld.exe /out=helloworld.il

•	Open created helloworld.il file via text editor and make changes namely find  “.entrypoint” under main function and move down and set under main2 function, save the file.

•	use the utility ILASM provided by the .NET to generate an assembly from an .IL file.
ilasm helloworld.il

•	all we need Is just open via cmd our updated helloworld.exe
Hello World (Desired Main) 

