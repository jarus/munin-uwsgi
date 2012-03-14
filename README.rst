munin-uwsgi
===========

Is a plugin for the monitoring software `munin <http://http://munin-monitoring.org/>`_ to monitor `uWSGI <http://prosody.im>`_ processes. 

Wildcard plugin
---------------

munin-uwsgi is written as wildcard plugin which provides following suffixes:

* memory
* processes

Install
-------

It is very simple to install the plugin.

::

    cd /usr/share/munin/plugins

    wget https://raw.github.com/jarus/munin-uwsgi/master/uwsgi_
    chmod 755 uwsgi_ 
    
    ln -s /usr/share/munin/plugins/uwsgi_ /etc/munin/plugins/uwsgi_memory
    ln -s /usr/share/munin/plugins/uwsgi_ /etc/munin/plugins/uwsgi_processes

    
After the installation you need to restart your munin-node:

::

    /etc/init.d/munin-node restart

