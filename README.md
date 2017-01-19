How to setup:
  - Checkout closure-library, closure-compiler, closure-linter and python-gflags next to libphonenumber 
    - git clone https://github.com/googlei18n/libphonenumber/   
    - git clone https://github.com/google/closure-library/
    - git clone https://github.com/google/closure-compiler.git
    - git clone https://github.com/google/closure-linter.git
    - git clone https://github.com/google/python-gflags.git
    
 How to compile:
  - Install Homebrew: 
    - /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"  
  - Install Java: 
    - brew cask install java
  - Install Maven: 
    - brew install maven
  - Install Ant: 
    - brew install ant
  - Build Closure's compiler.jar: 
    - cd closure-compiler
    - mvn -DskipTests
  - Compile the phonenumberutil.js file and all its dependencies to one file (phonenumberutil-compiled).js:
    - cd libphonenumber
    - ant -f javascript/build.xml compile-demo
    
