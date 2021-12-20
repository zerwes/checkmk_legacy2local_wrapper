# checkmk_legacy2local_wrapper
wrapper scripts in order to use legacy nagios checks as checkmk local checks

With [checkmk](https://docs.checkmk.com), you can still use good old nagios plugins via [mrpe](https://docs.checkmk.com/latest/en/agent_linux.html#mrpe).
These checks will be executed synchronously and sequentially.
So especially if you have many legacy checks, it makes sense to migrate them to [local checks](https://docs.checkmk.com/latest/en/localchecks.html).
Here are some sample scripts and a ansible playbook to generate and distribute them in e flexible way.
