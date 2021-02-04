# bloch-sim-py
The original bloch equation simulator was a matlab mex file created by Brian Hargreaves at Stanford University. 
This is a modification to run it as a python C extension.
The simulator was used in a graduate MRI class taught by Miki Lustig. 
Lustig wrote several helper modules in matlab, which have also been converted to python here.

This module was developed on a linux platform and has been since been tested on macos 10.14.6.

Minor edits by Gopal Nataraj

## Dependencies
`python 3.7`<br>
`numpy 1.16.4`<br>
`scipy 1.3.0`<br>
`matplotlib 3.1.0`<br>

Other versions have not been tested, but there should be some flexibility.

## Installation
First, make sure your build environment can build python c extensions. [Here](http://notesbyanerd.com/2018/11/02/pip-install-cant-find-numpy-header/) are some instructions that may help on macs. 

Next, run `pip install -e .` from the base directory.

Use `from bloch import bloch` for the primary bloch simulator function. 

## Testing
Run `python -m unittest` from the base directory.

## License
This library is distributed under the same terms as Brian's original bloch simulator.

## Acknowledgments
Thanks to Brian for the original bloch simulator, 
Miki for the helper modules, 
and NPann for assisting with a critical bug fix.
