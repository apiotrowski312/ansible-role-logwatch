logwatch
=========

Simple role to install and config logwatch.


Role Variables (with defaults):
--------------

```
logwatch_logDir: /var/log
logwatch_tmpDir: /var/cache/logwatch
logwatch_output: stdout
logwatch_format: text
logwatch_encode: none
logwatch_mailTo: root
logwatch_mailFrom: Logwatch
logwatch_filename: /tmp/logwatch
logwatch_archives: "No"
logwatch_range: yesterday
logwatch_detail: Low
logwatch_service: All
logwatch_mailer: "/usr/sbin/sendmail -t"
```

Example Playbook:
----------------

    - hosts: all
      roles:
        - role: apiotrowski312.logwatch
          logwatch_format: html


To Do
----------------
- list of logwatch_service to exclude

License
-------

MIT
