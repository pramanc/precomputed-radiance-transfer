# precomputed-radiance-transfer
undergraduate student course project in Zhejiang University

The diffuse and glossy materials are supported.

how to use it :
prt -l xxxx.jpg output.txt bandnumber samplenumber(4096)
prt -o -d 1 xxxx.obj output.txt bandnumber samplenumber
prt -o -g 1 xxxx.obj output.txt bandnumber samplenumber

-l: means lighting, -o: object type(material of glossy)

