---
title: "How to make linux Symbolic Link"
excerpt: "리눅스 심볼릭링크 만들기"

categories: 
    - CSE
    - Linux
last_modified_at: 2020-10-12T09:00:00-01:00
---

## Linux symbolic link

I used symbolic links to share files with my teammates.  
It is easy to understand if you ever use windows shortcuts(it's the same with desktop icons).  
But linux has two types, hard link, and symbolic link and the difference between the two links is whether to create a new link file or not.  

command : ln [option] [file] [link]  
  
example : ln -s ./mytest.txt /desktop/mytest

options 
1. -b : If there is already the same name link file, os will create a link file after they make a backup file.
1. -d : They enable the creation of a hark link file about the directory.
1. -f : If there is already the same name link file, os will remove it and create the new link file.
1. -i : If there is already the same name link file, os will ask the user whether to remove the link file or not.
1. -t : You can select the directory where to make a link file.
1. -s : You can create a symbolic link.
  
If you make it wrong, you can check the red sign.  
![](https://sunahy1011.github.io/assets/images/symboliclink_error.png){: .align-center}  
This means that the link can not find the original file, and it also happens when the file name was changed.  


**Quotation**  
[personal blog](https://server-talk.tistory.com/140)