---
layout: default
title: Settings
nav_order: 40
---


# [](#header-1)Settings


In order to reduce the overhead of getting ini files from each store  
registered in X-update, we merged to static files using GitHub Pages.  

> Note that any future changes made to `ini` of xupdate_store   
> should be update to the gh-pages branch of the repository.


ini files for X-update

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


* * *

