# ZMicro Cron Plugin

### Usage

```bash
# create a cron service
$ zcron create

? cron service name: date
? service command: date
? service schedule(crontab.guru, use _ instead of *): _/1 _ _ _ _

# remove a cron service
$ zcron remove date

# enable a cron service
$ zcron enable date

# disable a cron service
$ zcron disable date

# get a cron service log
$ zcron logs date

# get a cron service status
$ zcron status date
```

