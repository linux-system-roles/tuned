
# Ansible Role: tuned

An ansible role which configures tuned.

## Role Variables

**use_recommended_profile**: Set the profile which is recommended for the
machine instead of the one given in 'profile'.

**profile**: The profile to set. Unused if `use_recommended_profile` is true.
Basic profiles that are available are `balanced`, `powersave`,
`throughput-performance`, and `latency-performance`. More profiles may be
available depending on OS version.

**daemon**: If true, enable the daemon to support dynamic tuning.

**dynamic_tuning**: Enable dynamic tuning.

**sleep_interval**: Sleep interval for checking for events, in seconds.

**update_interval**: Update interval for dynamic tuning, in seconds.

**enable_recommend**: Enable recommend functionality.

**reapply_sysctl**: Wether to apply sysctl from `/etc` after tuned's sysctl are
applied.

## License

MIT

