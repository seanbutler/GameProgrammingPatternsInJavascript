# Entity

## Rationale

Typically in a modern computer game, many similar software objects are used to represent a large number of similar game elements, such as enemies, collectables, obstacles, etc.

Each of these kinds of objects have code in common which is required to participate in a game. The entity (or game object) pattern holds the interface so they can all participate in the same larger system.

## Related To

- component
- system
- gameloop

### Synonyms
- game object

### Makes Use Of
- update method

## Discussion

## Implementation

~~~javascript
// declaration of the loop in a browser context
class Entity() {
	constructor() {
		// ...
		self.position = new Position(0, 0, 0)
		// etc
	}

	update() {
		// ...
	}

	draw() {
		// ...
	}
}

class Zombie() extends Entity {}
class Critter() extends Entity {}
class Avatar() extends Entity {}

~~~

## External Links
