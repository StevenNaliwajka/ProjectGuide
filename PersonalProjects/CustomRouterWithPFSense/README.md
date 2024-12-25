### PFSense

A custom router OS that takes the place of a typical OS like Windows or linux.

The main reason for going through the effort to create and configure a PFSense box is to allow for custom control
over your network.

I am NOT an expert and to this day im petrified that I configured something wrong.  
The best security is obscurity so, I can not go too far into detail.

The high level theory of what my current stack looks like is as follows:

1) Internet
- Paying for internet through an ISP, comes into the wall.
2) Modem
- Cord gets fed into a cheap modem I got off ebay.
- Modem communicates with the ISP and registers me with them.
3) PFSense box
- My custom PFSense box was thrown together with used parts pulled from the trash at work and a cpu bought from [Maiikiru](https://github.com/Maiikiru).
- To this day I have not bothered to put it in a case, it lives open on my server stack. (See photo in folder)


The PFSense box flags traffic on each of my machines under a few different categories. Different categories have different rules applied. 
This allows me to effectively create virtual 'subnets' and segment traffic however I please.

If configured correctly, any 'outward facing' devices or webservers should be isolated to themselves.  
Any front facing webserver should never be able to identify and communicate with my personal machine.

This means that there are multiple checks before any bad actor can penetrate the network. If they do gain access to a
single device, hopefully that device is isolated enough that it is useless.

But uh. If you are a bad actor... Don't punk my shit please, I'm a broke ass college student, most of my software is open source
and most of my hardware comes out of a dumpster. Thanks.
