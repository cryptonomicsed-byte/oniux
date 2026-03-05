# oniux 0.9.0 - 05 March 2026

* Update various dependencies, including Arti 2.1.0.
* Share smoltcp version with onionmasq.
* Use 1.89 as the MSRV and decide upon an MSRV policy.
* Document the release process.

# oniux 0.8.1 - 08 February 2026

* Emergency fix for failing unprivileged user namespace clone on mainline
  Linux systems.
* Update various dependencies.

# oniux 0.8.0 - 03 February 2026

* Update various dependencies, including Arti 2.0.0.
    * Arti 2.0 has a breaking configuration syntax change, meaning that your
      Arti configuration may need updates.
* Log errors by default.
* Improve checks for availability of user namespaces.
* Improve internal error handling.
* Refactor FD send/recv logic.
* Log the unlikely death of an onion-tunnel.
* Refactor IPC sync logic for readiness.
* Update example in README

# oniux 0.7.0 - 14 January 2026

* Update various dependencies, including Arti 1.9.0.
* Support for Arti configurations using `-c`, which includes the possibility
  to use bridges with oniux.
* Use `localhost:9050` in the `ALL_PROXY` environment variable now.
    * Fixes a bug where one could not resolve addresses using curl.
* Implement logging using `tracing` and adding `-l` for setting a log level.
    * This deprecates the `RUST_LOG` environment variable.
* Add an example for anticenorship using `-c`.

# oniux 0.6.1 - 04 September 2025

* Updates various crates to their newest, this most notably includes Arti 1.5.0
  and the related crates.

# oniux 0.6.0 - 29 July 2025

* Improvements in error logging.
* Check for the TUN kernel module on startup.
* Enable release time optimizations.
* Implement support for SOCKS in a proper way.
* Check for `sysctl kernel.unprivileged_userns_clone=1` on startup.
* Updated various dependencies to their newest version.
* Various internal improvements in the codebase.

# oniux 0.5.0 - 22 May 2025

* Compile using the default toolchain.
* Don't panic when failing to spawn command.
* Use more explicit errors for common failures.
* Setup loopback device.
* Update dependencies.

# oniux 0.4.0 - 05 May 2025

* oniux now runs without capabilities.

# oniux 0.3.0 - 28 April 2025

* Bugfix related to the mounting of filesystems.

# oniux 0.2.0 - 27 March 2025

* onionmasq binary is no longer required.
* `/proc` is mounted automatically.
* Arguments are parsed before the PID and mount namespaces are created.
* Several cleanups in the codebase.

# oniux 0.1.0 - 27 February 2025

Initial release of oniux.
