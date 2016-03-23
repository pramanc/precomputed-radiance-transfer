# precomputed-radiance-transfer
undergraduate student course project in Zhejiang University

The diffuse and glossy materials are supported.
Sorry I don't have time to clean the code.

how to use it :

prt -l xxxx.jpg output.txt bandnumber samplenumber(4096)

prt -o -d 1 xxxx.obj output.txt bandnumber samplenumber

prt -o -g 1 xxxx.obj output.txt bandnumber samplenumber

-l: means lighting, -o: object type(material of glossy)

dependency: opengl,AnttweakBar,glm,Eigen,Cimg

Code from the website:

1.  The part to load a HDR image:HDRLoader.cpp, HDRLoader.h
http://svn.openscenegraph.org/osg/OpenSceneGraph/branches/OpenSceneGraph-2.6/src/osgPlugins/hdr/hdrloader.cpp

2.  The code of rotation of Spherical Harmonics is copied from Paul Debevec’ s project.
http://www.paulsprojects.net/opengl/sh/sh.html

3.  Create shader route: ShaderFunc.cpp,ShaderFunc.h
Two functions:
char* file_read(string filename)
GLuint create_shader(string filename, GLenum type)
http://en.wikibooks.org/wiki/GLSL_Programming/GLUT

result:

diffuse:

![alt tag](https://raw.githubusercontent.com/pramanc/precomputed-radiance-transfer/master/res1.png)

glossy:

![alt tag](https://raw.githubusercontent.com/pramanc/precomputed-radiance-transfer/master/res2.png)

performance:

![alt tag](https://raw.githubusercontent.com/pramanc/precomputed-radiance-transfer/master/res3.png)

Any problem, contact 568351074@qq.com




