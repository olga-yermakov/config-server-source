# config-server-source

The configuration source for changing the logging level using the config server.

Usage
-----

If you want to add a properties file, do it in the following tree structure: </br>
[app_name]/[environment]/[app_name]-[profile].properties </br>
for example, if you want a config file for csam, in aws DC with profile staging, you'll get the following file: </br>
csam/aws/csam-staging.properties </br>

in the properties file you can add a logback logging configuration as follows: </br>
logging.level.[logger_name]=[log_level] </br>

for example: </br>
logging.level.root=debug </br>
