# Docker-lab2
1-  Create MySQL database docker  image with:

•volume  called mysql_data to /var/lib/mysql

•Set ENV variable MYSQL_ROOT_PASSWORD to P4sSw0rd0!.
![Screenshot (810)](https://user-images.githubusercontent.com/93229250/229239217-647020c1-9166-40c6-938b-21bac956ebbd.png)
![Screenshot (808)](https://user-images.githubusercontent.com/93229250/229236488-38587ca2-ecd4-4aaf-a629-d5d4c94bdf4d.png)
2- What is the rest of Docker Networks ? “Name and Definition”

bridge: The default network driver. Bridge networks are usually used when your applications run in standalone containers that need to communicate.

host: For standalone containers, remove network isolation between the container and the Docker host, and use the host’s networking directly. 

overlay: Overlay networks connect multiple Docker daemons together and enable swarm services to communicate with each other. You can also use overlay networks to facilitate communication between a swarm service and a standalone container, or between two standalone containers on different Docker daemons. This strategy removes the need to do OS-level routing between these containers.

ipvlan: IPvlan networks give users total control over both IPv4 and IPv6 addressing. The VLAN driver builds on top of that in giving operators complete control of layer 2 VLAN tagging and even IPvlan L3 routing for users interested in underlay network integration.

macvlan: Macvlan networks allow you to assign a MAC address to a container, making it appear as a physical device on your network. The Docker daemon routes traffic to containers by their MAC addresses. Using the macvlan driver is sometimes the best choice when dealing with legacy applications that expect to be directly connected to the physical network, rather than routed through the Docker host’s network stack. 

none: For this container, disable all networking. Usually used in conjunction with a custom network driver. none is not available for swarm services.

3-What is the different  between  docker  images tags ?

Versioning: such as major versions, minor versions, or patch versions. For example, an image might have tags like 1.0, 1.1, and 1.2 to represent different releases.

Variants: such as images that have different operating systems, architectures, or configurations. For example, an image might have tags like ubuntu, alpine, or windows to represent different operating systems.

Stability: such as images that are in development, testing, or production. For example, an image might have tags like dev, test, or prod to represent different stages in the software development lifecycle.

Naming conventions: Docker image tags can follow different naming conventions depending on the organization or project that created the image. Common naming conventions include using semantic versioning, using descriptive names, or using a combination of both.
