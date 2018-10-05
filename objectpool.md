# Object Pool

## Rationale

Some games create a large number of identical or similar objects which may have a very short lifetime. For example particles or some simple enemies.

The allocation and deallocation of memory for an object takes time, this time can be avoided if we re-use the same object with new parameters.

If we create and destroy the same object repeatedly then the memory can end up being 'fragmented' which means when we ask for a piece of memory the only options are small pieces so no large objects can be created.

If we create a large number of small objects and keep them constructed then we gain a speed increase at the expense of memory usage. Overall memory usage goes up but the specific total becomes less volatile and more constant.

## Related To

- entity

### Synonyms

- circular buffer

### Makes Use Of

## Discussion

This method can be created through inheritance, composition or as a normal method.

## Implementation

This simple implementation reuses footprints in a naive circular buffer. More sophisticated implementations exist with various benefits.

~~~javascript
class Footprint {
    constructor() {this.initialise(0, 0, 0);}

    initialise(x, z, colour) {
		this.x = x;
		this.z=z;
		this.colour = colour;
	}
}

class FootprintPool {
    constructor(size) {
        this.size = size; this.new = 0;
        for (var n=0; n < this.size; n++) {
            this.poolArray.push(new Footprint(0,0,0));
        }
    };

    NewFootprint(x, y, z, c) {
        this.poolArray[new].initialise(x, z, c);
        this.new = this.new + 1;
        if (this.new>=this.size) {this.new = 0;}
    }
}

~~~


## External Links
