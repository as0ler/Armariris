# Armariris
Armariris - LLVM Confusion Framework maintained by the Code and Computer Security Lab of Shanghai Jiaotong University

Main author: f1ys0ar ( https://github.com/flysoar/ )

## English

Armariris: an obfuscator based on LLVM project for multiple languages and platforms.

Currently support:
 - string obfuscation
 - control flow flattening
 - instruction substitutions


### Armariris
Armariris is the alias of Amaryllis in conlang Selahpheno in sazaneK's light novel.
Amaryllis is a character in light novel <黄昏色の詠使い> and <氷結鏡界のエデン> written by 細音啓(sazaneK).
Although nobody unserstands her, she still guards her sister and the world persistently.

### Installation
```shell
mkdir obf
cd obf
git clone git@github.com:gossip-sjtu/Armariris.git
cmake -DCMAKE_BUILD_TYPE:String=Release ./../Armariris
make -j4
```

### Usage
Add option for opening string obfuscation when compiling.
```shell
-mllvm -sobf
```
Add option for opening control flow flattening when compiling.
```shell
-mllvm -fla
```
Add option for opening instruction substitutions when compiling.
```shell
-mllvm -sub
```
Add option for setting random seed.
```shell
-mllvm -seed=0xdeadbeaf
```
