Legion::Crypt
=====

Legion::Crypt is the class responsible for encryption, managing secrets and connecting with Vault

Supported Ruby versions and implementations
------------------------------------------------

Legion::Crypt should work identically on:

* JRuby 9.2+
* Ruby 2.4+


Installation and Usage
------------------------

You can verify your installation using this piece of code:

```bash
gem install legion-crypt
```

```ruby
require 'legion/crypt'

Legion::Crypt.start
Legion::Crypt.encrypt('this is my string')
Legion::Crypt.decrypt(message)
```

Settings
----------

```json
{
  "vault": {
    "enabled": false,
    "protocol": "http",
    "address": "localhost",
    "port": 8200,
    "token": null,
    "connected": false
  },
  "cs_encrypt_ready": false,
  "dynamic_keys": true,
  "cluster_secret": null,
  "save_private_key": false,
  "read_private_key": false
}
```

Authors
----------

* [Matthew Iverson](https://github.com/Esity) - current maintainer
