![Imgur](https://i.imgur.com/ebOnhmL.png) <br>

# Hyperion case for DIY SlimeVR!

The Hyperion is one of the smallest and slimmest cases to date for your DIY SlimeVR Trackers. <br>
With it's completely Tool-less design and tolerances fine tuned specifically for FDM 3D Printers.<br>
The Hyperion is both easy to print and assemble!<br>
Every part is carefully thought out and clicks together with a satisfying snap.<br>
The Hyperion offers support for various Battery sizes and types.<br>
<br>

<a href="https://imgur.com/9vDfYJD"><img src="https://i.imgur.com/9vDfYJD.gif" title="source: imgur.com" /></a> <br>
<br>

## Index
- [Components](#Components)
- [Compatibility](#Compatibility)
- [Versions](#Versions)
- [Printing](#Printing)
- [Assembly](#Assembly)
- [Links](#Links)
- [Contact](#Contact)
- [License (MIT)](#License)

## Components

For the Hyperion you will need the following components:<br>

- [TP4056](https://www.aliexpress.com/item/32649780468.html)
- [MPU6050](https://www.aliexpress.com/wholesale?SearchText=MPU6050)
- [Wemos D1 Mini](https://www.aliexpress.com/wholesale?SearchText=D1+mini)
- [SS12D00G3 (switch)](https://www.aliexpress.com/wholesale?SearchText=SS12D00G3)
- [Battery](https://docs.slimevr.dev/components-guide.html) (*804040 is what the docs suggest 503759 is smaller and usually higher capacity*)
    - [804040](https://www.aliexpress.com/item/33021202630.html)
    - [503759](https://www.aliexpress.com/item/1005003257130562.html)
- [40mm straps](https://www.aliexpress.com/item/1005002350231996.html)<br>

You can also order these parts elsewhere through sites like Amazon with a slightly higher markup, but they might arrive much faster depending on where you live.<br>

*The straps from the docs are only 25mm wide, the Hyperion is designed to fit up to 40mm straps for extra stability.*<br>
*Be aware that there are different versions of the TP4056 which are smaller and have less soldering pads, there is also a microUSB version which does not work with this case avoid these too if you're planning on using the Hyperion case.*<br>

## Compatibility

The Hyperion case offers compatibility for various battery types.<br>
For example: the 503759 supports any battery that is equal to or smaller than 5x37x59mm<br>
So if your battery is not a 503759 or 804040 but it is smaller than either one it will work!<br>
You might have to fill up the space a little bit to prevent the battery from sliding around if your battery is significantly smaller.
A good example would be a 503450, which would fit just fine.<br>

### But what about the BNO08X? <br>
Sadly as of now it is virtually impossible to get a BNO chip at a reasonable price.<br>
For that reason I'm sorry to say that this case does not ***yet*** officially support the BNO08X chips.<br>
If it does fit please let me know through Discord I'm [@Smeltie#1999](https://discord.gg/SlimeVR) on the [Official SlimeVR Discord server](https://discord.gg/SlimeVR)<br>
<br>

## Versions

As you may notice there are a lot of different .STL files included in this project.<br>
This is because the Hyperion supports multiple Battery sizes and separate AUX/extension versions of each case and lid.<br>
The names of the files indicate what the parts are for and which features they incorporate.<br>
To clarify some of the terminology:<br>
If the file name includes the following then:<br>

*- AUX*: This part has an opening for a ribbon/JST cable to an Extension.<br>
*- 503759*: This means the part is meant for batteries that are 5x37x59mm (or smaller)<br>
*- 804040*: This means the part is meant for batteries that are 8x40x40mm (or smaller)<br>
*- Slime*: This part has the SlimeVR logo on it, mostly for the lid.<br>
*- Blank*: This part has no print or logo on it, mostly for the lid.<br>


### So which parts do i need?
Of course this is totally dependent on the battery you chose.<br>
In total you will have to print at least 4 components per tracker, which are:<br>
Case, Tray, Lid and Switch.<br>


So for example, you bought a 503739 (or smaller) battery.<br>
You would need the following:<br>
*- Case_503759.stl*<br>
*- Tray_503759.stl*<br>
*- Lid_503759.stl*<br>
*The switch in this case is universal and not dependant on battery size!*
<br>


#### If you want to have a tracker that uses an AUX/Extension module beware<br>
In that case you would need the following:<br>
*- Case_503759_AUX.stl*<br>
*- Lid_503759_AUX.stl*<br>

*The tray is not dependent on the AUX/Extension feature!*


## Printing
It is heavily suggested to print these components on an FDM (Filament based) 3D printer such as the Ender 3 or similar.<br>
This is because all the tolerances have been adjusted to accommodate a wide variety of FDM printers.<br>
Personally I printed my parts on a slightly modified Ender3 V2 using E-Sun PLA+ (gray) with a stock 0.4mm nozzle.<br>

In terms of the printing itself, these parts don't need any support.<br>
Orientation wise the case, tray and switch can be printed as is.<br>
The lid you might want to turn 180 degrees so the flat side is against the bed:.<br>

![Imgur](https://i.imgur.com/Qy82Dcqm.png)

#### The Switch
As you might have guessed the switch is a little small and harder to print.<br>
However it is doable with the right settings!<br>
*- Bed Temperature* - 70c<br>
*- Initial layer speed* - 10mm/s<br>
*- Printing speed* - 20mm/s<br>
*- infill* - 0%<br>
*- layer height* - 0.08mm<br>
*- Location on the buildplate* - Close to the front or back not in the middle.<br>
*- build plate adhesion* - Brim<br>

![Imgur](https://i.imgur.com/j43d2Gm.png)<br>

*These settings worked well for me, they might not work for everyone*<br>
*Especially layer height might be challenging for some printers*<br>
*Just take your time and take it slow, I've printed more than a handfull now.*<br>
*The reason I say don't print in the middle is because on many printers that's a low spot, and this would hinder the adhesion needed to keep this little part stuck down.*<br>


## Assembly

![output](https://user-images.githubusercontent.com/38034111/148065707-96a622b4-d118-4901-adf6-c36dceab3feb.gif) <br>

Assembly is rather straight forward however there are some slight things to look out for.<br>
You might have to slightly sand the sides of the tray depending on your printers tolerances, not all printers are created equal.<br>
There should not be a need to sand anything but keep it in mind if something is just too tight.<br>
It is normal for the tray to snap into place a little bit, it's friction fit after all.<br>
I suggest soldering things out of the case and using the case/tray as a reference towards wire length, you want to keep your wires rather short like this:<br>

![Imgur](https://i.imgur.com/UCcndadm.jpg) <br>

Otherwise it might not close, there should be more than enough space for your wires in the case.<br>
So you don't have to make them extremely short just keep it manageable.<br>
<br>

#### The Switch
After printing the switch the bottom layer of the hole might be a little too tight due to elephants foot or squish.<br>
In this case you can take something like a hobby knife and slightly open that first layer up a little bit.<br>
<br>

#### The Lid
To install the lid it is best practice to install it as follows:<br>
Place the lid on the case at an angle with the back side first (vents).<br>
So that the notches align, after this lower the front and snap it shut.<br>
To remove the lid again place a fingernail or pry tool between the lid and the power switch and pry upwards, the lid should snap open.<br>

<a href="https://imgur.com/p8z1lyn"><img src="https://i.imgur.com/p8z1lyn.gif" title="source: imgur.com" /></a> <br>
<br>

#### The Strap
The strap is meant to be ran underneath the tracker, this is because otherwise the powerswitch would be obstructed.<br>



## Links
Here are some useful and fun resources:
- [The Docs (SlimeVR Documentation)](https://docs.slimevr.dev/)
- [Github Repository SlimeVR](https://github.com/SlimeVR/)
- [Github Repository Hyperion](https://github.com/Smeltie/Hyperion)
- [Thingiverse Hyperion](https://www.thingiverse.com/thing:5186756)
- [Cults3D Hyperion](https://cults3d.com/en/3d-model/gadget/hyperion-case-for-diy-slimevr)
- [CGTraders Hyperion](https://www.cgtrader.com/free-3d-print-models/hobby-diy/electronics/hyperion-case-for-diy-slimevr)
- [SmeltieVR YouTube](https://www.youtube.com/channel/UC4MEm3i0WxIGPyM8YBV9SSQ)
- [SlimeVR Discord](https://discord.gg/SlimeVR)

## Contact
If you experience any problems with your Hyperion or have any questions/suggestions?<br>
Feel free to reach out through either Discord I'm [@Smeltie#1999](https://discord.gg/SlimeVR) on the official [SlimeVR Discord server](https://discord.gg/SlimeVR).<br>
You can also shoot me an email: [SmeltieVR@gmail.com](mailto:smeltievr@gmail.com)<br>
If you want to help out with the project or have/want to make a version for a different set of hardware you're more than welcome to send it over or do a merge request!<br>

## License
This project is licensed under the MIT license.<br>
