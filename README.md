# DotPack
A dotPack simulator for Squeak.

## Install
<!--1. put the `dotpack-removebg.png` file to the default folder(the folder Squeak image is in).-->

* drap DotPack.st into current world (Squeak screen) and choose `fileIn entire file`.

## Usage
```
|pack|
pack := DotPack new.
pack stopStepping.
"clear"
pack clear.

"hello world"
pack x:1 y:1 color: Color red.

"set background color"
pack backgroundColor: Color blue.
"use Inspector to explore it!"
pack inspect.

"run Snow Crash for 2 seconds"
[	pack startStepping.
 	2 seconds wait.
	pack stopStepping.] fork.
```

## work with dotPack device
ref: [Squeak 与 MicroBlocks 互操作](https://wwj718.github.io/post/%E7%BC%96%E7%A8%8B/squeak-microblocks-interoperability/)
