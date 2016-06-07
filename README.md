# Anomaly Detection Engine for Linux Logs (ADE)

ADE can process a large numbers of logs from a large number of Linux systems to
create a compact summary of those logs. The summary identifies and
consolidates similar text strings into a single message example and assigns it
a key (message id). &nbsp;The summary determines if &nbsp;the
message id are being issued when expected, are being issued at the expected
rate during a time slice, and how often during the day are the message
or a similar message (same message id) issued.<br>

You can use those results to examine 

- A set of logs to find anomalies which may be
helpful when attempting to find
the root cause of a problem or incident
- The currently generated logs to find anomalies which may be
helpful when attempting to find the cause of an on-going problem or incident


Please see http://openmainframeproject.github.io/ade/ for documentation on ADE.

## Releases

### Initial release 1.0.0

- Parsing of Linux Logs in RFC5424 and RFC3164 format
- Splitting logs into time slices
- Handling wrapper messages
- Statistical analysis of logs
- Creates output 

### Esopus Creek 1.0.1

- Support for MariaDB(TM)
- Verify script - determine if sufficient messages are available to create a valid model
- Multiple SonarQube(TM) issues fixed
- Wiki article Hints on how to update XSLT - tailor the output shown in a browser to problem