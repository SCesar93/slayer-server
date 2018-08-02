# Slayer-Server-10x
Complete global server, map with halls of hope, wrap, store ingame, prey system, imbuing system.

# System requirements
Ubuntu 14.04 LTS and Windows 7+

# Events
Snow Ball<br>
Castle<br>
Zoombie<br>
BattleField

# How to's
How to make own client <a href="https://www.google.com.br/search?q=fazendo+seu+proprio+cliente+8.6+10xx&spell=1&sa=X&ved=0ahUKEwib8-Hp1r7VAhXG8CYKHRU4BVwQvwUIJCgA&biw=1366&bih=662">Click here</a>

# Downloads
Client version 10x with Retro Outifts <a href="https://mega.nz/#!TkJRTIhS!-pp6FSLWuey8S2KWdYYKDbQrSParGZ8yW5LeaWichNc">Click here</a><br>
Website<a href="https://github.com/Qwizer/gesior-accmaker">Click here</a>

# Utils
IpChanger versions 7.x - 10.x: <a href="https://static.otland.net/ipchanger.exe">Click here</a>

#Run exec to create database schema
mysql -u user_name -p db_name < script.sql

#Generate tfs in windows
Download visual studio <a href="https://msdn.microsoft.com/pt-br/library/e2h7fzkw.aspx">Click here</a><br>
Install C/C++ libraries. <br>
Clone vcpk.git repository: git clone https://github.com/Microsoft/vcpkg.git<br>
Install vcpkg .\bootstrap-vcpkg.bat <br>
and .\vcpkg integrate install <br>
Install boost libraries <a href="https://sourceforge.net/projects/boost/files/boost-binaries/1.62.0/boost_1_62_0-msvc-14.0-64.exe/download">Click here</a><br>
Install tfs sdk v.3.2 <a href="https://static.otland.net/dl/tfs-sdk-3.2.zip">Click here</a><br>
Run inside tfs-sdk folder the file register_tfssdk_env to register in path. <br>
Copy the file register_boost_env to boost library folder. <br>
Open the file 'theforgottenserver.vcxproj.user' with visual studio. <br>
Go in properties >> C/C++, change the inclusion directories, and add tfs-sdk folder (mysql-connector, luajJIT, mpir .. only the include folder), and finally add boost folder. <br>
Now go in properties >> Vincular, change the additional libs, and add the sames folder previous, only change the folder from include to lib64. <br>
Save everything in visual studio, and recompile.


# Generate tfs in ubuntu
Install dependencies<br>
$ sudo apt-get install git cmake build-essential liblua5.2-dev libgmp3-dev libmysqlclient-dev libboost-system-dev libboost-iostreams-dev libpugixml-dev<br><br>
Enter in main dir and run<br>
$ mkdir build && cd build<br>
$ cmake ../source<br>
$ make

# Extract map
Need enter in folder /data/world and extract the ot serv map

# GOD Account
Password: 2/god


# TODO:
Adjust xp stages. <br>
Adjust initials items (add more gold and reward by level). <br>
Adjust mana/hp regen. <br>
Adjust spells cds. <br>
Create site.