# Web Server Default Configuration

## IIS
```eval_rst
+---------------------------+----------------------------------------------------------------+
| Web Setting               | Default                                                        |
+===========================+================================================================+
| Installed Version:        | Latest Version                                                 |
+---------------------------+----------------------------------------------------------------+
| Installed Components:     |                                                                |
+---------------------------+------------------+------------------+--------------------------+
| Web-Server                | Web-Basic-Auth   | Web-ISAPI-Ext    | Web-Scripting-Tools      |
+---------------------------+------------------+------------------+--------------------------+
| Web-Http-Redirect         | Web-Windows-Auth | Web-ISAPI-Filter | Web-DAV-Publishing       |
+---------------------------+------------------+------------------+--------------------------+
| Web-CGI                   | Web-Net-Ext      | Web-Mgmt-Console | Web-Custom-Logging       |
+---------------------------+------------------+------------------+--------------------------+
| Web-Http-Logging          | Web-Includes     | Web-Mgmt-Tools   | Web-Stat-Compression     |
+---------------------------+------------------+------------------+--------------------------+
| Web-Filtering             | Web-ASP          | Web-Asp-Net      | Web-Asp-Net4 [2012 only] |
+---------------------------+------------------+------------------+--------------------------+
| Web-Net-Ext45 [2012 only] |                  |                  |                          |
+---------------------------+------------------+------------------+--------------------------+
```

## NGINX
```eval_rst
+----------------------+------------------------------------------------------------------------------+
| Web Setting          | Default                                                                      |
+======================+==============================================================================+
| NGiNX Version:       | Latest version from EPEL repository                                          |
+----------------------+------------------------------------------------------------------------------+
| Mount Point:         | /var/www/vhosts                                                              |
+----------------------+------------------------------------------------------------------------------+
| Additional Features: | N/A                                                                          |
+----------------------+------------------------------------------------------------------------------+
| Configuration:       | VirtualHosts will be set up under the mount point for the domain example.com |
+----------------------+------------------------------------------------------------------------------+
```

### APACHE
```eval_rst
+----------------------+------------------------------------------------------------------------------+
| Web Setting          | Default                                                                      |
+======================+==============================================================================+
| APACHE Version:      | Latest version from default repository                                       |
+----------------------+------------------------------------------------------------------------------+
| Mount Point:         | /var/www/vhosts                                                              |
+----------------------+------------------------------------------------------------------------------+
| Additional Features: | N/A                                                                          |
+----------------------+------------------------------------------------------------------------------+
| Configuration:       | VirtualHosts will be set up under the mount point for the domain example.com |
+----------------------+------------------------------------------------------------------------------+
```

## PHP
```eval_rst
+----------------------------+-----------------------------------------------------------------+
| Web Setting                | Default                                                         |
+============================+=================================================================+
| PHP Version:               | Latest version from default repositories                        |
+----------------------------+-----------------------------------------------------------------+
| Mount Point:               | /var/www/vhosts                                                 |
+----------------------------+-----------------------------------------------------------------+
| Specific Modules Required: | N/A                                                             |
+----------------------------+-----------------------------------------------------------------+
| Configuration:             | Separate PHP-FPM processes should be run for each VirtualHost.  |
|                            |                                                                 |
|                            | Service should listen on the server’s primary IP address.       |
+----------------------------+-----------------------------------------------------------------+
| Specific php.ini configs:  | display errors: On                                              |
|                            |                                                                 |
|                            | date.timezone: Europe/London                                    |
+----------------------------+-----------------------------------------------------------------+
```

```eval_rst
  .. meta::
      :title: UKFast web build documentation | UKFast Documentation
      :description: Build documentation for web servers
      :keywords: ukfast, hosting, web, server, virtual
