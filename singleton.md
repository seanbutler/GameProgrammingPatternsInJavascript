# Entity

## Rationale

It can be useful in complicated systems to have complete control over the initialisation of a global object. In particular for memory use when a class manages many others such as an game engine or service.

Sometimes we want to ensure that only one instance of a particular object is created. Consider a manager class or similar which has to maintain control over every entity. Perhaps it contains the main loop. We only want one.

The Singleton pattern addresses both of these problems.

## Related To

- service

### Synonyms

## Discussion

## Implementation

~~~javascript
let instance = null;

class EngineService{  
    constructor() {
        if(!instance){
              instance = this;
        }
		else {
			// this is just test code to confirm whether we have singleton or not, dont need this in your version
	        this.time = new Date()			
		}

        return instance;
      }
}

let cache1 = new Cache()
let cache2 = new Cache()
// both variables are the same object
~~~

## External Links
