---
ID_PAGE: 25258
PG_TITLE: CSG
PG_VERSION: 2.1
---
##Description

class [CSG](/classes/2.2/CSG)



##Members

###matrix : [Matrix](/classes/2.2/Matrix)

The matrix

###position : [Vector3](/classes/2.2/Vector3)

The position

###rotation : [Vector3](/classes/2.2/Vector3)

The rotation

###rotationQuaternion : [Quaternion](/classes/2.2/Quaternion)



###scaling : [Vector3](/classes/2.2/Vector3)

The scaling

##Methods

###static FromMesh(mesh) &rarr; [CSG](/classes/2.2/CSG)

Convert [Mesh](/classes/2.2/Mesh) to [CSG](/classes/2.2/CSG)

####Parameters
 | Name | Type | Description
---|---|---|---
 | mesh | [Mesh](/classes/2.2/Mesh) | 

###clone() &rarr; [CSG](/classes/2.2/CSG)

Clone this [CSG](/classes/2.2/CSG)
###union(csg) &rarr; [CSG](/classes/2.2/CSG)

Union the [CSG](/classes/2.2/CSG)

####Parameters
 | Name | Type | Description
---|---|---|---
 | csg | [CSG](/classes/2.2/CSG) | 

###unionInPlace(csg) &rarr; void

Union in place

####Parameters
 | Name | Type | Description
---|---|---|---
 | csg | [CSG](/classes/2.2/CSG) | 

###subtract(csg) &rarr; [CSG](/classes/2.2/CSG)

Subtract the [CSG](/classes/2.2/CSG)

####Parameters
 | Name | Type | Description
---|---|---|---
 | csg | [CSG](/classes/2.2/CSG) | 

###subtractInPlace(csg) &rarr; void

Subtract in place

####Parameters
 | Name | Type | Description
---|---|---|---
 | csg | [CSG](/classes/2.2/CSG) | 

###intersect(csg) &rarr; [CSG](/classes/2.2/CSG)

Intersect first solid with the second

####Parameters
 | Name | Type | Description
---|---|---|---
 | csg | [CSG](/classes/2.2/CSG) | 

###intersectInPlace(csg) &rarr; void

Intersect in place

####Parameters
 | Name | Type | Description
---|---|---|---
 | csg | [CSG](/classes/2.2/CSG) | 

###inverse() &rarr; [CSG](/classes/2.2/CSG)

Return a new [CSG](/classes/2.2/CSG) solid with solid and empty space swtiched. This solid is not modified.
###inverseInPlace() &rarr; void

Inverse in place
###copyTransformAttributes(csg) &rarr; [CSG](/classes/2.2/CSG)

This is used to keep meshes transformations so they can be restored
when we build back a [Mesh](/classes/2.2/Mesh)
NB : All [CSG](/classes/2.2/CSG) operations are performed in world coordinates

####Parameters
 | Name | Type | Description
---|---|---|---
 | csg | [CSG](/classes/2.2/CSG) | 

###buildMeshGeometry(name, scene, keepSubMeshes) &rarr; [Mesh](/classes/2.2/Mesh)

Build raw mesh from [CSG](/classes/2.2/CSG)
Coordinates here are in world space

####Parameters
 | Name | Type | Description
---|---|---|---
 | name | string | 
 | scene | [Scene](/classes/2.2/Scene) | 
 | keepSubMeshes | boolean | 

###toMesh(name, material, scene, keepSubMeshes) &rarr; [Mesh](/classes/2.2/Mesh)



####Parameters
 | Name | Type | Description
---|---|---|---
 | name | string | 
 | material | [Material](/classes/2.2/Material) | 
 | scene | [Scene](/classes/2.2/Scene) | 
 | keepSubMeshes | boolean | 
