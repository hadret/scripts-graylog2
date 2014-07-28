graylog2 systemd scripts
===

Here you can find systemd scripts for latest (v0.20.6) graylog2-server and
graylog2-web. Please note, that this script assumes couple of things:

* systemd is in version 208 or newer
* graylog2-server is located in /opt/graylog2-server
* graylog2-web is located in /opt/graylog2-web
* graylog2-server is running on the same machine as Elasticsearch and MongoDB
(if this is not the case, just remove Requires section from graylog2-server
script)


Installation
===

**graylog2-server:**

    sudo wget -O /lib/systemd/system/graylog2-server.service ...
    sudo systemctl enable graylog2-server
    sudo systemctl start graylog2-server

**graylog2-web:**

    sudo wget -O /lib/systemd/system/graylog2-web.service ...
    sudo systemctl enable graylog2-web
    sudo systemctl start graylog2-web


Authors
===

Filip "Hadret" Chabik <hadret@gmail.com>

_(Remember to add yourself when pull requesting)._ 
