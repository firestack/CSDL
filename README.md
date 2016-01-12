# CSDL: SDL For [Swift(lang)](https://swift.org/)

you need to have SDL installed on your system for this module to work

This module usually uses `/usr/local/include/SDL` for headers 

and

  `-lSDL2` for linking using the standard unix linker `ld`
  
(though both of these can be changed in the module.modulemap file to reflect the configuration of your system)
  
## Errors
### OSX Build
I think the cmake configuration at the moment for OSX installs the libaries wrong as `libSDL2.so` 
is a broken link to `libSDL2-2-4.so.0` which doesn't exist on OSX but rather exists as `libSDL2.dynlib.0`
