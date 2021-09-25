# Ubuntu-3d-printing

**Introduction**

This is a friendly devops and administration guide for 3D printing in Ubuntu 20.04. It presents a "blue collar manufacturing solution" for the rest of us using free software and 10 year old PC hardware. Printers are relatively cheap nowadays. You can do this whole setup at home for well under $1,000 in hardware including the cost of a good printer. The software side of things is free and easy to use with top notch results and usability. The excellent quality of what is available is why this guide was written. Investing in yourself is always wise. Considering the pandemic in 2021 and resulting system changes in manufacturing, studying this environment is a healthy use of time and resources with very little cash outlay.

Ubuntu 18 was prone to crashing and errors that made the user experience for this highly unpredictable. That major issue has been largely remedied AND deserves a healthy spotlight for development and support.

The goal of this guide is to support people who wish to 3D print applicable and low cost industrial solutions like:

1. parts
2. tooling
3. bracketry
4. adapters

This guide is NOT for 3D printing artistry. It is for "applicable, real world solutions in a free environment." That situation has not been reliable and easy to use until now. This is an attempt to open source some aspects of Industry 4.0 so you can practice at home or grow your small/medium enterprise or project. The depth and extensibility of this simple setup shrinks an entire shop to a desk sized workstation. You can have a super-concentrated toolset without all the floor space, rent, debt, waste, noise, or maintenance costs. The reduction and concentration of resources is another strength of this user environment.

This is a user-friendly means to 3D printing locally in Ubuntu 20.04. If you desire to protect your work and NOT be reliant on a 3rd party cloud provider, then this is a good guide for you. Some cloud providers require you to hand over rights to your designs in exchange for using their services. That clashes with the needs of a business to protect their IP. This simple toolchain respects your privacy. You don't need to be on the internet to use it, nor are you forced to compromise the integrity of your work. There are also numerous add-ons available. You can create a "chain-mail armor" solution, custom tailored to you or your shop's needs for free. That solution can be robust, reliable, and easy to use. 

Resources here are open source and readily available to download and install. This is a very small toolset that plays nicely on the Ubuntu 20.04 desktop. You can add to it as much as you like or as necessary. Having explored this setup for over a year, it is time to unveil the stability, robust quality control, and ease of use for average users. Industry 4.0 need not be a scary thing or overhyped buzzword. You can learn how to weild it at home in your spare time. This is a "blue collar solution" for the rest of us. It offers a pleasant user experience on older hardware that does not require a lot of resources. You don't need a PhD, an engineering degree, or security clearance to to this. If you are a decent technician or gneral Ubuntu Linux user looking to update your skills for a changing production environment, then this is a healthy way to do that.

A heartfelt "thank you" is extended to those developers who have toiled day and night to make this reality available to the rest of us. This guide is a nod to their extensive efforts. I'm not the best coder or developer, but I do know how to make quality documentation and support people's efforts. This repo is for UBUNTU linux users. RedHat, CentOS, etc---I'm just one person and have not explored that end of things. The robust usability and stability of this environment is why I have chosen to support it and educate people.


**Basics**

What this combination of software is called is a "toolchain" in industry terms. Instead of a single suite of tools in one interface, you have a short "chainlink" of tools that play nicely together. These tools function separately. The goal here is to output a file for your 3D printer in what is called "g-code". A g-code file is what the printer uses to create the desired design. 

The short chain described here allows you three main advantages present in more expensive suites:

1. Easy and local 3D design IN UBUNTU LINUX. Face it, Linux distors have not been very easy or reliable to design tooling in. Those who have not dabbled in this don't know the pain they are being spared to get to this point. The stability and ease of use have not been user friendly until right about now in late 2021. There is a much easier learning curve compared to the past. You get to see the quality of your own work and studies in a short time.

2. Extensive control of machine settings. This is the real power. There are extensive settings and controls available to dial in the quality of your prints. You are not forced to use them all at once and you can grow with these capabilities at your own pace.

3.--It's FREE! 


**Software** 

You do NOT need to know how to write code OR use the Linux command line for these two programs. That is an option for more advanced users at their leisure.

There are two key programs in Ubuntu Linux that enable all of these robust quality control capabilities. These capabilities will be expanded upon in further user guides.

1. **MatterControl 2.0 Beta**. Free to use. This is easy to use 3D design software that lets you design your solutions in a stable environment. Support from them requires a Pro upgrade if desired. This software is an excellent means to make a precise design NOT an artistic design. You work with generic shapes and can set the measurements for those shapes. The end result when printed is very close or exactly to your design specs. 

This program generates what is called an .STL file. An .STL file is an industry standard file for 3D objects and NOT 3D graphics. That is a big difference worth knowing. You are simply concerned with combining shapes and setting measurements in a drag and drop format on screen. This would be equivalent to the "CAD" solution to design an object. Some online resources offer the same functionality in a browser, but the trade off is no local control or privacy. 

Download MatterControl for Linux here: https://www.matterhackers.com/store/l/mattercontrol/sk/MKZGTDW6

2. **Cura Slicer v4.11**. Free to use. This program packs a real punch for quality control of your prints. The purpose of this program modifies your .STL file created upstream in MatterControl. It outputs a g-code file that the 3D printer uses to make your design into a real object. The major advantage with this software is the nearly 1,000 different granular settings available WHEN NEEDED. You can start off as a beginner. As you progress, you learn to use the custom settings. The power of the custom settings allows you to dial in the quality of your print. You can control quality down to the size of 60 microns. BUT, that level of quality control involves some further tweaking of the printer to bring them to life. This is equivalent to the "CAM" solution that makes instructions for the machine to follow.

