# InternetSpeedLogger

## Python Script for Testing the Speed of your Internet Connection

This Python script periodically tests the internet speed of your network and
logs the results in a CSV file. It uses the
[speedtest-cli](https://pypi.org/project/speedtest-cli/) library to measure
internet speed. You can control the frequency of testing and duration of the
entire test run via the script's parameters.

## Dependencies

The script relies on the
[speedtest-cli](https://pypi.org/project/speedtest-cli/) library to measure the
internet speed.

If you are installing InternetSpeedLogger manually, make sure that you have
already installed all requirements:

```bash
pip install -r requirements.txt
```

## Usage

Simply run the script using Python 3:

```bash
python3 InternetSpeedTest.py
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

Thank you for your interest in improving InternetSpeedDataLogger! :heart:

## License

This script is released under the MIT License.
