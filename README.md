<a href="https://www.bernardi.cloud/">
    <img src=".readme-files/internet-check-logo-72.png" alt="Internet Check logo" title="Internet Check" align="right" height="72" />
</a>

# Internet Check
> Command line tool to receive notifications about Internet connectivity outages

[![Python](https://img.shields.io/badge/python-v3.7+-blue.svg)](https://www.python.org)
[![License](https://img.shields.io/github/license/bernarpa/internet-check.svg)](https://opensource.org/licenses/AGPL-3.0)
[![GitHub issues](https://img.shields.io/github/issues/bernarpa/internet-check.svg)](https://github.com/bernarpa/internet-check/issues)

## Table of contents

- [Why Internet Check](#why-internet-check)
- [Usage](#usage)
- [License](#license)

## Why Internet Check

Mostly because my FTTC link is working very badly from several days and TIM (Telecom Italia) is taking quite some time to restore it. Therefore, to monitor the frequent and short connection outages I ~~wisely decided to use a pre-existing tool which requires just some tweaking~~ took the occasion to write some Python code to ~~pay my daily tribute to the universal entropy~~ keep myself sharp.

## Usage

Firstly, create a `settings.py` configuration file by using `settings.py-sample` as template.

Secondly, you might want to schedule the program to run every minute with cron. For example:

    # Internet downtime check
    * * * * * /home/rnd/anaconda3/bin/python /home/rnd/github/internet-check/internet-check

The script will send an email after an Internet connection outage as soon as the link goes up again; the email will contain information about the outage timing and duration.

## License

Internet Check is licensed under the terms of the GNU Affero General Public License version 3.
