# DNS-Command-Line-Tool

## Student Information

* Name - Vinuri Bandara
* Email - vinugayanthika@gmail.com
* GitHub Profile - https://github.com/VinuriBandara
* Medium - https://medium.com/@vinugayanthika
* Twitter - []()

# Project Abstract

DNSTool-CLI is an extension of the DNSTool, which is designed to monitor the given set of internet resources like domains, IP, SOA, etc. DNSTool-CLI allows the user to download the DNS scan feed(s) automatically by integrating the CLI to their corn jobs or Airflow automation. This project is to develop high throughput and low latency data transferring pipeline with authentication for transferring the data from the system’s file store to the consumer environment.

<div align="center">
    <a href="https://drive.google.com/uc?export=view&id=1mqz8ZL-7_ja3Z8dwKhhDqwtoqyMUtpL_"><img src="https://drive.google.com/uc?export=view&id=1mqz8ZL-7_ja3Z8dwKhhDqwtoqyMUtpL_" style="max-width: 100%; height: auto;" title="Click to enlarge picture"></a>
</div>

## [GSoC Project Page](https://summerofcode.withgoogle.com/dashboard/project/5429085385261056/overview/)

## [GSoC Project Proposal](https://drive.google.com/file/d/1YKg8H9WLDI2fyt6AXpV8xxB9bchcnmx6/view?usp=sharing)

## [GitHub Organization Repo](https://github.com/scorelab/DNS-Command-Line-Tool)

## [GitHub Personal Repo](https://github.com/VinuriBandara/DNS-Command-Line-Tool)

## [Commits during GSoC 2021](https://github.com/scorelab/DNS-Command-Line-Tool/pulls?q=is%3Apr+is%3Aclosed)

## [Project Demo Video](https://drive.google.com/file/d/1iqgdKL61aG-_veFg6mWb-wQ2-W9CuBqN/view?usp=sharing)

## [Project Wiki](https://github.com/scorelab/DNS-Command-Line-Tool#readme)

## [GSoC Blog](https://medium.com/scorelab/my-gsoc-2021-journey-with-score-lab-516353dea893?source=friends_link&sk=7f1797e3551fd55879d0f2f5abd59b24)

# Work Summary

For GSoC 2021, in the first coding phase i focused on communicating with my mentors and the fellow developer in order to build the initial plan for the DNSIP-CommandLine tool. Moving onto the coding i mainly focused on creating a command line tool which fulfills the necessary requests by a user. The implementation was carried out using python argparse, GCS queries, Google authentication and apschedulers. 

The current version of the command line tool can be found on PyPI under [DNS-Command-Line-Tool](https://pypi.org/project/DNS-Command-Line-Tool/) and can be installed for using. After installing the users can query the dataset as follows.

 ```
 usage: dnsip [-h] [--size] [--list] [--download file_to_download] [--download_bucket Local_location_of_files]
             [--schedule Local_location_of_files]

Check, download and update the local DNS IP dataset location.

optional arguments:
  -h, --help            show this help message and exit
  --size                The size of the downloadable blob
  --list                List the available data for downloading
  --download file_to_download
                        Download a single file
  --download_bucket Local_location_of_files
                        One-time download of the complete DNSIP dataset
  --schedule Local_location_of_files
                        Update the DNSIP dataset every 24 hours
                        
```

All the implementations and the learning process is included in the my medium blog [My GSoC 2021 journey with SCoRe Lab](https://medium.com/scorelab/my-gsoc-2021-journey-with-score-lab-516353dea893?source=friends_link&sk=7f1797e3551fd55879d0f2f5abd59b24)

# What's Covered

Using the command line tool users can query the database stored in GCS. The list of services it provides is as follows.

* Authenticate and access the Google Cloud Storage through a service account
* Check the size of the downloadable dataset
* List the downloadbale files - Using this the users can select one file to download if that's what they require
* Check when the files were last updates - Using this the users can check if the file they are currently utilzing to planning to utilize has been updated since the last download
* Downloading the complete dataset once
* Update the dataset every 24 hours - Users can run this query in the background and update the files, this will delete the non-existing files in the GCS that exists in the local directory.

# What's left

* Implementing more advanced queries.
* Writing a proper documentation after the complete implementation. 

### Reference
1. [argparse](https://docs.python.org/3/library/argparse.html)
2. [Cloud Storage authentication](https://cloud.google.com/storage/docs/authentication)
3. [Google Cloud Storage - Blobs / Objects](https://googleapis.dev/python/storage/latest/blobs.html)
