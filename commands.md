### Opening an url window
 
 gnome-open ( url name ) 
 
### Create a directory and any parents that don't already exist
 
 mkdir -p ( For example - src/js/store )


### Quicker filesystem navigation
pushd *directoryname* => navigate to directoryname and push your starting location to the stack.
dirs -v => Show what directories are on the stack
popd => navigate to the last directory in the stack
cd ~x (where 'x' is the position of that directory on the stack) jump to a directory that has previously been pushed to the stack.

### Find a process to kill quickly
pgrep *Nameof Process* (can also use wildcards)

### Make du and df commandds more useful
alias df='df -hT -x tmpfs'

### Extract tar.gz archive from the command line
tar -xzvf *filename*

### View the list of stuff installed on your linux
dpkg --list

### Uninistall the package
sudo apt-get purge packagename

### Convert a value between different number systems
**Decimal to Binary**
echo "obase=2; $VALUE" |bc

**Binary to Decimal**
echo "ibase=2; obase=2; $VALUE" |bc

**Decimal to Hexadecimal**
echo "obase=16; $VALUE" |bc

**Hexadecimal to Decimal**
echo "ibase=16; obase=10; $VALUE" |bc

### Add prefix to all files inside a directory(replace "PRE_" to any text).
find * -maxdepth 0 -exec mv {} PRE_{} \;
