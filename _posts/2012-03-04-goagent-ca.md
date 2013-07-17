---
layout: post
title: warning when visit https site use goagent
category: web
tag: [goagent]
---
when visit https sites like twitter,we account the warning "the site security certificate is not trusted",and can not proceed.
you need to add ca.crt of goagent to chrome:
~~~~~~~~~~~~~~~~~~~~~~ {.bash}
cp plugin/auto-pairs.vim ~/.vim/plugin
sudo apt-get install libnss3-tools
certutil -d sql:$HOME/.pki/nssdb -A -t "C,," -n GoAgent -i '/usr/local/goagent/CA.crt'
~~~~~~~~~~~~~~~~~~~~~~
then restart chrome.
