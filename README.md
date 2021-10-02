# Ubuntu-3d-printing

**Introduction**

This is a friendly devops and administration guide for 3D printing in Ubuntu 20.04. The real power here is inherent efficiency, creating a free CAD/CAM environment for desktop computers.

The two 3D printing suites supported in this documentation are MatterControl and Cura. Both work in other operating systems and are open source. The goal of this documentation is to apply their uses in Ubuntu 20.04 Linux. This is an interface like any other comsumer PC, with extensive control over quality at your fingertips. 

4 main talking points:

1. Ubuntu 20.04
2. MatterControl v 2.0 Beta
3. Cura v4.11
4. Quality Control

The infrastructure blueprints here presents a "blue collar manufacturing solution" for the rest of us. You don't need a degree, but some technical aptitude is very helpful. 

The test case presented here uses:

1. Free software, mentioned above. 
2. An affordable 3D printer (Anycubic Mega X)
3. 10 year old PC hardware

3D printers are relatively cheap nowadays. You can invest in yourself and develop new skills for well under $1,000. That includes PC hardware and a decent printer. The software side of things is free and fairly easy to use with top notch results and usability. Old bugs and usability problems have largely been addressed. You can use these tools in a normal user interface on a normal personal computer. No knowledge of Linux or coding is required. Although, that knowledge and use is very handy as your skills advance. The excellent quality control available is why this guide was written. Investing in yourself is always wise. This documentation was written to help those trying to help themselves, but not quite sure where to start or how to get there. Some users are brand new while others have existing skillsets in related areas. Considering the pandemic in 2021 and resulting system changes in manufacturing, studying this open source environment is a healthy use of time and resources with very little cash outlay. The skills will be applicable in the Industry 4.0 paradigm as it grows over the next 5 years. Not all employers are seeking this skillset together at once. It has not been a stable or strong base to build upon until just now.

The goal of this guide is to support people who wish to 3D print applicable and low-cost industrial solutions like:

1. small plastic parts
2. tooling
3. custom bracketry
4. custom adapters

This guide is NOT for 3D printing artistry. It is for "applicable design solutions" in a free and easy-to-use environment. The comfort and reliability is what is new. This has also not been relatively private and secure for the home user. You can keep your designs private and local. You can practice at home or grow your small/medium enterprise or project. The depth and extensibility of this simple setup can shrink an entire shop to a desk sized workstation. You can have a super-concentrated toolset without all the floor space, rent, debt, waste, noise, or maintenance costs. The reduction and concentration of resources is another strength of this user environment. 

If you desire to protect your work and NOT be reliant on a 3rd party cloud provider, then this can be a good guide for you. Some cloud providers require you to hand over rights to your designs in exchange for using their "free" services. That requirement actually presents an "ultimate cost" to the user in the long term. That requirement clashes with the needs to protect IP and customer information. Use of MatterControl and Cura on your own computer presents a simple toolchain that respects your privacy on a local machine. You don't need to be on the internet to use it, nor are you forced to compromise the integrity of your work. There are also numerous add-ons available. You can create a "chain-mail armor" solution, custom tailored to you or your shop's needs for free. That solution can be robust, reliable, and easy to use. Most of what is here is geared towards use of Ubuntu Linux, but you aren't restricted to that. 

Having explored this setup for over a year, it is time to unveil the stability, robust quality control, and ease of use for average users. Industry 4.0 need not be a scary thing or overhyped buzzword. You can learn how to weild it at home in your spare time. This is a "blue collar solution" for the rest of us. It offers a pleasant user experience on older hardware that does not require a lot of resources. You don't need a PhD, an engineering degree, or security clearance to to this. If you are a decent technician or gneral Ubuntu Linux user looking to update your skills for a changing production environment, then this is a healthy way to do that. 

A heartfelt "thank you" is extended to those developers who have toiled day and night to make this reality available to the rest of us. This guide is a nod to their extensive efforts. I'm not the best coder or developer, but I do know how to make quality documentation and support people's efforts. This repo is for UBUNTU linux users. RedHat, CentOS, etc---I'm just one person and have not explored that end of things. The robust usability and stability of this environment is why I have chosen to support it and educate people.


**Basics**

What this combination of software is called is a "toolchain" in industry terms. Instead of a single suite of tools in one interface, you have a short "chainlink" of tools that play nicely together. These tools function separately. 

1. The first tool in the chain creates a design or drawing file in MatterControl. You can work with basic shapes, addition, and subtraction. The measurements are easy to specify. The printed results are often within a tenth of a millimeter of specified measurements. There is no need for complex wireframes like common CAD solutions. This software functions like easy-to-use online CAD design tools, but it respects your privacy and is stable. 

2. The second tool is Cura. This creates a file for the 3D printer. The file for your 3D printer is made of "g-code". A g-code file is what the printer uses to create the desired design for the physical world. This software allows you to control the instructions given to the 3D printer VERY extensively. In here is where the extensive control of print quality is set in the software.

3. After making a design and setting quality parameters, the user is left with similar responsibilities of common craftsmanship. A good eye, good hand, and healthy patience makes the difference in the finished product. You can mind temperature, speed, and equipment maintenance like you might be used to from your day job. Knowing the depth of the tools involved is always good.


The short chain described here allows you three main advantages present in more expensive suites:

1. Easy and local 3D design IN UBUNTU LINUX. Face it, Linux distros have not been very easy or reliable for 3D design. Those who have not dabbled in this don't know the pain they are being spared to get to this point. The stability and ease of use have not been user friendly until right about now in late 2021. There is a much easier learning curve compared to the past. You get to see the quality of your own work and studies in a short time. 

