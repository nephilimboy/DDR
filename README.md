# Data Distribution Routing

## Updating the readme and the code...

With continuous advancements in robotics and networking, 
the adoption of smart industrial machines for automation has grown 
significantly. Leveraging the Robot Operating System version 2 (ROS-2) and its
topic-based data distribution mechanism, these machines are typically controlled by 
software deployed in the cloud. This control software is structured as a chain of ROS-2 nodes, 
with each node responsible for managing a specific function or component of the industrial 
machine. By applying the concept of Service Function Chaining (SFC), 
these ROS-2 node chains can be deployed in a distributed manner
across cloud infrastructure. An SDN controller is employed to steer ROS-2 traffic 
efficiently along the sequence of nodes. As the number of industrial machines increases in 
large-scale factories, the number of corresponding ROS-2 node chains also grows. 
This trend underscores the need to reuse common ROS-2 nodes across multiple chains 
to optimize the utilization of cloud resources. However, the default topic-based communication model 
of ROS-2 is not inherently compatible with such reuse. Sharing common ROS-2 nodes across different 
chains becomes challenging, thereby hindering efficient resource management in cloud environments. 
To address this limitation, we propose a Data Distribution Routing (DDR) framework powered by 
a Spatial Attention Convolutional Neural Network (SA-CNN). 
The DDR is capable of classifying and steering ROS-2 traffic originating from shared 
nodes to their appropriate service chains. Furthermore, it supports the NetConf protocol to 
communicate with the Software-Defined Networking (SDN) controller. 
