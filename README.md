# How to change color of root bash

# Start editin the .bashrc file

vim .bashrc

# Remove the comment of the force_color

#force_color_promt=yes

force_color_prompt=yes

# In the end of file, put the command for:

####Green Prompt User

PS1='${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\]\$ '

####Red Prompt for you user

PS1='${debian_chroot:+($debian_chroot)}\[\033[01;31m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\]$ '

# How this work

\[\033[Z;YY;XXm\]

Where Z is the characters style, YY is the background color and XX is the characters color.

# Color Codes

Black	  30

Blue	  34

Green	  32

Cyan	  36

Red	    31

Purple  35

Brown	  33


# Background color codes

Black   40

Red     41

Green   42

Yellow  43

Blue    44

Purple  45

Cyan    46

Gray    47

# Characters Style

Normal 0

Bold 1 makes it brighter

Undescore 4

Blink 5

Inverse 7 Inverse background color

Concealed 8
