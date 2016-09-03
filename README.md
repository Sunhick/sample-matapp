# sample-matapp
sample mat application making use of sample-matlib as a submodule in git

This repository provides a example tutorials for the git submodule command.

1. Clone the repository as, 

   `git clone git@github.com:Sunhick/sample-matapp.git`.
  
  This will get the source code for sample-matapp. However it will not pull the source for the submodules(present under folder /modules).
  
2. Pull the source code for all of the submodules in the .gitmodules. To do that,

   `cd sample-matapp`
   `git submodule init`
   `git submodule update`

3. Now that the source code for the application(sample-matapp) and submodules(sample-matlib) are available. We can go ahead and compile the code. First compile the submodules as 
   `cd modules/matlib/matlib`
   `make`

4. Compile the application as,
   `cd matapp`
   `make`

5. Run the application as, `./main`
