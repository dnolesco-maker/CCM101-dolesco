Mission Reflection

In this lab you will have explored some important differences between various types of cloud storage, block, file, and object storage. For example, block and file storage divide up the data that they store into different sized components (blocks and files/folders respectively), while object storage takes a very different approach by storing everything as “objects” within “buckets”.

What are some use cases where it might make sense to use an object-based storage system rather than other forms? An obvious use case would involve systems expecting to receive millions upon millions of user uploaded photos. Using an object based system allows us to easily organize these photos on disk while allowing us to easily access them when needed.

Another advantage of object storage over block storage becomes more evident if we need to quickly retrieve large numbers of images from our collection of user-submitted content. This can often be done with no changes at all to our existing application code! It’s just a matter of having a good enough storage backend to support what our users expect.

I found that working with Docker makes deployment of services like MinIO much simpler since I was able to deploy the service as a container instance running its own storage server. By simply executing one command, I was able to launch the storage service, specify my login credentials, and even ensure the correct ports were exposed on my network interface. I used the pgssty/minio image instead of the minio/minio image listed in the lab instructions since I couldn’t download the latter.

Bucket – A bucket is basically a container that allows you to organize your objects within an object storage. As part of this lab, we have created one with client-photos as its name and uploaded our sample file to validate our storage system.

Enterprise Companies – Enterprise companies can safeguard their object’s data against potential server failure by implementing some sort of replication or having a redundant storage system backed up at different devices/locations.

Confidence Level On Linux Command Line – We got more comfortable working with the Linux command line as we executed some docker commands, checked what was going on with the containers, accessed the web-based storage console via port forwardings, etc.

The last thing we want to mention here is that sometimes things might go wrong when deploying solutions and it will take us time to find out why, then come up with other alternatives to make everything work again. So all-in-all, this laboratory has provided me with the ability to know how you can deploy and use an object storage in a cloud computing environment.
