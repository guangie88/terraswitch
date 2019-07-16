# `terraswitch`

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
