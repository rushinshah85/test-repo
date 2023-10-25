### Background
_Why do we need this change?_
### Changes
_How does the change address the issue/feature?_
### Tests
- T1. PR Test-Please
- T2. [Canary tests](https://cerebras.atlassian.net/wiki/spaces/ENG/blog/2021/10/12/1908539575/Software+and+CS1+Regression+Hierarchy#Canaries-regressions%3A)
   - T2-1 Monolith canary "test canary" ($30.49)
   - T2-2 ws large language model stack perf "test ws-llm-perf" ($9.36), "test ws-llm-perf-evict-refill" (), "test ws_llm_ttfl" ($12.65), "test ws_stack_perf" ($11.79), "test ws_stack_perf_sdr" ($10)
   - T2-3 ml apps "test ws-ml-apps" ($18.59)
   - T2-4 ws others "test ws_runtime_p0" ($29), "test ws_simulation"($49.88), "test ws-sysemu"($11.76)
   - T2-5 Other test: kernel_canary ($4.32), stack_dashboard_short ($19.23), hostio_canary ($5.75), pytorch_canary($18), multibox_canary($9.67), multibox_canary_quick()
- T3. cs1 tests "test cs1 TRAIN_NAME=<train_name> SYSTEM=<system_name>" or use "cb_cli test-please cs1 --help" for more options
- T4. Other tests performed. Provide enough detail that they can be replicated by other developers with relevant logs.

### Commit-Message
_Add commit message here_

Jira issue: SW-XXXXXX
