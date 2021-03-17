# headerFileCPPMac
This is the infamous CPP header &lt;bits/stdc++.h> file for the Mac Operating System. 
It took me a while to figure out that that the MacOS does not have the bits/stdc++.h header file which is so convenient for cpp programmers. 
I am noob at CPP ,so yeah. I finally managed to include the header file after a bit of google searching and decided to create this short tutorial on how this header thing works for MacOS. 

Windows by default is in the GCC Compiler whereas MacOS is configured in Clang. 

The Clang Compiler does not have this header file hence we need to manually create one directory from where the contents of the bits/stdc++.h header file can be grabbed from. 

Steps to create this directory. 

Step 1 : Install a Package manager for the MacOS : [Homebrew](https://brew.sh/)

Step 2 : Open the terminal and install the GCC compiler in your MacOS
         
         brew install gcc

Step 3 : Go to the given directory by typing the following commands in your terminal 

         cd ~ 
         cd /usr/local/include
         mkdir bits
         cd bits 

Step 4 : Now that you are in the bits directory, copy the above contents in the stdc++.h file inside the directory by creating a new file using the following commands. 

         sudo nano stdc++.h
         copy paste the contents 

Now your cpp file is ready for compilation. 
         
