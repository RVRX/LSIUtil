# LSIUtil
Archive of the LSIUtil RAID controller software binaries and source.

A tool for working with some LSI RAID controllers, I have used it for controlling a SAS1068E on linux (LSI Logic / Symbios Logic SAS1068E PCI-Express Fusion-MPT SAS (rev 08))

LSIUtil is kind of hard to find online in binary format or source.
If you find binaries or source for different versions, feel free to make a pull request.
Hope this helps someone.

## useful command
```
echo $(( 16#$( sudo ~/LSIUtil/Binaries/LSIutil_1.71_binaries/Linux/lsiutil.x86_64 -p1 -a 25,2,0,0 | grep IOCTemperature: | cut -dx -f2 ) ))
```
