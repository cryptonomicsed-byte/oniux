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
