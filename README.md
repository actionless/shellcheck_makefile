# shellcheck_makefile

Small utility for applying Shellcheck on Makefiles. Depends only on `shellcheck`, `make` and `python`.

```
usage: shellcheck_makefile [-h] [-s TARGET] [-l] [--shell SHELL] [-e CODE1,CODE2..] [-P SOURCEPATHS] [-x] [Makefile]

Makefile shellcheck

positional arguments:
  Makefile              path to Makefile to check

options:
  -h, --help            show this help message and exit
  -s TARGET, --skip TARGET
                        make target to skip (arg could be used multiple times)
  -l, --list            list make targets
  --shell SHELL         make shell
  -e CODE1,CODE2.., --exclude CODE1,CODE2..
                        Shellcheck: Exclude types of warnings
  -P SOURCEPATHS, --source-path SOURCEPATHS
                        Shellcheck: Specify path when looking for sourced files ("SCRIPTDIR" for script's dir)
  -x, --external-sources, --external
                        Shellcheck: allow external source-s
```
