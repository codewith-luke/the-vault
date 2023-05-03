## Disk Usage

Shows metrics for our usage metrics

```sh
df -h
```

## Restart a service and check status of a service

```sh
systemctl restart {service}
systemctl status {service}
```

## Install Ping

```sh
apt-get update && apt-get install iputils-ping
```

### Update Snap store

```shell
killall snap-store
sudo snap refresh snap-store
```

# Reading data from a file and manipulating output

```bash
$(cat apps/distributor/package.json | grep version | head -1 | awk -F: '{ print $2 }' | sed 's/[\",]//g' | tr -d '[[:space:]]')
```

1) `cat apps/distributor/package.json`: This command reads the content of the package.json file located in the apps/distributor directory and outputs it to the pipeline.

2) `grep version`: This command filters the output from the previous command and keeps only the lines containing the word "version". In this case, it should return the line containing the version number in the package.json file.

3) `head -1`: This command takes the first line from the output of the previous command. It's used here to ensure that only one line is passed to the next command in the pipeline. In this case, it's helpful in case there are multiple lines containing the word "version" in the package.json file.

4) `awk -F: '{ print $2 }'`: This command splits each input line into fields using the colon : as a delimiter, and then prints the second field (the version number). In the package.json file, the version line usually looks like "version": "1.0.0", so the second field would be "1.0.0".

4) `sed 's/[\",]//g'`: This command uses sed (stream editor) to remove all occurrences of double quotes " and commas , from the version number. It replaces the matched characters with an empty string (i.e., it removes them).

6) `tr -d '[[:space:]]'`: This command uses tr (translate) to delete all whitespace characters (spaces, tabs, and newlines) from the output. It ensures that the version number does not contain any leading or trailing spaces.