# AWS Tools for Users

# Follow Logs Script
This script allows you to tail the logs of the most recently updated log group for an AWS Lambda function.

## Requirements

* [AWS CLI](https://aws.amazon.com/cli/)
* [bash](https://www.gnu.org/software/bash/)

## Installation

1. Clone this repository to your local machine.
2. Set the `LAMBDA_NAME` environment variable to the name of the Lambda function whose logs you want to tail. For example:

```
export LAMBDA_NAME="my-lambda-function"
```


If the `LAMBDA_NAME` environment variable is not set, the script will prompt you to enter the name of the Lambda function.

3. Make the `followlambdalog` script executable by running:


```
chmod +x followlambdalog
```


## Usage

To tail the logs of the most recently updated log group for the specified Lambda function, run:


The script will output the name of the log group with the most recent update time, and then start tailing that log group.

## License

This script is released under the [MIT License](https://opensource.org/licenses/MIT). See `LICENSE` for more information.

