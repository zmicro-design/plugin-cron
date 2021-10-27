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

### Example

```bash
# echo date at every minute
$ zmicro plugin run cron create echo_date _/1 _ _ _ _ date +%D\ %H:%M:%S

# update at 10:00 on every day-of-month
$ zmicro plugin run cron create zmicro_auto_update 0 10 _/1 _ _ zmicro update -a
```

