# noobient.cloudflare

## Synopsys

This role creates the `cloudflare` zone in firewalld that passes `https` traffic
between the host and Cloudflare's servers as described on their
[IP Ranges](https://www.cloudflare.com/ips/) page.

## Parameters

| Name | Required | Example | Description |
|---|---|---|---|
| `mode` | yes | `https` | Either `https` or `tunnel`. In `https`, incoming HTTPS traffic is only allowed from CF IP addresses. In `tunnel` mode, you shall ensure the node does not have public IP addresses at all. In this case, HTTPS traffic is going through CF Tunnel, while others like SSH must be set up using CF WARP. |
| `token` | no | `foo123` | Cloudflare token. Mandatory if in `tunnel` mode, ignored otherwise. |

## Examples

```yml
- include_role:
    name: noobient.cloudflare
    mode: tunnel
    token: foo123
```

## Return Values

N/A

## Support

| Platform | Support | Status |
|---|---|---|
| Linter | ✅ | [![Lint](https://github.com/noobient/ansible-galaxy-cloudflare/actions/workflows/lint.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-cloudflare/actions/workflows/lint.yml) |
| AlmaLinux 8 | ✅ | [![AlmaLinux 8](https://github.com/noobient/ansible-galaxy-cloudflare/actions/workflows/almalinux-8.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-cloudflare/actions/workflows/almalinux-8.yml) |
| AlmaLinux 9 | ✅ | [![AlmaLinux 9](https://github.com/noobient/ansible-galaxy-cloudflare/actions/workflows/almalinux-9.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-cloudflare/actions/workflows/almalinux-9.yml) |
| Fedora 38 | ✅ | [![Fedora 38](https://github.com/noobient/ansible-galaxy-cloudflare/actions/workflows/fedora-38.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-cloudflare/actions/workflows/fedora-38.yml) |
| Fedora 39 | ✅ | [![Fedora 39](https://github.com/noobient/ansible-galaxy-cloudflare/actions/workflows/fedora-39.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-cloudflare/actions/workflows/fedora-39.yml) |
| Ubuntu 18.04 | ✅ | [![Ubuntu 18.04](https://github.com/noobient/ansible-galaxy-cloudflare/actions/workflows/ubuntu-18.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-cloudflare/actions/workflows/ubuntu-18.04.yml) |
| Ubuntu 20.04 | ✅ | [![Ubuntu 20.04](https://github.com/noobient/ansible-galaxy-cloudflare/actions/workflows/ubuntu-20.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-cloudflare/actions/workflows/ubuntu-20.04.yml) |
| Ubuntu 22.04 | ✅ | [![Ubuntu 22.04](https://github.com/noobient/ansible-galaxy-cloudflare/actions/workflows/ubuntu-22.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-cloudflare/actions/workflows/ubuntu-22.04.yml) |
