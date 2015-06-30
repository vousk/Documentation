---
ID_PAGE: 6717
PG_TITLE: OctreeBlock<T>
PG_VERSION: 2.1
---

Create a new OctreeBlock
##new OctreeBlock&lt;T&gt;(minPoint, maxPoint, capacity, depth, maxDepth, creationFunc)



The OctreeBlock constructor




####Parameters
 | Name | Type | Description
---|---|---|---
 | minPoint | [Vector3](page.php?p=6751) | The minimum point
 | maxPoint | [Vector3](page.php?p=6751) | The maximum point
 | capacity | number | @param capacity
 | depth | number | @param depth
 | maxDepth | number | @param maxDepth
 | creationFunc | (entry: T, block: OctreeBlock&lt;T&gt;) =&gt; void | @param creationFunc
---

##Members

###entries : T[]




The entries



###blocks : Array&lt;OctreeBlock&lt;T&gt;&gt;




The blocks



###capacity : number




The capacity of the octreeBlock



###minPoint : [Vector3](page.php?p=6751)




The min point



###maxPoint : [Vector3](page.php?p=6751)




The max point











##Methods

###addEntry(entry) &rarr; void
Add an entry to this octree block. The creationFunc linked to this octreeblock is used on the given entry





####Parameters
 | Name | Type | Description
---|---|---|---
 | entry | T | @param entry
---

###addEntries(entries) &rarr; void
Add an entries to this octree block.





####Parameters
 | Name | Type | Description
---|---|---|---
 | entries | T[] | @param entries
---

###select(frustumPlanes, selection, allowDuplicate) &rarr; void
Select





####Parameters
 | Name | Type | Description
---|---|---|---
 | frustumPlanes | [Plane](page.php?p=6755)[] | [Frustum](page.php?p=6757) plan of the mesh
 | selection | SmartArray&lt;T&gt; | @param selection
optional | allowDuplicate | boolean | True if you want to duplicate it, false otherwise.
---

###intersects(sphereCenter, sphereRadius, selection, allowDuplicate) &rarr; void
Intersects





####Parameters
 | Name | Type | Description
---|---|---|---
 | sphereCenter | [Vector3](page.php?p=6751) | The sphere center
 | sphereRadius | number | The sphere radius
 | selection | SmartArray&lt;T&gt; | The selection element
optional | allowDuplicate | boolean | True if you want to duplicate it, false otherwise.
---

###intersectsRay(ray, selection) &rarr; void
Intersects ray





####Parameters
 | Name | Type | Description
---|---|---|---
 | ray | [Ray](page.php?p=6758) | @param ray
 | selection | SmartArray&lt;T&gt; | @param selection
---

###createInnerBlocks() &rarr; void
