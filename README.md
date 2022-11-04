Exim4
=====

Simple role to install and configure exim4. This role will handle vmails, mailing lists, etc. (in a close future).

Mailman3 and Mailman3-web are now supported by this role. vhost/vmail not yet.

Requirements
------------

No requirements

Role Variables
--------------

By default the role didn't install exim4 nor configure it

* `exim4__install` Should install or not (Default : False)
* `exim4__configure` Configure or not (Default : False)
* `exim4__root_email` Destination of local root mails (No default)
* `exim4__conf`
  *  `split` use splitted config
  *  `type` server type
  *  `smarthost` to which server resend outgoing mail
  *  `readhost`

Dependencies
------------

None

Example Playbooks
-----------------

Play with:

```
- hosts: all
  name: Setup Exim4
  roles:
    - role: exim4
```

License
-------

GPLv3

Author Information
------------------

François TOURDE

