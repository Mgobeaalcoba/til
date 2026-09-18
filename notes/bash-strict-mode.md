# Bash: set -euo pipefail

A common preamble for scripts:

- `-e` exits when a command fails
- `-u` treats unset variables as errors
- `-o pipefail` makes a pipeline fail if any command in it fails

`-e` has subtle exceptions (for example inside `if` conditions and `||` chains), so it is a safety net, not a guarantee.
