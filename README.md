
RPZ
===

### 280blocker
```bash
curl -o - "https://280blocker.net/files/280blocker_domain_$(date "+%Y%m").txt" | tr -cd "\0-\177" | tr -d "\r" | awk '/^[a-zA-Z0-9]/{print $1 " CNAME ."}' > 280blocker.rp
```
