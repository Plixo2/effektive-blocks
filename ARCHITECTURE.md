

### High level code structure

The [main.effekt](src/main.effekt) file is responsible for the web interface and user interaction. 
The Wave Function Collapse implementation is located in the [wfc](src/wfc) folder.
The FFI and wrappers are located in the [lib](src/lib) folder and the [ffi.effekt](src/ffi.effekt) file.

Each file contains a more detailed description of its contents and purpose.
Some files have a `/* Interface */` section at the bottom that lists the main functions that are intended to be used by other files.

### Web Interface

[main.effekt](src/main.effekt)  
    Contains all the layouting and updating of the web interface
    See the `createWFCContext` function for handling of user data & the `render` function for updating the DOM grid


### Wave Function Collapse Implementation

[adjacency.effekt](src/wfc/adjacency.effekt)  
    Contains the core logic for rule generation based on a uploaded ruleset image

[wfc1.effekt](src/wfc/wfc1.effekt)  
    First, naive implementation of the Wave Function Collapse algorithm. Not used anymore, but kept for reference.

[wfc2.effekt](src/wfc/wfc2.effekt)  
    Current implementation of the Wave Function Collapse algorithm, using propagation. \
    See the `wfcStateGrid` function for initializing a new grid. \
    See the other functions described below the `wfcStateGrid` function, like `step` or `solve`, to run the algorithm.



### FFI and Wrappers

[ffi.effekt](src/ffi.effekt) \
    This file contains the full ffi to javascript (FFI namespace) \
    These functions should never be used directly, but rather through the wrappers (see below)


[dom.effekt](src/lib/dom.effekt) \
    Wrapper around the ffi functions for DOM manipulation (FFI::DOM namespace) \
    These functions are mainly used in the main file to layout the web interface

[canvas.effekt](src/lib/canvas.effekt) \
    Wrapper around the ffi functions for canvas manipulation (FFI::Canvas namespace) \
    These functions are used to create and manipulate canvas elements and images

[array.effekt](src/lib/array.effekt) \
    Wrapper around the ffi functions for array manipulation (FFI::Array namespace) \
    Used for manipulating arrays of tiles and rules. These wrap existing javascript array methods. 
    Arrays are mainly used for better speed.

[color.effekt](src/lib/color.effekt) \
    Color utilities. Used to extract rules from images



### WFC Algorithm references & other implementations

- https://en.wikipedia.org/wiki/Wave_function_collapse
- https://github.com/mxgmn/WaveFunctionCollapse
- https://robertheaton.com/2018/12/17/wavefunction-collapse-algorithm/
- https://bolddunkley.itch.io/wfc-mixed / https://www.youtube.com/watch?v=2SuvO4Gi7uY
- https://oskarstalberg.com/game/wave/wave.html 