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
// declaration of the loop in a browser context
class Entity() {

	update() {
		// update and/or realise my current state externally
	}
}

~~~

## External Links
