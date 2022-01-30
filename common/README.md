Lab.Common Ansible Collection
=============================
This collection is part of the [lab](https://github.com/suppaduppax/ac_lab) namespace.

Installation
------------
If this wasn't installed by cloning https://github.com/suppaduppax/ac_lab then ensure that the collection is cloned inside the collections/lab directory inside your ansible collections directory to keep documentation consistent. 

Install as a submodule into your ansible project's collection's lab directory:

Create the collections directory
```
mkdir -p collections/lab
```

Change to the directory you just made
```
cd collections/lab
```

Add the submodule in the lab collection, renaming the `ac_lab_common` repo to `common` 
```
git submodule add ssh://git@github.com/suppaduppax/ac_lab_common.git common
```
