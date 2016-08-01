---
layout: post
title: "Java에서 사용할 수 있는 matrix 관련 API"
date: 2006-05-23 12:00
categories: ⊙ 전공노트
---

COLT project ([http://dsd.lbl.gov/%7Ehoschek/colt/](http://dsd.lbl.gov/%7Ehoschek/colt/))
 This distribution consists of several free Java libraries, for user convenience bundled under one single uniform umbrella. Namely the Colt library, the Jet library, the CoreJava library, and the Concurrent library. The Colt library provides fundamental general-purpose data structures optimized for numerical data, such as resizable arrays, dense and sparse matrices (multi-dimensional arrays), linear algebra, associative containers and buffer management. The Jet library contains mathematical and statistical tools for data analysis, powerful histogramming functionality, Random Number Generators and Distributions useful for (event) simulations, and more. The CoreJava library contains C-like print formatting. The Concurrent library contains standardized, efficient utility classes commonly encountered in parallel & concurrent programming.  JmatrixView ([http://jmatrixview.sourceforge.net/](http://jmatrixview.sourceforge.net/))

The JMatrixView project is aimed at matrix visualization. It provides a reliable java widget/component for matrix visualizationthat one will be able to embed in its own software. Implementation is in Java 1.4.2. Thanks to the Colt matrix package ([http://dsd.lbl.gov/~hoschek/colt/](http://dsd.lbl.gov/%7Ehoschek/colt/)) JMatrixView can support huge matrix, that can eventulally be sparse. It features rows and columns labelling and customizable CellRenderer-s : cells of the matrix can be rendered as small squarres, rectangles, circle, triangle, etc, and with gradient of colors taking into account the value stores in the cell. 



       
