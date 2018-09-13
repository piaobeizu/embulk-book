## embulk的命令通览

>embulk命令实现





> 全部命令

**用法: embulk [-vm-options] <command> [--options]**

**Commands:**

```shell
mkbundle   <directory>         # create a new plugin bundle environment.

bundle     [directory]         # update a plugin bundle environment.

run        <config.yml>        # run a bulk load transaction.

cleanup    <config.yml>        # cleanup resume state.

preview    <config.yml>        # dry-run the bulk load without output and show preview.

guess      <partial-config.yml> -o <output.yml>    # guess missing parameters to create a complete configuration file.

gem        <install | list | help>    # install a plugin or show installed plugins.

new        <category> <name>          # generates new plugin template

migrate    <path>          # modify plugin code to use the latest Embulk plugin API

example    [path]          # creates an example config file and csv file to try embulk.

selfupdate [version]       # upgrades embulk to the latest released version or to the specified version.

VM options:

-E...              Run an external script to configure environment variables in JVM
(Operations not just setting envs are not recommended nor guaranteed. Expect side effects by running your external script at your own risk.)

-J-O               Disable JVM optimizations to speed up startup time (enabled by default if command is 'run')

-J+O               Enable JVM optimizations to speed up throughput

-J...              Set JVM options (use -J-help to see available options)

-R...              Set JRuby options (use -R--help to see available options)

```



