# Conflict Example

## About

This repository is used as a submodule within the driftool as an example.
You find the driftool here: https://github.com/convidev-tud/driftool

## Content

This repository contains some branches and files that deliberately cause merge conflicts.

### Branches

* main
* feature/a
* feature/b
* feature/c

Each branch contains the additional files: 
* numbers.txt
* letters.txt

Due to synthetic modifications, the following merge conflicts occur:

a <-> b : 1 cf in letters; 2 cf in numbers
a <-> c : letters in c deleted vs changed; 1 cf in numbers
b <-> c : letters in c deleted vs changed; 1 cf in numbers

### main

**main/numbers.txt**
```
1
2
3
```

**main/letters.txt**
```
a
b
c
```

### feature/a

**main/numbers.txt**
```
1!
2+
3
```

**main/letters.txt**
```
a
b
c
d
```

### feature/b

**main/numbers.txt**
```
1?
2-
3
```

**main/letters.txt**
```
a
b
c
x
```

### feature/c

**main/numbers.txt**
```
1
2?
3
```