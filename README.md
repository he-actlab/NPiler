# README #

This README would normally document whatever steps are necessary to get your application up and running.

### What is this repository for? ###

* Quick summary
* Version 1
* [Learn Markdown](https://bitbucket.org/tutorials/markdowndemo)

### How do I get set up? ###
As the era of Dennard scaling comes to an end, both the semiconductor industry and the research community are searching for solutions which allow energy efficiency and performance to continue to scale while retaining generality and programmability.
%
Programmable accelerators, which exploit some common characteristic within a \textit{domain} of applications to achieve efficiency gains at the cost of some generality, have emerged as a possible answer. One such characteristic, present in many modern applications, is \textit{tolerance to approximation}. As a result, approximate accelerators are a new class of accelerators that focus on strategies for improving efficiency and maintaining generality at the cost of strict program accuracy. In particular, one promising strategy is to ``learn'' the behavior of a region of code using artificial neural networks which, although inherently imprecise, are highly efficient to compute on specialized hardware and can run as a surrogate for the original precise code.
%
In this report, we develop NPiler, an automatic compilation framework for transforming regions of code to a neural-network representation.
%
NPiler consists of three phases: programming, in which the programmer marks candidate regions for the transformation; compilation, in which the compiler selects a topology and trains a suitable neural network; and execution, where the original code is replaced with instructions to invoke the specialized neural accelerator, pass inputs, and retrieve outputs.
%
We have developed NPiler to efficiently create and execute an efficient neural representation of the code on both on a traditional CPU and in a SIMD environment such as CUDA or AVX.
