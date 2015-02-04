Hello Roberto,
      For your intro to c, here are the basics you need to know.
      EMACS is the defaut editor however you could also try nano or VIM.
      To create a file in emacs, use C^x C^f to specify the name of the file that you wish to create. This will also open the file if it already exists.
      To save, use C^x C^s (Execute, Save)
      To quit, use C^x C^c (Execute, Close)
      
      I have included a very simple sample program for you to look at. I'm sure you will also use the internet to learn syntax etc.

      When you have a .c file that you are ready to compile and run, here are the neccesary steps.
      You need to create a make file. (There is a sample one in the sample folder)
      It can be replicated almost exactly with the name changes from sample to whatever your project name is. The first statement "sample: all" tells the make file that it should monitor all files in the sample folder.
      The rest is the use for the compiler. For the most part clang will be a good compiler.
      Once the Makefile (capital M) is set up then you can use the command "make" from within the directory also containing a Makefile. this will compile your program to the output specified in the Makefile.

      After the c program is created you can execute by running "./programname" it should not have a file type as it is an executable binary. The output will be sent to stdout and can then be piped wherever you want.

      Another nifty tool is valgrind. The arguements used is "valgrind ./programname" this is what can be used to track memory usage and leaks.

      If you actually make it this far it will be more than I expected you to lean in 1 day. I'll have more for you later.

Update 1:
	So I have decided that I will try to keep updating this file occasionally with more information or tips.
	They may or may not be directly related to c but they will have to do with things that can be done on the pi/linux.
	Here is a shortlist of commands that you need to figure out to use very naturally:
	ls [-la]
	cd
	rm [-r]
	mv
	less
	cat
	echo 'used to create files often
	Use of the operands >> with echo to create a file
	grep
	emacs/vim/nano (pick one)
	| 'PIPE!!! (one of the things that makes linux awesome.
	
	even knowing how to fluently use this short set of commands will let you navigate around and manipulate files.

Update 2: I doubt you'll ever read this.
