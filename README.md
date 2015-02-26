# Bootstrap: FreeBSD

This is a very simple Role designed to "bootstrap" FreeBSD 10 with a Python 2.7 installation. Without this, a very minimal FreeBSD 10 installation won't support Ansible modules (except for the odd exception, such as the [raw](http://docs.ansible.com/raw_module.html) module, which this Role actually uses.)

## Notes

- You have to turn off fact gathering to bootstrap a Python-less system. If you don't turn off fact gathering, Ansible will still attempt to call out to a Python binary, preventing the boostrap process.
- This is Role may seem like a waste of time and space, but if the need to make the bootstrap process more complicated ever arises, then there is a Role in place to work with.

## License

GPLv3

Author Information
------------------

- Michael Crilly
- Autologic Technology Ltd
- http://www.mcrilly.me/
