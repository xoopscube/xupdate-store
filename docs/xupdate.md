---
layout: default
title: X-Update Manager
nav_order: 20
---

# Install X-Update Manager
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

<div class="code-example">
## X-Update Manager Installation  
</div>
```
1. First, log in to the administration area.    
2. Go to » Module Management
3. Click Install Module » X-Updater
4. Complete the Installation Wizard
```

<div class="d-flex flex-justify-start bg-blue-000 m-4 p-4">
<div class="text-grey-lt-000">
<svg xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" viewBox="0 0 24 24" style="-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); transform: rotate(360deg);"><path d="M2 12A10 10 0 1 0 12 2A10 10 0 0 0 2 12m13.6 1.72A4 4 0 0 0 16 12a4 4 0 0 0-4-4v2L8.88 7L12 4v2a6 6 0 0 1 6 6a5.9 5.9 0 0 1-.93 3.19M6 12a5.9 5.9 0 0 1 .93-3.19l1.47 1.47A4 4 0 0 0 8 12a4 4 0 0 0 4 4v-2l3 3l-3 3v-2a6 6 0 0 1-6-6z" fill="currentColor"/></svg>
</div>

<div class="text-grey-lt-000 ml-2 p-2">
<p>Follow the instructions of the Installation Wizard.<br>  
Finally, get and deploy modules, preloads and themes from X-Update dashboard.<br>
X-update always deploys the latest code of modules, preloads, and themes.</p></div>
</div>
</div>

<hr>

<h2>X-Update Manager Preferences</h2>

<p>Free public store<br>
Copy this link and past in the input field of X-Update Manager Preferences</p>

```html
http://xoopscube.xyz/uploads/xupdatemaster/stores_json_V1.tx
```

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

