This version we modified the code to deal with the case that param_card.dat is generated by SPheno. Sometimes it can't be directly used in MG5 and it needs "update missing" to update the parameter file and make MG5 work smoothly. 

Installation Guide 
Environment Setup:
  1. Python2.7.X(X>3)
  2. Delphes 3.4.2(Delphes3.5.0 will not work). When installing Delphes 3.4.2, need to modify Delphes/validation/DelphesValidation.cpp, add "#include TF1.h" and then make
  3. Pythia 8245(Pythia 8.3 will not work)
  
Steps: 
  1. git clone [website]
  2. autoreconf  ----> If can't autoreconf, $export ACLOCAL_PATH="/usr/share/aclocal/:/usr/local/share/aclocal"
  3. ./configure
  4. make -j4
