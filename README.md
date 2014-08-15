# Ansible Login Role

[![Build Status](https://travis-ci.org/weareinteractive/ansible-role-login.png?branch=master)](https://travis-ci.org/weareinteractive/ansible-role-login)
[![Stories in Ready](https://badge.waffle.io/weareinteractive/ansible-role-login.svg?label=ready&title=Ready)](http://waffle.io/weareinteractive/ansible-role-login)

> `login` is an [ansible](http://www.ansible.com) role which: 
> 
> * installs login
> * configures login

## Installation

Using `ansible-galaxy`:

```
$ ansible-galaxy install franklinkim.login
```

Using `arm` ([Ansible Role Manager](https://github.com/mirskytech/ansible-role-manager/)):

```
$ arm install franklinkim.login
```

Using `git`:

```
$ git clone https://github.com/weareinteractive/ansible-role-login.git
```

## Variables

```
login_umask: 022
login_usergroups_enab: 'yes'
```

## Example playbook

```
- host: all
  roles: 
    - franklinkim.login
  vars:
    login_umask: 002
```

## Testing

```
$ git clone https://github.com/weareinteractive/ansible-role-login.git
$ cd ansible-role-login
$ vagrant up
```

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests and examples for any new or changed functionality.

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## License
Copyright (c) We Are Interactive under the MIT license.