2. Extensive control of machine settings. This is the real power. There are extensive settings and controls available to dial in the final qualities of your prints. You are not forced to use them all at once and you can grow with these capabilities at your own pace.

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

2. Wings3D. I do not mean to disparage this work. It's my least favorite option because it wasn't very stable in this environment. It hasn't been maintained recently by a large population of users or a paid staff to our knowledge.

http://www.wings3d.com/

3. Blender. This program is a BEAR to learn as a newbie. It is made FOR graphics professionals BY graphics professionals. It is very good at drawing a graphic design by artistic means. If you desire to make custom graphics for figurines and artwork, then it is an incredibly good option. There is also an important distinction between CAD design and computer graphics. This is a graphics program first for games, animation, etc. You will need to know how to work with wire meshes. They have add-ons for 3D printing BUT this was an afterthought at best. Blender is a very good graphics design program first and it always will be, just like AutoCAD will always be really good design software. Both are very in-depth tools that have a steep learning curve. The most important thing to remember when working with wire meshes is the word "MANIFOLD." This means to "make water-tight". Your final drawing has to be completely sealed. Getting there in Blender can be stressful on the eyes. If gotten wrong, you will get holes and artifacts in your print. If gotten right, then you will be rewarded with near infinite control of the smallest of design details. 

https://www.blender.org/download/

4. OpenSCAD. This is a decent option for 3D design. You have to design everything line by line or with a basic shape. The graphical interface feels a little unweildy. But, it's largely stable. I've based this guide on stability and ease of use. This option is good, but not really for beginners or those picking it up cold without prior CAD experience. FreeCAD can be the same way. It's hard to know where to intuitively start or end. I'm not entirely sure how well protected it is from phishing and hacking. My browser does throw warnings on the main site, so here's a Wiki link.

https://en.wikipedia.org/wiki/OpenSCAD

5. BRL-CAD. This is an honorable mention for being the oldest and open source CAD software that has been continually maintained. This is the US Army's version of CAD software. It was stable in our testing in Ubuntu. However, it was no less unweildy compared to FreeCAD. I would definitely recommend this for students studying CAD. It's still a software that requires you to build line segment by line segment. I just prefer MatterControl because it's faster to use than of all of these.

https://brlcad.org/

6. LuaRocks. This suite has a lot of potential and good support. It is popular in South America, academia, and even with the Catholic Church. A lot of the documentation is written in Spanish and Portuguese. The software itself was relatively stable, but again requiring you to work line by line. It offers a lot of the minute control mentioned earlier. All of these software suites presented here can be a little cult-ish at times, requiring the user to learn their rituals and ways of doing things.

https://luarocks.org/

**Growth from here**

It took a lot of patience to get to this point. I admit to not being the fastest or most experienced at computer code, and having stuck to computer administration as a means to an end. I code when necessary but don't have the time to fix the bugs that were endemic to these tools. If you are interested, all of these options are open source and waiting for coding help. You need a healthy amount of coding experience and focus to be useful and effective to those ends. As a user, you can just concentrate on making stuff with MatterControl and Cura.

The extensibility of this setup is also worthy of mention. There is a lot of minute control over quality of the final product with just MatterControl and Cura. Everything else is still available like editing G-code, scripts, and downloading add-ons. I found no dead-ends in the last year of studying any of these options.  You can go straight through from design to printed results. Preference was given to ease of use, speed, and control of printed results.

Computer languages to study with are Python, C, C++, and SQL. G-code is the other. The solutions mentioned here allow an "infrastructure as code" approach that just depend on minimal administration skills to set up. 

For small electronics, Arduino and Raspberry Pi play a role in the functionality presented here. I use an Octopi for control of my Anycubic printer, which uses an Arduino for its brain. If you wish to use a Pi based 3D printer then that is up to you. You are not restricted to printer choice or OS preference. The beginning of this guide is focused on making a stable and usable experience in Linux. You can customize software, hardware, firmware, monitoring, sensors, etc. All of these present more options waiting to be used.

**Background**

The information and subject matter in this guide was studied for a bit over a year. I've been a Linux user for 5 years starting in Ubuntu 16.04. I have been a crack developer and hack in Linux for 2 years with Python and C++. If you need access to customization, then there are nearly limitless options in Ubuntu Linux. Trying to simplify those options and explain them easily is why this was written. Embedded systems and devices have been a career concentration for 10+ years inlcuding electronic fuel injection, X-ray scanners, medical devices, robotics and IOT. I am studying for an LPIC1 certification from the Linux Professional Institute, aiming to use my time and resources wisely during the pandemic, while probably working too much overtime testing embedded devices and systems. 

I have built an at-home Linux network with some older hardware to support this series of documentation. You are not required to invest in extensive hardware at all. Actual experience is needed for modern certifications, and I was looking to make unique use of these general Linux administration tools. I preferred to break  hardware down into smaller pieces for the sake of safety and reliability. I didn't want any dips or spikes in power supplies to hurt the entire system, so I broke hardware down into easily accessible breakpoints that talk easily on a common network. Mixing all of this with a business degree and IT programming certification, I am travelling full circle with embedded Linux for devices and instrumentation. Those skills were applicable in other areas that I brought together to support this. DevOps for 3D printing in Linux is currently a very specialized subject matter. It is poised to be a standard for open source manufacturing in the Industry 4.0 era. This is due to all the reason listed here. I hope to support the growth of this endeavour for end users, small/medium entreprises, and project management needs.

Thank you for your interest and time.
