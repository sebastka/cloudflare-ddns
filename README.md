# cloudflare-ddns

Update DNS record on Cloudflare's nameserver using their API.

Set up `.env` files for every record to update:
```bash
$ cp www.domain.tld.env.example www.karlsen.fr.env
$ vi www.karlsen.fr.env
```

## dhclient exit hook

```bash
$ ln -s /path/to/script/cloudflare-ddns/cloudflare-ddns /etc/dhcp/dhclient-exit-hooks.d/
```
