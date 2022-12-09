# bviktor.cloudflare

## Synopsys

This role creates the `cloudflare` zone in firewalld that passes `https` traffic
between the host and Cloudflare's servers as described on their
[IP Ranges](https://www.cloudflare.com/ips/) page.

## Parameters

N/A

## Examples

```yml
- include_role:
    name: bviktor.cloudflare
```

## Return Values

N/A

## Support

| Platform | Support | Status |
|---|---|---|
| Linter | ✅ | [![Lint](https://github.com/noobient/ansible-cloudflare/actions/workflows/lint.yml/badge.svg)](https://github.com/noobient/ansible-cloudflare/actions/workflows/lint.yml) |
| AlmaLinux 8 | ✅ | [![AlmaLinux 8](https://github.com/noobient/ansible-cloudflare/actions/workflows/almalinux-8.yml/badge.svg)](https://github.com/noobient/ansible-cloudflare/actions/workflows/almalinux-8.yml) |
| AlmaLinux 9 | ✅ | [![AlmaLinux 9](https://github.com/noobient/ansible-cloudflare/actions/workflows/almalinux-9.yml/badge.svg)](https://github.com/noobient/ansible-cloudflare/actions/workflows/almalinux-9.yml) |
| Fedora 37 | ✅ | [![Fedora 37](https://github.com/noobient/ansible-cloudflare/actions/workflows/fedora-37.yml/badge.svg)](https://github.com/noobient/ansible-cloudflare/actions/workflows/fedora-37.yml) |
| Ubuntu 18.04 | ✅ | [![Ubuntu 18.04](https://github.com/noobient/ansible-cloudflare/actions/workflows/ubuntu-18.04.yml/badge.svg)](https://github.com/noobient/ansible-cloudflare/actions/workflows/ubuntu-18.04.yml) |
| Ubuntu 20.04 | ✅ | [![Ubuntu 20.04](https://github.com/noobient/ansible-cloudflare/actions/workflows/ubuntu-20.04.yml/badge.svg)](https://github.com/noobient/ansible-cloudflare/actions/workflows/ubuntu-20.04.yml) |
| Ubuntu 22.04 | ✅ | [![Ubuntu 22.04](https://github.com/noobient/ansible-cloudflare/actions/workflows/ubuntu-22.04.yml/badge.svg)](https://github.com/noobient/ansible-cloudflare/actions/workflows/ubuntu-22.04.yml) |
