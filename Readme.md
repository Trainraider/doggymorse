# Doggy Morse Code
 This program can encode ordinary text into a varient of morse code expressed with barking.

 For example, "Hello world!" becomes:
 
 > bork bork bork bork ruff bork ruff bork baaark bork bork ruff bork baaark bork bork ruff baaark baaark baaark ruff ruff bork baaark baaark ruff baaark baaark baaark ruff bork baaark bork ruff bork baaark bork bork ruff baaark bork bork ruff baaark bork baaark bork baaark baaark ruff 
 
 Morse code mapping:
 
 | Doggy | Morse |
 |-------|-------|
 | bork  | .     |
 | baaark| -     |
 | ruff  | /     |

 ## Usage

 ```
$ doggymorse -h
usage: doggymorse [-h] (-d | -e) [input]

Translate between English and Doggy Morse Code

positional arguments:
  input          Input string to translate

options:
  -h, --help     show this help message and exit
  -d, --doggy    Translate to Doggy Morse Code
  -e, --english  Translate to English

$ doggymorse -d "Hello"
bork bork bork bork ruff bork ruff bork baaark bork bork ruff bork baaark bork bork ruff baaark baaark baaark ruff

$ doggymorse -e "bork bork bork bork ruff bork ruff bork baaark bork bork ruff bork baaark bork bork ruff baaark baaark baaark ruff"
HELLO

$ echo "Hello" | doggymorse -e
bork bork bork bork ruff bork ruff bork baaark bork bork ruff bork baaark bork bork ruff baaark baaark baaark ruff
 ```

### Unix, Linux, MacOS, etc.

 The doggymorse source file is ready to be ran as a script directly on any Unix-like system with python installed and python3 in the PATH. You may need to `chmod +x doggymorse` if it doesn't have permission to execute however.

### Windows

Install python 3 and make sure it is in your path. Open a terminal like cmd and enter the src folder. Run `python doggymorse -d "Hello"` for example.
