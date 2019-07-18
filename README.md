# A1200KB Amiga 1200 mechanical keyboard

This PCB design was reverse-engineered from the original keyboard in an Amiga 1200. It is designed to connect to your Amiga 1200 with no modifications to the original machine, just take out the original keyboard and store it away safely. I don't know much about the keyboard interface for other Amigas but everything I read tells me this will only work on an Amiga 1200.

![PCB](https://github.com/aeberbach/A1200KB/blob/master/images/rev2-pcb.jpg)

## Requirements
To make a working keyboard for your Amiga 1200, you need:

- one PCB (this project)
- MX-compatible PCB-mount keyswitches, one for each key
- one LED (caps lock)
- one FFC connector, 32-way RA 1.25mm pitch. Molex 52044-3245 is one example, available from Mouser Electronics.
- one FFC ribbon cable, 32-way, 1.25mm pitch. Molex 15168-0400 is one example, available from Mouser Electronics.
- keycaps
- some way to mount the keyboard inside the Amiga.

## Design
The Amiga 1200 keyboard is a simple passive key matrix connected via a 31-conductor cable. Some special keys are not on the matrix but have a dedicated circuit, such as the CTRL and Amiga keys - this is why so many conductors are necessary. The original Amiga 1200 PCB uses a 31-way FFC connector, I was not able to buy this anywhere as they are long discontinued. However cutting one conductor away from the cable allows it to fit in the Amiga connector with 31 conductors and to the keyboard with 32 conductors and everything is fine. The specified FFC cable is slightly longer than required but in 2019 there is not  a lot of choice available, so the longer one will do. 
I had my boards made with 2mm PCB substrate, no other special options. Using a thick substrate makes it reasonably sturdy but attaching a piece of aluminium right angle to the top of the PCB is a requirement to make it as stiff as a keyboard should be.  
 
![Complete](https://github.com/aeberbach/A1200KB/blob/master/images/case-closed.jpg)

### Amiga Keycaps
These aren't available. I'm making some using a blank set of keycaps from aliexpress and a laser etcher, but I do not know of anywhere that sells a MX-stem set of Amiga keycaps. The space bar on this PCB has a dual-footprint space bar. I am using a 7U space bar for which there are also stabilizer mounts provided. If I ever find a 9U, for which there are also stabilizer mounts provided (nobody seems to make these) I will switch, but the two empty spaces don't bother me.

## Construction
Without going into all the detail here - as there is lots of detail on www.grayunicorn.com - I rate this a mid-level project. There is no power, no delicate soldering, and nothing can really be inserted the wrong way. Mounting the keyboard requires 3D printing the files you will find in the 3Dfiles folder - 13 of the cover pieces, both side pieces, both bottom pieces, M3 nuts and bolts, and a length of 10x3mm aluminium extrusion. I'm a 3D design amateur so if you make a better design please share.

You can damage your Amiga if you don't know what you are doing. Please be careful and if you are not experienced in projects like this get some help, vist your local makerspace or somthing, and don't hurt yourself or your computer.

## Share
Most of all - if you have any suggestions for improvements, adding an issue or a pull request to this repo would be much appreciated. And share your project with the Amiga community, I'd really like to see what you made.

#### Donate?

I hate to think what this has cost so far. It's been fun and I'd do it again, but if you'd like to help the next project happen that would be awesome.

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.me/grayunicorn)
