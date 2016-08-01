---
layout: post
title: "[Compiler] Term Project"
date: 2004-05-07 21:25
categories: ⊙ 전공노트
---

**MinimL Project**

The purpose of the project is to implement a functioning interpreter for the MinimL programming language. The MinimL programming language was developed by Prof. Doug Baldwin for educational purposes, and much of this project description is borrowed from his specification of the language and related programming projects:

**Reference:**
The MinimL language. http://www.cs.geneseo.edu/~baldwin/csci331/spring2003/miniml.html

You can also use the MinimL test source files in the course homepage to test your program.


If a file named lib.min is available in the current directory (see the collection of example source codes), its content should be read along with the content of the specified file. The implementation of MinimL should follow the following steps: 

* Scanner: Write a formal specification of the MinimL lexical conventions as an EBNF grammar, and transform the grammar to LL(1) EBNF. Implement a recursive-decent scanner which prints the type and spelling of each MinimL token encountered in the input file to the standard out. 

* Parser: Transform the MinimL grammar from the previous section into LL(1) EBNF and implement a recursive-decent parser. The parser should indicate whether the input is correct or not. 

* Tree Builder: Design an abstract syntax for MinimL, and extend the parser so that it builds an AST according to the abstract syntax. Verify that the trees are correct by implementing tree printers and/or pretty printers as visitors 

* Context Checker: Identify which tasks are to be performed by the context cheker, and implement a context checker as a visitor. Decide how the AST should be decorated. 

* Interpreter: Identify the need for run-time entities, and implement an MinimL interpreter as a visitor.

       