Download Cura slicer for Linux here: https://ultimaker.com/software/ultimaker-cura

These two programs have so much control and usabilty available that you will spend the better part of a couple of months learning all of those bells and whistles. Fear not. Just diving in to learn is pretty easy. You could spend a nice Saturday setting all this up from scratch and never touch the command line or write a single line of code.

**Other design software options**

There are certainly other software options available to support your tooling and design needs. These are all the other suites that we explored with Ubuntu 18 and 20. The two listed above have proven to be the most stable AND easy to use in Ubuntu 20.04. That is their main advantages. Their other advantage is the depth of quality control over the final product. That being said, what other stuff is available and why would you use it?

1. FreeCAD. This software is pretty robust. You can build your object line by line if desired, like other CAD solutions. It isn't quite as fast or stable as expensive suites, but that's the trade-off for free software. It is a fantastic free option for people looking to get into the CAD profession or just tinker with it and learn something new. You learn how to make objects from scratch.

https://www.freecadweb.org/

2. Wings3D. I do not mean to disparage this work. It's my least favorite option because it wasn't very stable in this environment.

http://www.wings3d.com/

3. Blender. This program is a BEAR to learn as a newbie. It is made FOR graphics professionals BY graphics professionals. It is very good at drawing a design by artistic means. If you desire to make custom graphics for figurines and artwork, then it is a good option. This is part of the important distinction between CAD and computer graphics. This is a graphics program first for games, animation, etc. They have add-ons for 3D printing BUT this was an afterthought at best. Blender is a very good graphics design program first and it always will be, just like AutoCAD will always be really good design software. Both are very in-depth tools that have a steep learning curve.

https://www.blender.org/download/

4. OpenSCAD. This is a decent option for 3D design. You have to design everything line by line or with a basic shape. The graphical interface feels a little unweildy. But, it's largely stable. I've based this guide onstability and ease of use. This option is good, but not really for beginners or those picking it up cold without prior CAD experience. FreeCAD can be the same way. It's hard to know where to intuitively start or end. I'm not entirely sure how well protected it is from phishing and hacking. My browser does throw warnings on the main site, so here's a Wiki link.

https://en.wikipedia.org/wiki/OpenSCAD

5. BRL-CAD. This is an honorable mention for being the oldest and open source CAD software that has been continually maintained. This is the US Army's version of CAD software. It was stable in our testing. However, it was no less unweildy compared to FreeCAD. I would definitely recommend this for students studying CAD. It's still a software that requires you to build line segment by line segment. I just prefer MatterControl because it's faster to use than of all of these.

https://brlcad.org/

6. LuaRocks. This suite has a lot potential and support. It is popular in South America, academia, and even with the Catholic Church. A lot of the documentation is written in Spanish and Portuguese. The software itself was relatively stable, but again requiring you to work line by line. It offers a lot of the minute control mentioned earlier.

https://luarocks.org/

**Growth from here**

It took a lot of patience to get to this point. I admit to not being the fastest or most experienced at computer code, and having stuck to administration as a means to an end. I code when necessary but don't have the time to fix the bugs that were endemic to this setup until now. If you are interested, all of these options are open source and waiting for help but you need a healthy amount of coding experience and focus to be useful to those ends. As a user, you can just concentrate on making stuff with MatterControl and Cura.

The extensibility of this setup is also worthy of mention. There is a lot of minute control over quality of the final product with just MatterControl and Cura. Everything else is still available for you to use. I found no dead-ends in the last year of studying these options. There were no peaks and valleys or tradeoffs of usabilty and speed. You can go straight through with both with little effort. 

Computer languages to study with are Python, C, C++, and SQL. G-code is the other. The solutions mentioned in the beginning here allow an "infrastructure as code" approach that just depend on minimal administration skills to set up.

For small electronics, Arduino and Raspberry Pi play a role in the functionality presented here. I use an Octopi for control of my Anycubic printer which uses an Arduino for its brain. If you wish to use a Pi based 3D printer then that is up to you. The beginning of this guide is focused on making a stable and usable desktop interface. You can customize software, hardware, firmware, monitoring, sensors, etc. All of these present more options waiting to be used.

**Background**

The information and subject matter in this guide was studied for a bit over a year. I've been a Linux user for 5 years starting in Ubuntu 16.04. I have been a crack developer and hack for 2 years with Python and C++. Embedded systems and devices have been a concentration for 10+ years inlcuding electronic fuel injection, X-ray scanners, medical devices, robotics and IOT devices. I am studying for an LPIC1 certification from the Linux Professional Institute, aiming to use my time and resources wisely during the pandemic, while probably working too much over time testing embedded devices and systems. To support this series of documentation, I have built an at-home Linux network with some older hardware. Actual experience is needed for modern certifications, and I was looking to make unique use of these general Linux administration tools. Coupled with a business degree and programming certification, I started down the road of embedded Linux for devices and instrumentation. Those skills were applicable in other areas that I brought together to support these ends. DevOps for 3D printing in Lionux is currently a very specialized subject matter. It is poised to be standard for open source manufacturing in the Industry 4.0 era. I hope to support the growth of this endeavour for end users, small/medium entreprises, and project management needs.
