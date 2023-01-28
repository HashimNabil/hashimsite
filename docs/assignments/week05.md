# 5. Electronics production

## 0.2 mm Tool Diameter **Amal Ashoor**

The goal of this week assignment is to describe the design rules using the Roland SRM-20 CNC machine CNC machine. To start the fabrication process, I downloaded the interior and the traces in PNG format from this [website](http://academy.cba.mit.edu/classes/electronics_production/index.html).
![](../images/amal/g1.jpg)
To change the PNG images to Ronald mill (.rml), I mainly used this [website](https://mods.cba.mit.edu/). I started by right-click then I selected "Program", "Open server program", and "Roland mill SRM-20 PCB png".
![](../images/amal/g2.jpg)
After that, I selected the traces png file and changed the tool diameter to 0.2 mm which equals , which equals 0.00787401 inches.
![](../images/amal/g3.jpg)
 I changed the origin of the machine to zero on all axis. To save the output file, I right-clicked on the page and selected "Modules" and "Open server module" and "file save". Then, I connected the input and output as shown below.
![](../images/amal/g4.jpg)
Moving to the mill raster 2D, I changed the tool diameter to 0.2 mm and the direction to climb. Then, I pressed on calculate and saved the (.rml) file. I repeated this step in the conventional direction. Then, I changed the png file to the interior and repeated this step in the two directions.
![](../images/amal/g5.jpg)
 I changed the milling bit of the machine to 1/64 milling bit and selected the origin point. Then, I cut the climb files first then the conventional files. The results are shown below (top is the climb direction). According to the following image, the climb direction milling is clearer compared to the other one.
![](../images/amal/g6.jpg)


<<<<<<< HEAD
=======

>>>>>>> 4255d2635aa16b1cb2a9e0e8819f10f8b977a776
## **Yousef Jalil **

 For the Group assignment we had to test the capabilities of the Machine (Roland SRM-20) to mill extra fine details. also through different milling directions (Climb and Conventional) 
                
 I downloaded the traces provided to test the machines from [Here](http://academy.cba.mit.edu/classes/electronics_production/index.html).
                
 Linetest traces
 ![](../images/Yousef/Electronic_production/linetest.png)
 Outline 
 
 ![](../images/Yousef/Electronic_production/linetest.interior.png)
 
 Then Proceded with Mods to set up the cutting files
 I went to [Mods](https://mods.cba.mit.edu/),Click Right click to pull up the interface then go to Programs 
 
 ![](../images/Yousef/Electronic_production/mods_prog.JPG)
 
 Then ---> Open Local Server 
 

 ![](../images/Yousef/Electronic_production/mods_server.JPG)
 
 Choose ---> Roland SRM-20 --> PCB PNG  
 
 ![](../images/Yousef/Electronic_production/mods_server.JPG)
 
 After that you will see a set of nodes 
 
 ![](../images/Yousef/Electronic_production/mods_nodes.JPG)
 
 what we are going to use is on the left side, click on select PNG and pick the linetest 
 
 ![](../images/Yousef/Electronic_production/mods_process.JPG)
 
 Make sure to change the tool diameter to the one you are going to use in this case 1/64"  
 
 ![](../images/Yousef/Electronic_production/mods_0.1mm..JPG)
 
 Make sure to set the machine coordinates x,y,z  to Zero (origin)  
 
 ![](../images/Yousef/Electronic_production/mods_origin.JPG)
 
 Then to save your file open the menu by clicking right click again and choose ---> Programs 
 
 ![](../images/Yousef/Electronic_production/mods_programms.JPG)
 
 Then --> Open server program
 
 ![](../images/Yousef/Electronic_production/mods_server_programm.JPG)
 
 --> Modules
 
 ![](../images/Yousef/Electronic_production/mods_modules.JPG)
 
 Then --> Open server module
 
 ![](../images/Yousef/Electronic_production/mods_server_module.JPG)
 
 Then --> File --> Save
 
 ![](../images/Yousef/Electronic_production/mods_file_save.JPG)
 
 And you will get this Node
 
 ![](../images/Yousef/Electronic_production/mods_file_module.JPG)
 
 And lAST connect the nodes together
 ![](../images/Yousef/Electronic_production/mods_connect_nodes.JPG)
 
 After checking everything is ok click we will do the the calculation twice, one for the Climb direction and one for the Conventional direction.
 
 ![](../images/Yousef/Electronic_production/mods_calculate.JPG)
 
 <h3> Results </h3>
 
 <h4>          Climb  </h4>
 
 ![](../images/Yousef/Electronic_production/Climb.jpg)
 
 <h4>          Conventional  </h4>
 
 ![](../images/Yousef/Electronic_production/Conventional.jpg)

                
    
