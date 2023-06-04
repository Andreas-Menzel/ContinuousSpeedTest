# InternetSpeedLogger

## Python Script for Testing the Speed of your Internet Connection

This Python script periodically tests the internet speed of your network and
logs the results in a CSV file. It uses the
[speedtest-cli](https://pypi.org/project/speedtest-cli/) library to measure
internet speed. You can control the frequency of testing and duration of the
entire test run via the script's parameters.

## Installation

Just install using pip:

```bash
pip install InternetSpeedLogger
```

## Usage

If you installed InternetSpeedLogger with pip, you should be able to simply
execute the script from anywhere:

```bash
InternetSpeedLogger
```

Type `InternetSpeedLogger --help` to get detailed execution information:

```
usage: InternetSpeedLogger [-h] [--version] [-i INTERVAL] [-d DURATION] [-l LOG_FILE]

A Python script that continuously monitors and logs your internet
speed. It tests both download and upload speeds at regular intervals
and records the data in a CSV file for easy analysis and tracking.
Ideal for auditing your network performance or ISP reliability over
time.
            

options:
  -h, --help            show this help message and exit
  --version             show program's version number and exit
  -i INTERVAL, --interval INTERVAL
                        Testing interval in seconds. Make sure that the interval is not shorter than the time needed for testing. (default: 60)
  -d DURATION, --duration DURATION
                        Duration of the entire test runs. The script will automatically end after this duration. Set to <= 0 for infinite. (default: 0)
  -l LOG_FILE, --log_file LOG_FILE
                        Filename for the log-file. NOTE: A similar filename will be chosen if a file with this name already exists.

Default location of the log-file:
    A .csv-file will be created, which will contain all logged information.
    Default Filename: "YYYY-MM-DD_HH:MM:SS_internet_speeds.csv"
    Default Location: <tmp_dir>/InternetSpeedLogger/
        <tmp_dir> on Windows: C:\TEMP, C:\TMP, \TEMP, or \TMP, in that order
        <tmp_dir> on all other: /tmp, /var/tmp, or /usr/tmp, in that order
```

## Contribution

We warmly welcome contributions to the InternetSpeedLogger project! Your ideas
and work can make a real difference to its development.

There are many ways to contribute:

- **Bug Reports:** If you encounter any issues with the script, please create a
  new issue in the GitHub repository. Be as detailed as possible, including
  steps to reproduce the bug, the Python version you're using, and any error
  messages you've received.
- **Feature Requests:** Have a great idea for improving InternetSpeedLogger?
  We'd love to hear about it! You can propose new features by opening a new
  issue and using the Feature Request template.
- **Code Contributions:** If you are keen to get hands-on and directly
  contribute to the InternetSpeedDataLogger codebase, we enthusiastically
  welcome your input. Your efforts can help to fix bugs, add features, improve
  efficiency, and generally make the tool more robust and user-friendly.
- **Documentation:** A project is only as good as its documentation. If you can
  improve the readme, comment the code more thoroughly, or create better user
  guides, your contributions are welcome.

Remember, the best way to make successful contributions is to communicate! Feel
free to ask questions and discuss your ideas in the issue tracker.

In your pull request, provide a clear and comprehensive explanation of your
changes and their necessity. This will help us understand the purpose of your
contribution and expedite the review process.

Thank you for your interest in improving InternetSpeedLogger! :heart:

## License

This script is released under the MIT License.
