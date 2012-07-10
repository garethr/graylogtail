Script inspired by logster that takes a log file and sends all output
periodically to a Graylog2 server via running on cron.

    Usage: graylogtail [options] logfile

    Tail a log file and filter each line to generate log lines that can be sent to
    gralog2.

    Options:
      -h, --help            show this help message and exit
      -s STATE_DIR, --state-dir=STATE_DIR
                            Where to store the logtail state file.  Default
                            location /var/run
      -d, --dry-run         Parse the log file but send stats to standard output.
      --graylog-host=GRAYLOG_HOST
                            Hostname for Graylog, e.g. graylog.example.com
      --graylog-port=GRAYLOG_PORT
                            Hostname for Graylog, e.g. graylog.example.com
      --facility=FACILITY   Facility for filtering messages in graylog
      -D, --debug           Provide more verbose logging for debugging.
      --level=LEVEL         Specify the level messages should be logged at.
                            Default to info
