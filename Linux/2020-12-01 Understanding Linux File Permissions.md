# Understanding Linux File Permission
File permission is part of the security feature in Linux.

## 1. Basic File Permission
Each file and directory has 3 user based permission groups:
        - **owner**
        - **group**
        - **all users**

## 2. Permission Types
Each file and director has 3 basic permission types:
        - **read**
        - **write**
        - **execute**

## 3. How to view the file permission in terminal
Execute the command `ls -l` to view the file or directory permission. In terminal the permission will display `_rwxrwxrwx 1 owner:group`.

|No|Character(s)|Description|
|:---:|:---|:---|
|1.| `_`|Special permission flag that can be vary|
|2.| `rwx`| 1st group character is for **Owner permission**|
|3.| `rwx`| 2nd group character is for **Group permission**|
|4.| `rwx`| 3rd group character is for **All User permission**|
|5.| `1`  | The number of hardlinks to the file|
|6.| `owner:group`| Owner and Group assignment|

To modify the permission, use the `chmod` command.

## 4. Assignment of Permission
There are 2 ways to explicitly assign permission:
        - by permission group and permission type
        - by using binary references

### Permission Group and Permission Type
|Permission Group|Description|
|:---|:---|
|**u**| Owner|
|**g**| Group|
|**o**| Others|
|**a**| All Users|

|Assignment Operator|Description|
|:---|:---|
| **+**| Add Permission|
| **-**| Remove Permission|

|Permission Type|Description|
|:---|:---|
|**r**|Read|
|**w**|Write|
|**x**|Execute|

**Example:**  
- To remove read and write permission of a `fileA` for All Users: **chmod a-rw fileA**
- To add read and write permission for `fileA` to All Users: **chmod a+rw fileA**

### Binary Reference
|Permission Type|Value|
|:---|:---:|
|**r**|4|
|**w**|2|
|**x**|1|

**Example:**  
- To set a file permission on `fileA` to read **_rwxr_____**: **chmod 740 fileA**

## 5. Change Owners and Groups
The command is `chown`. For example, to change `fileA` to user1 and family group, simply invoke the command `chown user1:family fileA`


---

### Source
1. [Linux.com](https://www.linux.com/training-tutorials/understanding-linux-file-permissions/)
