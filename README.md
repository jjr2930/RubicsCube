# RubicsCube
My apple native game application, control rubics cube and solve problem to original

# SceneGraph
- Root1 : [GameObject]
  - Child1 : [GameObject]
    - ChildChild1 : [GameObject]
    - ChildChild2 : [GameObject]
      - ChildChildChild1 : [GameObject]
        - ChildCHildChildCHild1 : [GameObject]
    - ChildChild3 : [GameObject]
  - Child2 : [GameObject]
- Root2 : [GameObject]
  - Child1 : [GameObject]
  - Child2 : [GameObject]

# how to Rotate
Use Scene Graph
- Front
- Back
- Left
- Right
- Top
- Bottom

# Class description
### 1. Game
##### Members variables
```
var scenes : [Scene] : scene list of this game.
var startScene : Scene : what is start scene of this game.

and insert here about games options... or create option class
```
##### Member functions
```
init() : setup games
Update() : update games logic
Render() : create render queue, and commit to gpu, wait until gpu will complete calc
```

### 2. Scene
###### Member Variables
```
var sceneObjects : [GameObject] : Things to composite a scene.
```
###### Member functions
```
init() : initailize sceneObjets recursively
Update() : Update sceneObjects recursively
Render() : Render sceneObjects recursively
```

### 3. GameObject 
###### Member varibles
```
var transform : Transform  -> it has 3d transformation's information
var components : [Component] -> it has every component for this object..
```
###### Member fucntions
TBD
