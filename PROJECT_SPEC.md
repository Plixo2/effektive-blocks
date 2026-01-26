


# Effektive Blocks

A browser page for map generation, based on the _wave function collapse_ algorithm, where users can upload their own art and generate a realistic looking world.

## Must-have

- Functional _wave function collapse_ algorithm
- Web interface:
     - Generate a map automaticly
     - Set speed of visualization
- A way of loading user generated content
- Good errors when a user makes a mistake
- A explanation on how to use the tool (short!)
- Random map each time


## Can-have

- A way to set up rules what tile can connect to another (otherwise fixed)
- A way to set weights for certain tiles
- Incremental execution of the WFC algorithm
- importing/exporting of the map (e.g. json or the 'tiled' format, but dont know how complex this is)
- abiliy to download a map as an image

## Will-not-have

- Any kind of 'game' interactivity
- A explanation on how wfc works
- any advanced graphic effects 
- sound
- Any online interactivity, except links

## Effects and Handlers

- For implementing the main step of the _wave function collapse_ algorithm
- Any mutability, when applicable
- HTML layouting and css styling
- Error reporting for user errors

## FFI and Libraries

- Custom handlers for the HTML dom (e.g. creating elements, installing hooks and getting data from <\input> elements)
- A way to process images (Javascript Canvas)
