---
ID_PAGE: 3365
PG_TITLE: RenderingManager
PG_VERSION: 1.14
---
##new [RenderingManager](page.php?p=3365)(scene)

Builds a new Rendering manager object
####Parameters
 | Name | Type | Description
---|---|---|---
 | scene | [Scene](page.php?p=3274) | The scene linked to this rendering manager
---

##Members

###static MAX_RENDERINGGROUPS : number


The max rendering groups

default : 4



##Methods

###render(customRenderFunction, =&gt;, activeMeshes, renderParticles, renderSprites) &rarr; void

####Parameters
 | Name | Type | Description
---|---|---|---
 | customRenderFunction | (opaqueSubMeshes: SmartArray&lt;SubMesh&gt;, transparentSubMeshes: SmartArray&lt;SubMesh&gt;, alphaTestSubMeshes: SmartArray&lt;SubMesh&gt;, beforeTransparents: () =&gt; void) | 
 | =&gt; | void | 
 | activeMeshes | [AbstractMesh](page.php?p=3269)[] | 
 | renderParticles | boolean | 
 | renderSprites | boolean | 
---

###reset() &rarr; void


###dispatch(subMesh) &rarr; void

####Parameters
 | Name | Type | Description
---|---|---|---
 | subMesh | [SubMesh](page.php?p=3339) | 
---