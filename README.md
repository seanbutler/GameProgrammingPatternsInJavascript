# Game Programming Patterns In Javascript
## Overview

There is a list of game programming patterns in common use throughout the industry. Many of (all) these patterns can be seen elsewhere on the web including:

- https://en.wikipedia.org/wiki/Software_design_pattern
- http://gameprogrammingpatterns.com/

This repository is similar to those other sites, except that the patterns are expressed in __javascript__ as written in the context of code running within a __web page in a browser__ or similar environment. In this way they are suitable for __programming web games__ in particular.   

- https://en.wikipedia.org/wiki/A_Pattern_Language

<!--
![Pattern Language](https://upload.wikimedia.org/wikipedia/en/e/e6/A_Pattern_Language.jpg)

_(By Source, Fair use, https://en.wikipedia.org/w/index.php?curid=27713585_) -->

## Categories

We can in reality organise the patterns in any way we might wish. In practice software patterns are an idiomatic use of a language that have evolved organically. As a result rarely fit into one single category. Instead perhaps we should think of these as 'tags' so more than one can apply to a given pattern.

| Category | Description |
|---|---|
| Structural | Arrangement or structure of the code, or the software objects |
| Flow | Controlling the order of execution |
| Decoupling | Separation of software objects and types so they can be manipulated independently |
| Optimisation | Reducing computation, speeding up execution, reducing memory use |
| Other | No doubt there are other tags, what can we think of that is widely applicable? |

## Patterns

|Name|Tags (Categories)| Status |
|---|---|---|
| [update method](./updatemethod.md) |flow, decoupling| done |
| [entity](./entity.md) | structural | done |
| [game loop](./gameloop.md) |flow| done |
| [object pool](./objectpool.md) |optimisation| done |
| [singleton](./singleton.md) |structural| done |

## More Patterns

|Name|Tags (Categories)| Status |
|---|---|---|
| [scene graph](./scenegraph.md) |structural, optimisation| todo |
| [finite state machine](./finitestatemachine.md) | flow, decoupling |  todo |
| [state](./state.md) |decoupling| todo |
| [positionroationscale](./positionroationscale.md) | |  todo  |
| [component](./component.md) | |  todo |
| [entity component system](./entitycomponentsystem.md) | |  todo |
| [spatial partition](./spatialpartition.md) | |  todo |
