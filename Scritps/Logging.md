## Por qué log?  

Logs are the who, what, when, and why

Output may scroll off the screen.

Script may run unattended 

## Syslog standard
The syslog standard uses facilities and severities to categoriza messages.
	- Facilities: kern, user, mail, daemon, auth, local0, local7
	- Severities: emerg, alert, crit, err, warning, notice, info, debug
Log file locations are configurable:
	./var/log/messages
	./var/log/syslog
## Logging with logger
	- The logger utility
	- By default creates user.notice messages.
logger "Message"
logger -p local0.info "Message"
logger .t myscript -p local0.info "Message"
logger -i -t myscript "Message"

## Custom logging functions


 