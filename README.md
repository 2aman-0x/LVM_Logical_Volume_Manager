## LVM 
LVM is used to manage volume and disk on the Linux Server.  
Logical Volumn Manager allows disks to be combined togather.  

## Examples of LVM
Like partition of disk in windows C,D drive similarly we can do the same in the linux.  

- Single disk can be divided into different partitions.
- Multiple disks combined and group the into one -> then change it into different partitions

## Advantage of LVM

- In case of disk is running out of space, you can add new disk without breaking partitions of your system.

## Posibilities of LVM
- New space can be created on a server for new project
- In case of low disk space, increase the space.
- In case of extra space allocated to a partition, capacity can be reallocated (reduce capacity in one volume group and add it to another)

## Requirement 
We need to deploy two new applications app1 and app2 on our server and need a seperate partitons and space for each applications.

## Steps of LVM for adding new space

1. Install a new Hard Disk Drive
2. Make a partiton to use it
3. Designate Physical Volume
4. Manage Volume Group (VG)
5. Manage Logical Volume(LV)
6. Apply a filesystem
7. Set a mount point

## Partition usign 'fdisk'
1. Choose ```n``` to create new.
2. Choose ```p``` to create a primary partition.
3. Choose which number of partition we need to create.
4. Press ```Enter``` twice to use the full space of the Disk.
5. We need to change the type of newly created partition type ```t```.
6. Which number of partition need to change, choose the number which we created its ```1```.
7. Here we need to change the type, we need to create LVM so we going to use the type code of LVM as 8e, if we do not know the type code Press ```L``` to list all type codes.
8. Hx code (type ```L``` to list all codes): ```8e```
9. press ```w``` for write disk and created done for partion.
10.Write the changes and exit fdisk.
11. For checking ```fdisk -l```




