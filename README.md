# `plod-parser`

A Scala library for parsing data from Pompeii LOD project

Data sets (TTL format): in `data` directory, file names appended with download date.

## Notes reverse-engineering data structures

Current TTL has 1272 entries of four spatially hierarchical types:

-  `p-lod:city` (1)
-  `p-lod:region` (9)
-  `p-lod:insula` (112)
-  `p-lod:property` (1150)


Properties for each type:


`p-lod:region`, `p-lod:insula` and `p-lod:property` all have properties:

-  p-lod-vocab:p-in-p-url (URL)
-  p-lod-vocab:spatially-within (URI)

In addition, `p-lod:property`  has

-  p-lod-vocab:arcgis-id (String)
-  p-lod-vocab:area (Float)
