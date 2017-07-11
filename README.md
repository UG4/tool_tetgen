# tetgen #

This is a mirror of **tetgen** (www.tetgen.org). Tetgen generates tetrahedral meshes with prescribed quality constraints. Tetgen is used under the AGPL license.

## INSTALLATION: ##
Install ugmat with ug4's package manager [ughub](https://github.com/UG4/ughub):

    ughub install tetgen

Or simply clone this repository to any place on your harddrive.


## BUILDING: ##
### As part of UG4 (e.g. after installing tetgen through 'ughub install tetgen'): ###
Go to your ug4 build directory and execute:

	cmake -Dtetgen=ON .
	make

The resulting tetgen executable will be written to ug4/bin
