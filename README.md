# ContinuousSpeedTest

## Python Script for Testing the Speed of your Internet Connection

This Python script periodically tests the internet speed of your network and
logs the results in a CSV file. It uses the
[speedtest-cli](https://pypi.org/project/speedtest-cli/) library to measure
internet speed. You can control the frequency of testing and duration of the
entire test run via the script's parameters.

## Dependencies

The script relies on the following Python libraries:

- csv
- datetime
- signal
- speedtest-cli
- time

Install the speedtest-cli library using pip:

```bash
pip install speedtest-cli
```

## Usage

Simply run the script using Python 3:

```bash
python3 speedtest.py
```

You can configure the script by modifying the following variables:

- **interval_in_secs**: The frequency of testing in seconds. Make sure that the
  interval is not shorter than the time needed for a single test.
- **testing_duration_secs**: The total duration of the test run in seconds. The
  script will automatically terminate after this duration. Set it to `<= 0` for
  an infinite duration.
- **csv_file**: The filename of the CSV file in which the test results will be
  logged.

## Contribution

If you want to contribute, feel free to make a pull request.

## License

This script is released under the MIT License.
