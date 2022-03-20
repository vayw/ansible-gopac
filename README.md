Role Name
=========

simple proxy.pac file server written in go

Requirements
------------

Proxy is not included

Role Variables
--------------

```
gopac_proxy_domains: list of domains proxy will work for (subdomains will be proxied to)
gopac_ip: address of server
gopac_proxy_address: proxy server address
gopac_proxy_port: proxy server port
gopac_proxy_scheme: proxy scheme (default to SOCKS5)
```


Example Playbook
----------------

```
- role: gopac
  tags: [gopac]
  vars:
    gopac_proxy_domains: ["exaple.com", "blocked.org"]
    gopac_ip: 192.168.10.1
    gopac_proxy_address: 192.168.40.40
    gopac_proxy_port: 8080
    gopac_proxy_scheme: HTTP
```

License
-------

BSD

