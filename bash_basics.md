
``` s
sed -i -e 's/3\.13/3\.14/g' /etc/apk/repositories

python3-dev py3-pip gcc libffi-dev g++ libxml2-dev libxslt-dev

if [ "$CS_ISSUE_REPORTING_DISABLED" == "FALSE" ] || [ "$ISSUES_REPORTING_ENABLE" == "TRUE" ] ; then post_issues ; fi

DYNAMIC_ENVIRONMENT_URL=$(gitlab-terraform show | grep link | tail -n 1 | cut -d '"' -f 2)


```

## Traverse through folders


``` s
<command-1> || <this command runs if command-1 fails>
<command-1> && <runs reguardless if command-1 failed or not>
<directory-1> : <directory-2> : <directory-3>
$<variable>
$(<command>)
<file> >> <append this to file>

```

- `:` is seperator
- `#!` tells kernal to look for interpreter (bash | sh)
- `#!/bin/bash` kernal will use bash interpreter to run script following this command
- `$PATH`
- `.` refers to current directory
- `^` 
- `=~` performs regular expression match
- `grep` searches the given files for lines containing a match to a given pattern list. (example pattern list:)
- `sed` short for stream editor, performs editing operations on text coming from standard input or a file.

``` bash
for docker_dir in *; do if ! [ -f $docker_dir ]; then echo $docker_dir;  cd $docker_dir; hadolint --failure-threshold warning Dockerfile || FAILURE_COUNT=$((FAILURE_COUNT+1)); cd ..; fi; done;
```
- `-f` 
- `||`
- `!` 




```bash
    - |-
      if [ "$DS_IGNORE_DEV_DEPENDENCY" == "TRUE" ] ; then
        apk add jq;
        jq 'del(.devDependencies)' package.json > tmp.package.json;
        mv tmp.package.json package.json;
      fi;
```
