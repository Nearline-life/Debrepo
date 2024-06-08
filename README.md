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
