![stand with Ukraine](https://badgen.net/badge/stand%20with/UKRAINE/?color=0057B8&labelColor=FFD700)
[![ansible-lint](https://github.com/zerwes/checkmk_legacy2local_wrapper/actions/workflows/lint.yml/badge.svg)](https://github.com/zerwes/checkmk_legacy2local_wrapper/actions/workflows/lint.yml)

# checkmk_legacy2local_wrapper
**ansible playbook to distribute wrapper scripts in order to use legacy nagios checks as checkmk local checks**

With [checkmk](https://docs.checkmk.com), you can still use good old nagios plugins via [mrpe](https://docs.checkmk.com/latest/en/agent_linux.html#mrpe).
These checks will be executed synchronously and sequentially.
So especially if you have many legacy checks, it makes sense to migrate them to [local checks](https://docs.checkmk.com/latest/en/localchecks.html).
As the output of the legacy checks differs from the syntax expected by checkmk from local checks, this needs to be reformated.
Here are some sample scripts and a ansible playbook to generate and distribute them in e flexible way.
