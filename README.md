# rm

## Remove special chars
* Search the inode and remove by using find -exec
```
ls -i
284333 admin-openrc-clear.sh  284321 admin-openrc.sh  290808 --name
root@controller:/home/ubuntu# rm -i 290808


find . -inum 290808 -exec rm -i {} \;
rm: remove regular empty file './--name'? y
```
