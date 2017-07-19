## About:
This repository contains the LaTeX sources for my bachelor thesis about implementing generators support within a [PHP to CIL compiler Peachpie](https://github.com/peachpiecompiler/peachpie) that was written at Charles University in Prague in 2017. You can find the final .pdf [here](https://github.com/petrroll/bachelor-thesis/raw/master/text/thesis.pdf).

## Abstract:

The goal of this thesis is to design and implement the support for generators within the Peachpie framework, a PHP to CIL compiler. Generators are the simplest form of methods that resume from the same state in which they returned earlier when called repeatedly. 

The reference PHP interpreter Zend engine supports generators natively. Due to that fact that generators in PHP support a number of features that are not common in other languages. CIL, on the other hand, does not have a native support for generators. Therefore, languages built on top of CIL (e.g. C#, F#) have to implement them by other means, such as by rewriting the original generator methods into state machines. 

In this thesis, we will design and implement the support for generators through semantic tree transformations. All this is handled with the intention of keeping the maximum possible compatibility with reference PHP generators. We will also make a comparison to generators in C\#, whose main implementation also uses CIL as a backend.

## Prerequisites:
- LaTeX
- Python on path
- `pygments` [package](http://pygments.org/)

## Building:
- Makefile located [in](https://github.com/petrroll/bachelor-thesis/blob/master/text/Makefile) `text/Makefile`