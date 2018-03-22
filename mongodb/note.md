
## Commands for server start/stop
```
# Start server
sudo service mongod start

# Check the mondbd process has started successfully
cat /var/log/mongodb/mongod.log | grep "initandlisten"

# Stop server
sudo service mongod stop

# Restart server
sudo service mongod restart

# Start mongo shell
mongo --host 127.0.0.1:27017
```

## Configuration
```
# Config path for mongod
/etc/mongod.conf
```
