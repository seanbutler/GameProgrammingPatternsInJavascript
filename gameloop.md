# Game Loop

## Rationale

In real-time dynamic software a loop is used manage the control flow of the program so that input, state and output are updated continuously and at such a high frequency that the illusion of a continuous reality is maintained.

## Related To

### Synonyms
- coreloop
- mainloop

### Makes Use Of
- update method

## Discussion

In the context of a web browser we use a call to

~~~javascript
requestAnimationFrame()
~~~

with a function as its parameter from within the function to create a looping structure which is initiated by our own code, but continued by the browser with one loop per window paint/render.

Typically in other contexts the game loop can be even driven by the operating system or in some cases an actual while loop.

## Implementation

~~~javascript
// declaration of the loop in a browser context
function gameloop() {

	requestAnimationFrame( gameloop )

    // handle input and logic of the simulation
    get_input()
    do_logic()

    // handle output of the simulation, typically rendering
    do_render()
}

// starting the loop
gameloop()
~~~

## External Links

https://en.wikipedia.org/wiki/Object_pool_pattern
