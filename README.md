# NBU-SOID
-----------COPYRIGHT NOTICE STARTS WITH THIS LINE------------
Copyright (c) 2019 The Ningbo University
All rights reserved.

Permission is hereby granted, without written agreement and without
license or royalty fees, to use, copy, modify, and distribute this
database (the images, the results and the source files) and its 
documentation for any purpose, provided that the copyright 
notice in its entirity appear in all copies of this 
database, and the original source of this database,  
Multi-media Signal Processing Laboratory at the Ningbo University,
is acknowledged in any publication that reports research using this database.
The database is to be cited in the bibliography as:

Y. Qi, G. Jiang, M. Yu, Y. Zhang, and Y.-S. Ho,"Viewport Perception based Blind Stereoscopic Omnidirectional Image Quality Assessment",
 IEEE Transactions on Circuits and Systems for Video Technology, in review.
 
You can change this program as you like and use it anywhere, but please refer to its original source (cite our paper and our web page at https://pan.baidu.com/s/1UKjtZ6XRJ46AF9Hf7vQpOw, and the corresponding password for database extraction is "yr64").

-----------COPYRIGHT NOTICE ENDS WITH THIS LINE------------
Please contact Yubin Qi (qiyubin123@126.com), Gangyi Jiang (jgyvciplab@126.com) if you have any questions.
This investigators on this research were:
Mei Yu (yumei2@126.com) -- Faculty of Information Science and Engineering at Ningbo University
Yun Zhang (yun.zhang@siat.ac.cn) -- Shenzhen Institutes of Advanced Technology at Chinese Academy of Sciences
Yo-Sung Ho (hoyo@gist.ac.kr) -- School of Electrical Engineering and Computer Science at Gwangju Institute of Science and Technology

--------------------------Descriptions of NBU-SOID Database-----------------------------------------------

12 high-quality source image sequences with resolution of 2560x2560 and 4096x4096 are selected to 
cover diverse image content including natural sceneries, indoor and outdoor views, and man-made architectures. 

The origins of the sequences are specified in the above paper. 

Description:
Explanation of image name in the NBU-SOID database:'id(scene)_id(distortion type)_id(distortion level of left and right view).' 
The id(scene) is from [01,02,...,12], id(distortion type) is from [1,2,3], and id(distortion level) is from [1,2,3,4,5].
where the definition of id(distortion type) and id(distortion level) is expressed as follows
distortion type: 1, 2, and 3 denote the JPEG, JPEG2000 and HEVC distortion, repectively.
distortion level: The control parameters in JPEG, JPEG2000, and HEVC are q, bpp, and QP, repectively.
JPEG(levels)  left(q)   right(q)   JPEG2000(levels)   left(bpp)  right(bpp)      HEVC    left(QP)   right(QP)
  11            10        10            11               0.05       0.05          11        22         22
  22            30        30            22               0.10       0.10          22        27         27
  33            50        50            33               0.30       0.30          33        32         32
  44            70        70            44               0.60       0.60          44        37         37
  55            90        90            55               1.00       1.00          55        42         42
  13            10        50            13               0.05       0.30          12        22         27
  15            10        90            15               0.05       1.00          13        22         32
  23            30        50            23               0.10       0.30          15        22         42
  24            30        70            24               0.10       0.60          24        27         37
  35            50        90            35               0.30       1.00          34        32         37
  45            70        90            45               0.60       1.00          35        32         42
e.g.,'01_1_11.png'in the "dis" folder, and 
'id(scene).png' in the "ref" folder represents the reference images.

The mean opinion scores (DMOS) of distorted images range from 1 to 5, where 1 
denotes the worst quality and 5 the best. 
------------------------------------------------------------------------------------------------------
ref folder: includes 12 source reference images;
			       
dis folder: contains 396 distorted images with three kinds of distortion types organized in imgname.mat;

MOS.mat:  contains DMOSs of 396 distorted images organized according to imgname.mat;

imgname.mat : summarizes the image names in the dis images folder.

------------------------------------------------------------------------------------------------

Please refer to the above papers for more details.
