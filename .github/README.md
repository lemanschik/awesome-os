# AwesomeOS
AwesomeOS - AOS Main Repository of the Public Documentation and Parts for Enterprise Ask Frank

AOS is a general-purpose operating system, that can be built with the monolithic Linux kernel, The Mach Micro Kernel, The Zricon Fuchsia OS kernel, or any other Compatible Kernel that has C Binary Interop. Its package system allows you to quickly install, update and remove software; software is provided in binary packages or can be built directly from sources.

It is an independent distribution, developed entirely by Frank at present.

Unlike 99.99% of other existing distros, AwesomeOS is not a modification of an existing distribution. AwesomeOS is the first of Its Kind. As its package manager and build system Implementation, Unlike most Other distros, is independent it has no Affiliation to any of the Big Main Distros while our tooling works with any Linux, MacOS, Windows, Android, Fuchsia, LaCroOS, BSD, or Distribution.

focuses on stability, while being bleeding-edge. Install once, update routinely and safely.
Thanks to our continuous linear world wide build grid, new software is built into world wide accessible shared Memory exposed as Handels as soon as the changes are saved. This allows you to Realtime iterate over your code while adopting changes to production only after everything is fully tested and works as expected. Without Additional Deployment!

We Implemented highly Generic APIs for any need so that you got a Stable Platform where you can build and run your software on. No matter what workloads you targeting or if it is an IoT Device. Software Management is fully Handled by AwesomeOS 

The AwesomeOS Gui is Implemented in HTML CSS and Nativ ASM. Offering Scripting and Integration Support via ECMAScript and C++

Learn more about:
- The B8G Compiler Framework. If you want to create the next generation of Highly Efficient Services.
- The Stealify Lang Framework. If you want to Implement your own DSL or Instruction Procedural Language give it a shot.
- The Web Virtual Environments WVE Framework. If you want to Deploy use and maybe even improve the next generation of Containerised Workloads and System Emulation directly in any WInterOP Compatible Environment you found the right place.
  - Chromium Virtual Environments ChromiumVE is the First Implementation of this using the Chromium API all others get generated out of that.
- Learn more about the Chromium Project.
- Learn more about the Unlicense Code Project.
- Learn more about the future of Compilers: Principles, Techniques, and Tools in the 3rd Edition offered as Interactive Notebook
  - The White Dragon Book. - Can be also buyed as Subscription Model to Support Software Development patterns that are designed to be stable evolving and stop the framework horror.

## References and Demos
- https://opfs.zip A Single Private Place for your data that never transfers your data to us. Not even Routes your Data over us.
  - acts as WInterOP EntryPoint offers shareAble FileSystem Implementations. Based on the Origin Private FileSystem Concepts and API's
- https://cloud-fs.zip 
  - Adds Clustering and other services based on the opfs.zip implementation includes *.opfs.zip domain services. and *.cloud-fs.zip clustered services. 
- https://cloud-fs.zip/node The NodeJS Compatible Implementation of cloud-fs designed to be used via webrtc. 
- https://www.awesome-os.com A Webpage to get viewed it will never be neat or pritty but it will be a Entrypoint.
  - https://www.awesome-os.com/documentation Will be maybe a more nice view of this repositiorys main educational content.

## Some Entry Level Concepts about ECMAScript and C++ as also a bit ASM to Explain sharedMemory Handels
Maybe you know out of the WInterOP World already a bit about sharedArray Buffers which are transferable to a so called Context/World
a Context/World is something like a isolated System it got its own rules of execution and gets Manged by a Outer Component that instantiated it. This is called Capability based Permission Protocol Security and Handling. The Concept is Simple a Higher order Component that can be a Component Manager gets Some System Capabilitys to manage then this can be passed fully or partial to other
Components that are instantiated by it. This is Comapreable To the Rust Memory Management Principels with the Brrrow Checker.

While we do that on Execution. All ECMAScript code gets Ignited by v8 thats the term for turning your ECMAScript into ASM and then Reference that via a C++ Tempalte Function. This Turns Your Code Into Nativ ASM that Runs inside its own Context/World for internal
ipc we have the concept of so called Context Security ID's that are the same that get used internal in WebRTC Peer Sessions.

So we can work and operate even on Encrypted Memory. Memory is simple a Array of Data this data can be manipulated via ASM C or internal via the genrated ASM from ECMAScript code Ignition processes. In AswesomeOS how ever we try to unifie to the term Task for everything a Component executes runs defined tasks under defined conditions. The Task executin it self is watchable observable as it gets exposed as Handle that supports Streams to consume the processing progress or incremental results...... or even modify the runtime behavior via additional input like a contract. 
