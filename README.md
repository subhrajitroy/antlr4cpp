# Grammar installation

Download the following files \

[CPP14Parser.g4](https://github.com/antlr/grammars-v4/blob/master/cpp/CPP14Parser.g4) \

[CPP14Lexer.g4](https://github.com/antlr/grammars-v4/blob/master/cpp/CPP14Lexer.g4) \

[CPP14ParserBase.py](https://github.com/antlr/grammars-v4/blob/master/cpp/Python3/ CPP14ParserBase.py) \

[transformGrammer.py](https://github.com/antlr/grammars-v4/blob/master/cpp/Python3/CPP14ParserBase.py) \

# Install antlr4 tools

pip install antlr4-tools

# Install antlr4 runtime

pip install antlr4-python3-runtime

# Run the transformGrammer

It apparantly transforms Grammer files to fit target python in this case python 3 \

- Checked in Grammar files are already transformed. The \*.bak files are the original ones \*
  python transformGrammar.py \

# Generate the parsers in python using the Antlr tools

- Step 1 \*
  antlr4 -Dlanguage=Python3 CPP14Lexer.g4 -o generated

- Step 2 \*
  antlr4 -Dlanguage=Python3 CPP14Parser.g4 -visitor -o generated

Files will be generated in the generated file
