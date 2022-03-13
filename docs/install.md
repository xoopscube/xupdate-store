---
layout: default
title: Getting started
nav_order: 10
---

# X-Update Store
{: .fs-9 }

X-Update Manager provides an effective and user-friendly dashboard with a set of features  
that can help manage the complex task of applying software updates to Web Applications.  
The software update management process is necessary to maintain operational efficiency,  
continuous improvement process and the stability of the Web Application Platform.   


<div class="code-example" markdown="1">
### The Minimum Requirements
</div>
```
        XCL version 2.3.x
        Apache, Nginx, etc.
        PHP 7.2.x
        MySQL 5.6, MariaDB
        InnoDB utf8 / utf8mb4
          
```

   
### X-Update Manager Installation  

1. First, log in to the administration area.    
2. Go to » Module Management
3. Click Install Module » X-Updater
4. Complete the Installation Wizard

Follow the instructions of the Installation Wizard.  
Finally, get and deploy modules, preloads and themes from X-Update dashboard.  

X-update always deploys the latest code of modules, preloads, and themes.

### Administration Settings  

Free public store    
Copy this link and past in the input field of X-Update Manager Preferences

```html
https://xoopscube.github.io/xupdate-store/modules_xcl.ini


```

### X-Update Manager Preferences

#### FTP library 

- Direct (Files owner is PHP)
- Custom FTP (standard)
- PHP_FTP (for FTPS)
- Custom SSH_FTP (for SFTP)
- Custom SSH2 (for Key-Auth)

#### SSH connection port

- SSH port for SSH_FTP or SSH Key-Auth connection
- Private key for SSH connection

#### Custom Permissions

- File permission modification 
- Writable directory

#### X-elFinder Module

- Preload files (php extensions) can be edited with X-elFinder

#### Other options

- Debug output
- Themes Store
- Updates Store
- Maximum HTTP connections
- Disable SSL certificate verification in curl
- Set the number of curl simultaneous connection

