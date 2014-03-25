---
category: documentation
layout: documentation
title: "Start Up <em>Guide</em>"
author: matthieulapeyre
sidemenu: null
published: true
---

<!-- <div id="betatest"></div>
## I. Beta _Test_ -->

<hr />
<div id="repository"></div>
## I. Repository _Access_

### Software
The source code used with Poppy can be found on a public bitbucket repository. They are available under a GPLV3 licence. The software is based on the [PyPot Library](http://www.poppy-project.org/pypot-library/). To contribute you can directly fork our repository and send us pull requests. Do not hesitate to directly contact us for any information. Any help or idea will be appreciated!

- [PyPot Repository](https://github.com/poppy-project/pypot)

### Hardware
->[![Creative Commons v3](http://i.creativecommons.org/l/by-nc-sa/3.0/88x31.png)](http://creativecommons.org/licenses/by-nc-sa/3.0/)<-

*The Poppy project* by [Inria](http://www.poppy-project.org) is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License](http://creativecommons.org/licenses/by-nc-sa/3.0/).

- [GrabCAD Repository](https://github.com/poppy-project/poppy-hardware-beta)

- [GrabCAD STL Files](https://grabcad.com/library/poppy-beta-2)


<hr />
<div id="components"></div>
## II. Component _list_
[Here](https://docs.google.com/spreadsheet/ccc?key=0Avq9MlqcWxlNdGpjY1RwbDMtSDJJSlVpM1VhRkVLVUE&amp;usp=sharing) is the list of all components needed to build a Poppy :

- [www.poppy-project.org/wp-content/uploads/data/3Dprint.csv](http://www.poppy-project.org/wp-content/uploads/data/3Dprint.csv)
- [www.tablesgenerator.com/markdown_tables](http://www.tablesgenerator.com/markdown_tables)
- [www.poppy-project.org/wp-content/uploads/data/electronics.csv](http://www.poppy-project.org/wp-content/uploads/data/electronics.csv)
- [www.poppy-project.org/wp-content/uploads/data/mounting_tools.csv](http://www.poppy-project.org/wp-content/uploads/data/mounting_tools.csv)

<hr />
<div id="known_issues"></div>
## III. Known _Issues_
### Missing _electronics_

The current open source distribution of Poppy does not include all the head electronics. The design is still a prototype and it cannot be easily reproduce and it is not really effective **so we decided to not share the electronic design it for the moment**.
The Poppy electronics architecture is the main development challenge for the public release. It is our priority and we are spending the most of our development time on it.
**In the forum, we will share our issues and questions. It is the place to help us by sharing your experience. It is also the opportunity for you to ask for new features or needs. For example if you think about other sensors or if you want extension plug, etc.**

### ~~Hip/pelvis assembly~~ Fixed by _Andreas NTALAKAS_
<div class="alert alert-success">
Description="Andreas NTALAKAS adds a new part named **_Connector HN07-N101_FR05-S101_** on GrabCAD Workbench. This part is now included in the BOM list and should be 3D printed.
</div>
To connect the pelvis to the thigh, you will have to assemble FR05-S101 on MX-64 with HN07-N101 horn on MX-28. The problem is that the holes between FR05-S101 and HN07-N101 do not match.
On our Poppy we made the missing holes with a drill and it works fine. If you have access to a drill, you could use a 2mm drill-bit.

### Motors _weakness_
The Robotis Dynamixel motors are expensive but they are still easily breakable :/
They can easily melt if they have to support high torque for long time. Currently, there is no security in the PyPot code to avoid breaking. So if you do not want to change a motor every time you use Poppy, please reduce the [maximum torque](http://pierrerouanet.bitbucket.org/pypot/pypot.dynamixel.html#pypot.dynamixel.motor.DxlMotor.torque_limit) output to 70%.
By using these precautions we have only broken, on average, one engine per year.

<hr />

<div id="repository"></div>

## IV. Advices
Last but not least, we encourage you to use in prior the wiki portal:

- [http://poppy-project.github.io/wiki2](http://poppy-project.github.io/wiki2)

Ask and answer question on the forum:

- [https://forum.poppy-project.org/](https://forum.poppy-project.org/)

Grab the code on the github (hardware and software oriented): 

- [https://github.com/poppy-project/](https://github.com/poppy-project/)