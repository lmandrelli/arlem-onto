## Extensions to the ARLEM Ontology

In addition to the base model defined by IEEE-ARLEM, this ontology provides the following extensions:

1.  Detailed 3D and Multimedia Primitives  
    - `Model3D` abstraction to handle any 3D model (GLB, OBJ)  
    - `fileFormat` property to specify the format of each 3D resource (string).  

2.  AR/VR Primitive Types  
    - `PrimitiveType` enumeration (cube, sphere, cylinder, cone, custom) to catalog basic geometric shapes and custom meshes.  
    - `primitiveType` property to link each primitive instance to its VR/AR type.  

3.  Spatial Transforms  
    - `Transform` class with position (`positionX`, `positionY`, `positionZ`), rotation (`rotationX`, `rotationY`, `rotationZ`) and scale (`scaleX`, `scaleY`, `scaleZ`) properties to position any 3D primitive in space.  
    - `hasTransform` property to associate a transform with a primitive.  

4.  Model Format Support  
    - `ModelFormat` enumeration preserved (individuals: `obj`, `glb`) to ensure compatibility with external 3D resources.  

These additions provide fine-grained control over 3D and multimedia resources in the ontology, extending beyond the core ARLEM model.
