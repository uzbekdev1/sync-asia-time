# Sync Windows Net Time

net stop w32time
w32tm /unregister
w32tm /register
net start w32time
tzutil /s "West Asia Standard Time"
w32tm  /resync /force
