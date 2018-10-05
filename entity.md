# Entity

## Rationale

Typically in a modern computer game, many similar software objects are used to represent a large number of similar game elements, such as enemies, collectables, obstacles, etc.

Each of these kinds of objects have code in common which is required to participate in a game. The entity (or game object) pattern holds the interface and possibly overlapping functionality so they can all participate in the same larger system. Because they all are part of the same simulation we don't want to re-write the code each time.

## Related To

- component
- system
- gameloop

### Synonyms

- game object
- agent
- actor

### Makes Use Of
- update method

## Discussion

## Implementation

~~~javascript
// declaration of the loop in a browser context
class Entity() {
	constructor(x, y, z) {
		// ...
		self.position = new Position(self.x, self.y, self.z)
		// etc
	}
}

class Avatar() extends Entity {}
class Enemy() extends Entity {}
class Nazi() extends Enemy {}
class Zombie() extends Enemy {}

~~~

## External Links
