# tetgen #

This is a mirror of **tetgen** (www.tetgen.org). Tetgen is used under the AGPL license.

## INSTALLATION: ##
Install ugmat with ug4's package manager [ughub](https://github.com/UG4/ughub):

    ughub install tetgen

Or simply clone this repository to any place on your harddrive.


## BUILDING: ##
### As part of UG4 (e.g. after installing ugmat through 'ughub install tetgen'): ###
Go to your ug4 build directory and execute:

	cmake -Dtetgen=ON .
	make

The resulting tetgen executable will be written to ug4/bin


## FURTHER INFORMATION: ##
Please find tetgen's original README below:

###
This is TetGen version 1.5 (released on November 4, 2013)

Please see the documentation of TetGen for compiling and using TetGen.
It is available at the following link:

            http://www.tetgen.org

For more information on this product, contact :

  Hang Si
  Research Group of Numerical Mathematics and Scientific Computing
  Weierstrass Institute for Applied Analysis and Stochastics
  Mohrenstr. 39
  10117 Berlin, Germany

 Phone: +49 (0) 30-20372-446   Fax: +49 (0) 30-2044975
 EMail: <si@wias-berlin.de>
 Web Site: http://www.wias-berlin.de/~si

------------------- IMPORTANCE NOTICE -----------------------------

BEFORE INTALLING OR USING TetGen(R) READ the 
GENERAL LICENSE TERMS AND CONDITIONS

-------------------------------------------------------------------
###