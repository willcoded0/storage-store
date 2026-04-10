# Deploy

Deploy this site to `batserver` from your desktop with:

```bash
batdeploy-site \
  --name storage-store \
  --source /home/teao/CHAINSAW/storage-store \
  --port 8787 \
  --hostname project.batmap.win
```

This publishes the files to:

- `/srv/sites/storage-store`

And runs the site as:

- `site-storage-store.service`

Origin URL on `batserver`:

- `http://127.0.0.1:8787`

If Cloudflare Tunnel is remote-managed, add `project.batmap.win -> http://127.0.0.1:8787`
as a Public Hostname in the `batserver` tunnel from the Zero Trust dashboard.
