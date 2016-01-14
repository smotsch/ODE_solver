Numerical solver for differential equations
===========================================

**Table of Contents**
- [Presentation](#presentation)
- [Numerics](#numerical-method)
- [Credits](#credits)


## Presentation
This program aims at solving numericallly differential equations of the form:

	`x'=f(x,y) , y'=g(x,y)`
	
The user specifies the functions `f` and `g` in the address bar.

Some examples:
* [`x'= cos y, y'=sin(x)`](http://seb-motsch.com/geek/solver_RK4.html?xprime=cos%28y%29&yprime=sin%28x%29)
* [`x'= 1-y, y'=x*y`](http://seb-motsch.com/geek/solver_RK4.html?xprime=1-y&yprime=x*y)
* [`x'= xy+xy(1-x^2+y^2), y'=-x^2+y^2*(1-x^2+y^2)`](http://seb-motsch.com/geek/solver_RK4.html?xprime=x*y+x*y*%281-x*x+y*y%29&yprime=-x*x+y*y*%281-x*x+y*y%29) (*Butterfly*)

## Numerical method

The script uses the popular Runge-Kutta method of order $4$ (also known as [RK4]( https://en.wikipedia.org/wiki/Runge-Kutta_methods)) to discretize the differential equations. Right now, the discretization step `Δt` is fixed (`Δt=.02`) but we will let the user changes this value in a future release

## Credits

The script has been inspired from [universefactory](http://universefactory.net/). The design has been updated by [Adrien](https://github.com/amotsch). 

<!--  http://universefactory.net/test/difeq.html?yprime=-x*x&xprime=y -->
