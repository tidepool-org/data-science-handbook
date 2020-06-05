# AWS Tips

Once you've setup your AWS credentials, here are some common commands that you will find yourself doing often to access the different compute machines.

Note: Replace **USERNAME** with your assigned username (typically your first and last name combined)

## Within Local Machine

#### Adding your ssh key for use

```
ssh-add <your-ssh-key>
```

#### SSH into compute-1 machine

```
ssh -o ProxyCommand="ssh tidepool-forward@bas.ops.tidepool.org -q -W %h:%p" -A USERNAME@compute-1.analytics.private.tidepool.org
```

#### SCP from compute-1

```
scp -o ProxyCommand="ssh tidepool-forward@bas.ops.tidepool.org -q -W %h:%p" USERNAME@compute-1.analytics.private.tidepool.org:~/example_file.csv ~/Downloads/
```

#### SCP local file to compute-1

```
scp -o ProxyCommand="ssh tidepool-forward@bas.ops.tidepool.org -q -W %h:%p" ~/Downloads/example_file.csv USERNAME@compute-1.analytics.private.tidepool.org:~
```



## Within compute-1 machine

#### SCP from compute-2

```
scp compute-2.analytics.private.tidepool.org:~/example_file.csv .
```

#### SCP file to compute-2

```
scp example_file.csv compute-2.analytics.private.tidepool.org:~
```

#### SSH into compute-2 machine from compute-1

```
ssh compute-2.analytics.private.tidepool.org
```
