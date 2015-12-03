Simple docker container to generate btsync keys for various usages.

Utilizes sciurius' btsync-keygen [perl script](https://gist.github.com/sciurius/787e99af74132b62b397)

Usage:

```bash
docker run -it --rm aevumdecessus/btsync-keygen
```

Example Output (Don't use these keys as they are public)
```
~/docker/bt-keygen: docker run -it aevumdecessus/btsync-keygen
    // RW, normal  AE4F7ZVELX7ED3CHB34PDMCFFI4MHDOTZ
    // RO, normal  BNP3V5LRJT5IMMJ3VCFBLBUA5TZSN5DW7
    // RW, encrypt DE4F7ZVELX7ED3CHB34PDMCFFI4MHDOTZ
    // RO, decrypt EXGGYBAIPIJEMDPOLJN6NCFAVEPASIRBYZBDKCEFANPBVT5ON5UPJ3467CA
    // RO, secret  FXGGYBAIPIJEMDPOLJN6NCFAVEPASIRBY
    {
      "secret"           : "AE4F7ZVELX7ED3CHB34PDMCFFI4MHDOTZ",
      "dir"              : "/",
      "use_relay_server" : false,
      "use_tracker"      : false,
      "use_dht"          : false,
      "search_lan"       : true,
      "use_sync_trash"   : true,
      "known_hosts"      :
      [
	"192.168.1.16:58291"
      ]
    },
```
