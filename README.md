# Spyware_Project

## KPI
We evaluate the quality of each component, and take the minimal as our KPI.
i.e., we aim to have all our components work and function, rather then pushing through with a single feature while the others can't carry on.

### Server - SRV
SRV should provide commands via an endpoint;
be accessable everywhere;
format the commands as expected by the core;
track the status of each command's proccesing;
retrieve the logs of the commands;
provide replacements for the core, runner, and SA;

### Core 
Core should be durable, i.e. keep running even if commands fail;
support a variaty of commands;
fetch commands from the server;
provide the server with data,
and in particular with insights on the state of the spyware and logs;
have modularity, i.e. low assumptions on the commands list, scripts (code, location, or encryption), input source, SA, RUNNER;
have persistancy, i.e. surving reboots, e.g. having a bootstraper;
be installed easily;

### Runner
RUNNER should run scripts;
support scripts that differ in code, location, or encryption;
have low assumptions on the SA;
run in silence;

### Storage Agent - SA
SA should provide SA functionality;
disguise the stored data;
protect the data from getting deleted;

### Spyware Utilities - SUTIL
SUTILs should provide insightful logs on the computer;
be diverse, i.e. having a lot of them;
