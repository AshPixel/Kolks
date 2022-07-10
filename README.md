# ![Kolks Logo](/kolks_full.png "Kolks Logo")

Version 1.3, Build: ***Stable***

## Introduction
### About Kolks:
Kolks is a high-level programming language. The goal of Kolks was to originally create a moderately good and functional programming language that may used in professional cases. Instead the goal of Kolks is to make a easy to learn programming language, while still having the capabilities to create a wide-range of products and programs.

Kolks is created by: Ashton "Pixel" Melvin.

### How to install Kolks:
#### Windows:
1. Download and run the setup file. ``Kolks-v1.3.exe`` This will also add Kolks to the path.  
2. Start Creating! Have fun with Kolks!

#### Linux:
Install the Linux Package "wine" and attempt to run it.

# Official Links:
#### Website: https://kolks.glitch.me/
#### GitHub : https://github.com/AshPixel/Kolks/
#### VSCode : https://marketplace.visualstudio.com/items?itemName=KolksTeam.kolks
#### Discord: https://discord.gg/vu7bxCHu84
#### Twitter: https://twitter.com/KensuiE

# Getting Started:
## Hello Kolks!
Make a new folder, this is where our project will be located. Lets name it "HelloKolks". Lets create the main file, which will be called "main.ko".

Lets write "Hello Kolks":
```objectivec
  #write "Hello Kolks!";
```

This should output:
```log
> kolks main.ko
  Hello Kolks
  # Kolks Program Terminated: [time]
```

Optionally for single-file projects such as this one you can use a entry function that only runs the main file. Such as:
```objectivec
  #define *% ~ () {
    #write "This should only show if this is the file your running";
  };
```

This should output the same thing:
```log
> kolks main.ko
  Hello Kolks
  # Kolks Program Terminated: [time]
```

## Group and Assign
After writing your first Kolks Script you will need to learn how to store variables and make functions.
You make can make functions like so:
```objectivec
  #define milk ~ () {
    
  };
```

This is a pretty bland function but since it doesn't have anything in it lets add a variable:
```objectivec
  #define milk ~ () {
    #define coffee ~ "Perfectly done";
  };
```

Okay now that we know how to make functions lets run it!
This should output:
```log
> kolks main.ko
  # Kolks Program Terminated: [time]
```

Uh-oh it seems that we haven't ran our function or used the variable at all! Lets quickly do that.
You run functions like:
```objectivec
  milk();
```

and for now you can use `#write coffee;` to print the current variable.
Your file should now look like:
```objectivec
  #define milk ~ () {
    #define coffee ~ "Perfectly done";
    #write coffee;
  };
  milk();
```
This should output:
```log
> kolks main.ko
  Perfectly done
  # Kolks Program Terminated: [time]
```
# Beginner Concepts
## Conditions
Conditions (If you don't know already) are statements where the output only runs if the condition is true.
As a example lets set a condition so see if apples are red:
```objectivec
#define apples ~ "red";
#if apples == "red" {
  #write "Apples are red";
};
``` 
If we run the file:
```
> kolks main.ko
  Apples are red
  # Kolks Program Terminated: [time]
```
Success!
