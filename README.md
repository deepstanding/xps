# xps
This repository provides an R package for people who wonder how the phase problem can be solved and/or want to explore the possibility to solve protein structures at low resolution. It is a very much simplified version of my C++ package sxMatrix (Acta Cryst. A68, 298-300 (2012)), but enough to start with. Play with it and extend it in your own way, you might be able to complete the century-old challenge (http://www.nobelprize.org/nobel_prizes/chemistry/laureates/1962/perspectives.html).

An R wrapper of the 3D FFTW function is included following the style of the fftwtools package, which covers only 1D and 2D fftw functions. The FFTW library should be properly installed in your system (linux).

An example to run the program:
  x <- load.xps("~/xps/data/1ejg-sf.cif"); 
  rho <- solve.xps(x, 100, 680)
  
