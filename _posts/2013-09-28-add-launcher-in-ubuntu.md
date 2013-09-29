---
layout: post
title: add program to Dash Home and launcher 
category: ubuntu
tag: [ubuntu]
---
Programs in Dash Home are configured in /usr/share/applications, so what we need is created one for our own program.

so we created a file in directory /usr/share/applications named eclipse.desktop, and filled with below

~~~~~~~~~~~~{.bash}
[Desktop Entry]
Version=4.2
Name=Eclipse Juno
Exec=/usr/local/eclipse/eclipse
Terminal=false
Icon=/usr/local/eclipse/icon.xpm
Type=Application
Categories=Development
~~~~~~~~~~~~~~

Then we should find program named eclipse in type Application in Dash Home. Open it, then you should be able to lock it in the launcher.
