# **Journal-3**

## *06/07/26 20:00 - 22:00*

## *07/07/26 10:00 - 16:00*



## **CAD/PCB Redesign**



#### **CAD**



I know the guide uses onshape but I personally think **fusion 360** is so much nicer to work with, so that's what I'll be using.

I started by exporting my pcb as a `.step` and then setting up my cad workspace.



I imported the `the-clanker-pcb.step` and outlined how I want the case to look with a 4mm gap from the pcb all over.



once the case was made I uploaded a .step of cherry mx keycaps and place every single one, all 68...
and then I raised the pcb into position in the case.



#### **Next Day (PCB)**



I ended up remaking the whole case in a new document as the last one was just too messy for my liking.

I also slightly fixed the positioning of some keys, for example caps lock was 1mm off so I fixed that.

I actually decided to redo the whole pcb because I could do I lot better and the current look is kinda... pathetic.

so I started by going to `https://www.keyboard-layout-editor.com` and design the keyboard and following that design into the pcb.

Id say this went a lot quicker because I had the design right Infront of me and I already understood what to do by this point.



Eventually I had the new design laid out and start to route everything.

This took for ever because, some how the keys were in wrong places like sw68 being where sw15 should be, and that took a while along with fixing all the diodes too.



At least the routing was quick and **much** tidier than before.

Once I had everything for the pcb done I ran a quick *(it took 4 mins)* DRC, there were over 250 errors but most were just clearance so actually only 2 errors about thermal, and then 58 about led grounds not connected to ground fill.

I added vias on the gnds of the leds and ran drc again...
only 1 error and its thermal but i cant do anything about it so its fine.





##### **Tomorrow**

* ##### 3d models on pcb *(est. 1-2hrs)*
* ##### CAD *(est. 3hrs)*

