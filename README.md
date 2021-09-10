# smartmet-base-international

Install and maintain SmartMet server enviroment.

Based on https://github.com/fmidev/smartmet-base-international

## Running it:
`ansible-playbook --inventory inventories/production/hosts.yml --user=root install-production-server.yml`

Add host server(s) to `inventories{production/development}/host.yml`

Note: the `--list-hosts`-argument can be used to first check what command would do. Actual operation is fully run without it.

Add `--connection=paramiko` if you are running the command on macOS.

Add `--check` to prevent any real changes; instead, try to predict some of the changes that may occur