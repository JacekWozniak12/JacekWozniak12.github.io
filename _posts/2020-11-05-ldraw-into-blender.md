---
layout: post
title: Importing from BrickLink Studio into Blender 2.81
categories: [Blender, Graphics]
imageLink: "/assets/images/posts/ldraw-into-blender/00-main.PNG"
---
How to quickly move your Lego creation into 3D software.

### Prerequisites
1. [Blender](https://www.blender.org/download/releases/)
2. [BrickLink Studio](https://www.bricklink.com/v3/studio/download.page)
3. [TobyLobster's ImportLDraw](https://github.com/TobyLobster/ImportLDraw)

### What we are going to do
Import model file from BrickLink Studio to Blender
![main](/assets/images/posts/ldraw-into-blender/00-main.PNG)

### Instalation
1. Install Blender and BrickLink Studio using provided links. Keep directory of BrickLink Studio, it will be needed later.
2. Download ZIP file of ImportLDraw from github page.
3. Open Blender. Select Edit > Preferences. 

![preferences](/assets/images/posts/ldraw-into-blender/01-preferences.PNG)

4. Find ZIP file using Blender directory manager.
5. Install addon and then apply it in preferences. Use find option to make it quicker ("Import LDraw").

![import-and-apply](/assets/images/posts/ldraw-into-blender/02-import-and-apply.PNG)

6. Save preferences if you wish to have it as default.

![save-preferences](/assets/images/posts/ldraw-into-blender/02-save-preferences.PNG)

### Pipeline
1. Create or open model in BrickLink Studio that you wish to import to Blender.
2. Select 'Export as Ldraw'.

![export-as-ldraw](/assets/images/posts/ldraw-into-blender/03-export-as-ldraw.PNG)

3. Open Blender. Select Import > LDraw

![import](/assets/images/posts/ldraw-into-blender/04-import.PNG)

4. Supply directory path of BrickLink Studio/LDraw folder to *LDraw Filepath* - that way, you can be sure that BrickLink Studio and importer are using same files to render creations.

![library](/assets/images/posts/ldraw-into-blender/05-library.PNG)

5. Select file to import and change import options as you wish.

![file-import](/assets/images/posts/ldraw-into-blender/06-file-import.PNG)

6. It may take a while, so be patient.
7. Now you may render it or modify it via Blender tools.

<br>
### Legal
All rights belongs to respective owners, including: LEGO, Blender Fundation, TobyLobster and Estate of James Jessiman. This manual is not developed or endorsed by any of those mentioned before.
