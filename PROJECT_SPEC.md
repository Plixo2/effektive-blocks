


# Effektive Blocks

A browser page for map generation, based on the _wave function collapse_ algorithm, where users can upload their own art and generate a realistic looking world.

## Must-have

- [x] Functional _wave function collapse_ algorithm
- [x] Web interface:
     - [x] Generate a map automaticly
     - [x] Set speed of visualization
- [x] A way of loading user generated content
- [x] Good errors when a user makes a mistake
- [x] A explanation on how to use the tool (short!)
- [x] Random map each time


## Can-have

- [x] A way to set up rules what tile can connect to another (otherwise fixed)
- [ ] A way to set weights for certain tiles
- [x] Incremental execution of the WFC algorithm
- [ ] Importing/exporting of the map (e.g. json or the 'tiled' format, but dont know how complex this is)
- [x] Abiliy to download a map as an image

## Will-not-have

- [x] Any kind of 'game' interactivity
- [x] A explanation on how wfc works
- [x] any advanced graphic effects 
- [x] sound
- [x] Any online interactivity, except links

## Effects and Handlers

- [ ] For implementing the main step of the _wave function collapse_ algorithm
- [x] Any mutability, when applicable
- [x] HTML layouting and css styling
- [x] Error reporting for user errors

_The Wave Function Collapse does not use effects for its core logic anymore for performance reasons_

## FFI and Libraries

- [x] Custom handlers for the HTML dom (e.g. creating elements, installing hooks and getting data from <\input> elements)
- [x] A way to process images (Javascript Canvas)
