# Caution.
there are no best-practices here..
in fact it's anti-best-practice here, for a very specific use case

# Debrepo
one of the early steps to going nearline is to get a local repository.

since i use debian, that's what i'll set up

# iso's vs Proper mirror
so, why's this repo based around the isos rather than a propper mirror.

well, i have a proper mirror.. and if its sync breaks, so does the mirror. 
Sure this makes it so your repo cant go stale, because you have to keep fixing it. but if i want to go nearline my repo shouldnt expire

so, we download the isos with jigdo, and dissasemble them again

# Setting up
make sure all the scripts are writable, and run setup. this ensure all needed, and a couple of convenince packages are installed

# First run
1. comment out rm debian-12* from get-updates
2. remove the comment from rm debian-update*
3. update gen-src to reffer to your server

4. run get-updates.
this will
- download the jigdo files.
- assemble the jigdo files into isos
- un-pack the isos into directories
- generate apt source listings
- to be done - pack source listings into the local repo
- refresh the local repo content

# Local repo
Primarily this is used to ensure all users have the requisite apt repo list
you can also just dump arbitary dpkg files in here


