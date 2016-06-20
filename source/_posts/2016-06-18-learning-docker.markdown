---
layout: post
title: "Learning Docker"
date: 2016-06-18 09:01:01 -0400
comments: true
---

**What are containers?**

Below is very High Level discussion

Any business requires applications to run their business, and for running those applications it requires some hardware, in past when we go to application owners and ask them what kind of hardware they require to run their application and always you know the answer will be  "hmmm... " "aaaa..", let's get the fastest machine.

and business will buy strong machine like 16 core CPUs, 32GB of memory and 200GB of disks.

later it's found that application is only using 10% of the resources and all other capacity is wasted, 

above is not a great model to follow and it requires some solution.

**VMware**

 
The solution to above problem is VMware or hypervisor, VMware is now much more mature, so let say for above configuration server if you find out server is only utilizing 10% or hardware, you can add more virtual machines to it.

Above solves the problem by making the utilization of server more efficient, but that's not the only problem we want to solve.

{% img http://www.virtuatopia.com/images/2/21/Type_1_virtualization.jpg %}

if you look at above Vmware/hypervisor architecture, it requires, hypervisor and on top of that it requires operating system(VMs), so if you are running five applications you will need to install five operating systems and application on top of that.

the cons of doing above are:

- you still have to manage those 5 operating system ( like patching, bug, upgrades ,rebooting, shutdown and so on), this requires extra resources.
- even if you have assigned 25% of capacity to each of your 5 VMs, they might be using 10% out of that 25%.
- and as always Cost and licenses to run those operatingsystems.

**Containers**

{% img http://2.bp.blogspot.com/-1ep1ZnQ7J4U/VKFqsRuBGTI/AAAAAAAAAEc/MbzWKcDrxsc/s1600/Docker-Engine.png %}

And here comes the containers, which solves the above problems, in case of containers, you only need to install single operating system on top of your hardware, and you can start containers on top of that, there is no need for hypervisors and operating systems for segregating different applications.

they are very light weight and very fast in starting and stoping. More details on containers is in next chapter. 

Note: i am not saying stop using hypervisor and move it to containers over night, as hypervisor is very mature and containers are moving fast and still under heavy development.

http://localhost:4000/what-is-docker
