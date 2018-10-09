# Update Method

## Rationale

When we have a large number of self-similar software objects it can be convenient to have control flow of the larger system visit each of these in turn.

A pattern has emerged where each object has an update method.

## Related To

- entity
- game loop

### Synonyms

- tick method
- logic method
- execute method

### Makes Use Of

## Discussion

This method can be created through inheritance, composition or as a normal method.


## Implementation

~~~javascript
class GameObjectOrOtherActiveClass() {
	update() {
		// update and/or realise my current state externally
	}
}

CalledAtRegularIntervals() {

	// inside the game loop or some manager?
	for (var i = 0; i < numEntities; i++)
	{
		entities[i]->update()
	}
}


~~~

## External Links
