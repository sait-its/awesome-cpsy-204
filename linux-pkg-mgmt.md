### Package Management in Linux

https://www.linode.com/docs/guides/linux-package-management-overview/

> On Linux, software is typically built as a *package*, distributed through *repositories*, and managed on the end-user’s system through *package managers*. Each Linux system typically contains thousands of packages, many of which are required dependencies for other packages.

> #### Core Concepts for Package Management
>
> #### Packages
>
> Most software applications designed for Linux or Unix systems are distributed as *packages*, which are archives that contain the pre-compiled binary software files, installation scripts, configuration files, dependency requirements, and other details about the software. These packages are typically specific to a particular distribution and formatted in that distribution’s preferred package format, such as `.deb` for Debian/Ubuntu and `.rpm` for CentOS/RHEL.
>
> While it’s relatively simple for a user to install a package file, there are other complexities to consider. These complexities include obtaining (downloading) the package, ensuring packages are upgraded with security and bug fixes, and maintaining all the dependencies for the software.
>
> #### Repositories
>
> While a user can obtain package files through any method of file transfer, it is typical to use *software repositories* (also called *repos*) to obtain packages. Repositories are simply the location where the packages are stored, commonly accessible via the internet. A repository can contain a single package or thousands of packages. Most Linux distributions have their own unique repositories, sometimes separating out their cores packages into one while additional features are in others.
>
> #### Dependencies
>
> Its very common in almost any operating system for software to require other software to run. In Linux, each package contains metadata detailing the additional packages that are required. These additional packages are called *dependencies*. A single package can sometimes have hundreds of dependencies. When installing, upgrading, or removing packages, these dependencies may also need to installed, upgraded, and optionally removed.
>
> #### Package Managers
>
> A *package manager* reduces the complexity for the end-user by automating the process of obtaining, installing, upgrading, and removing packages *and their dependencies*. This dramatically improves the user experience and the ability to properly and efficiently manage the software on your Linux system. Today, package managers can be a defining feature for Linux distributions and many system administrators prefer to use a particular distribution based on its package management system (among other considerations).

> #### Benefits of Package Management Systems
>
> - **Easily obtain the correct, trusted, and stable package for your Linux distribution.** Since most distributions maintain their own repositories, using a package manager can ensure you only install packages that have been thoroughly vetted, are stable, are trusted, and work with your system. The subjective judgments and community standards that guide package management also guide the “feel” and “stability” of a given system.
> - **Automatically manage all dependencies when taking action on a package.** While dependencies can be distributed inside the original package to ensure the correct versions of the required software are always present, this increases disk usage and package file size. In most cases, package managers will manage dependencies as separate packages, allowing them to be shared with other software and reducing disk usage and file size.
> - **Follow the unique conventions for each Linux distribution.** Linux distributions often have conventions for how applications are configured and stored in the `/etc/` and `/etc/init.d/` directories. By using packages, distributions are able to enforce a single standard.
> - **Stay up-to-date on security patches and software updates.** Most package managers provide a single command to automatically update all packages to the latest versions stored on the configured repositories. Provided those repositories are consistently maintained, this enables you to quickly get important security updates.



---

#### RHEL/AlmaLinux/Rocky Linux Package Management

DNF vs. YUM - Learn the Differences: https://phoenixnap.com/kb/dnf-vs-yum

Add EPEL to Red Hat: https://www.redhat.com/en/blog/whats-epel-and-how-do-i-use-it

Enable EPEL and EPEL Next in AlmaLinux 9 or Rocky Linux 9: https://linux.how2shout.com/enable-epel-and-epel-next-in-almalinux-or-rocky-linux-9/ 