# Using bridges with oniux

The following guide will explain on how to use obfs4 bridges with oniux.

Please refer to the Arti documentation for more sophisticated use of bridges.
This is just a short summary.

1. Install `oniux` v0.7.0 or newer.
2. Install `obfs4proxy`, probably from your distribution repository.
3. Create a configuration file with the following content:
```toml
[bridges]
enabled = "auto"
bridges = [
  # These are just examples, and will not work!
  # Obtain real bridgelines from:
  # https://bridges.torproject.org/bridges?transport=obfs4
  "Bridge 192.0.2.66:443 8C00000DFE0046ABCDFAD191144399CB520C29E8",
  "Bridge 192.0.2.78:9001 6078000DFE0046ABCDFAD191144399CB52FFFFF8",
]

[[bridges.transports]]
protocols = ["obfs4"]
path = "/usr/bin/obfs4proxy"
arguments = []
run_on_startup = true
```
4. Launch oniux as follows:
```sh
oniux -c /path/to/the/config.toml <CMD>
```
5. Enjoy access to the internet!
