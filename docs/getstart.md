---
layout: default
title: Getting started
nav_order: 10
---

# Getting started
{: .no_toc }

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

---


## Overview

X-Update ensures that the latest code for modules, preloads and themes is always deployed.  
In order to reduce the overhead of getting `ini` files from each store registered in X-Update,   
we merge the static files using GitHub pages.

> Note that any future changes made to the `ini` file of xupdate_store   
> must be updated in the gh-pages branch of the xupdate-store repository.


## INI File

An `.ini` file contains configuration information in a simple, predefined format.  
It is used by applications to store information about the preferences and operating environment.  
These files are plain text files with a basic structure comprised of properties and sections.  

It is pronounced as “dot in-ee" or simply "in-ee” file, where .ini signifies “initialization."  

Initialization File should always use the UTF-8 character encoding.  
This means the content also needs to be saved as UTF-8.  

## Format of .ini file

**Property** : The basic element contained in an `.ini` file is a property.  
Each property includes a name and a value that are delimited using a sign `=` "equals".  
This is represented in the format "keyname=value".

**Section** : The properties can be arranged into arbitrarily named “sections” in the file.  
Every section begins with a section header containing a section name in the square brackets.  
For example, `[section name]`

**Comment** : The semicolons `;` used at the start of the line represent a comment.   
The commented lines are usually ignored.

## Format of modules.ini

"modules.ini" needs to be UTF-8 encoding. 

Two or more specifications are possible for  
- "no_update[]", 
- "no_overwrite[]", 
- "writable_dir[]", 
- "writable_file[]", 
- "delete_dir[]" and "delete_file[]" respectively.


## module.ini

```
[ItemKey]                 ; Probably it will be the same as that of target_key, and is good.
dirname = "dirname"       ; module directory name (string)
target_key = "UniqKey"    ; Unique key (string)
target_type = "X2Module"  ; TrustMudule , X2Module or Theme (string)
version = 1.00            ; Version numbar (float)
detailed_version = ""     ; Detailed version (string) [optional]
replicatable= false       ; Replicable i.e. D3 (bool)
addon_url = "https://"    ; Archive URL ( %s replaces target_key ) (string) 
detail_url = "https://"   ; Detail page URL [optional] (string)
changes_url = "https://"  ; Recent changes page URL [optional] (string)
license = "GPL"           ; Software license (string)
required = "normal"       ; required , recommend or normal (string)
description = ""          ; General description
screen_shot = "https://"  ; URL screenshot (Theme only) [optional] (string)
tag = ""                  ; Tags (separated with a space) [optional] (string)
force_languages = ""      ; Force upload language directory with `Used language only`. [optional] (string comma delimited)
no_update[] = ""          ; Do copy only installing [optional] (string)
no_overwrite[] = ""       ; Do copy only file not exists [optional] (string)
writable_dir[] = ""       ; Set write permission to directory [optional] (string)
writable_file[] = ""      ; Set write permission to file [optional] (string)
delete_dir[] = ""         ; Delete unnecessary Directory [optional] (string)
delete_file[] = ""        ; Delete unnecessary File [optional] (string)
```

## Label of ini files for X-update

<div class="code-example" markdown="1">
Stable
{: .label .label-green }

Module
{: .label .label-blue }

Preload
{: .label .label-purple }

Theme
{: .label .label-yellow }

Update
{: .label .label-red }
</div>
```markdown
Stable
{: .label .label-green }  
Module
{: .label .label-blue }  
Preload
{: .label .label-purple }  
Theme
{: .label .label-yellow }  
Update
{: .label .label-red }
```


* * *

## GIT commit


Enter git status to see the changes to be committed.  
Enter git commit -m '<commit_message>'  
at the command line to commit new files/changes to the local repository.  
For the <commit_message>, you can enter anything that describes the changes you are committing.  
Commit files to the xupdate-store Git repository.


## [](#header-2)Branch gh-pages

Set-up the gh-pages tracking branch (when the remote name is origin)

```
git fetch origin git checkout -b gh-pages origin / gh-pages

```

### [](#header-3)Modify & commit   

First time :  

```
git push -u origin gh-pages to track with -u option
```

Then :  

```
git pull 
```

A simple git push will do fine.
