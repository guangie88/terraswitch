# `terraswitch`

[![Codefresh build status]( https://g.codefresh.io/api/badges/pipeline/guangie88/guangie88%2Fterraswitch%2Fterraswitch?key=eyJhbGciOiJIUzI1NiJ9.NWM4MjcyMzg3Y2NkOTUzZTcxM2RiMjRl.cTJ8XB8rM4mRl2LmZBHaIVZ92MxdGgb7Mmib1jt8o4E&type=cf-1)]( https://g.codefresh.io/pipelines/terraswitch/builds?filter=trigger:build~Build;pipeline:5d2d21a5a1d4a99add2d614c~terraswitch)

Contains script to download and switch between terraform 0.11 and 0.12. Also
fetches for corresponding compatible `terragrunt` binary.

You may run the script via curl like this, for example, to switch between
`v0.11` and `v0.12`:

```bash
curl -sL https://raw.githubusercontent.com/guangie88/terraswitch/master/terraswitch | sudo bash /dev/stdin 0.11
curl -sL https://raw.githubusercontent.com/guangie88/terraswitch/master/terraswitch | sudo bash /dev/stdin 0.12
```

This assumes that `/usr/local/bin` to be the binary holding directory, which you
might need to run the script with `sudo` in order to save the binaries into. If
you wish to use a different directory, override `BIN_DIR` to the directory path
that you wish to save into.
