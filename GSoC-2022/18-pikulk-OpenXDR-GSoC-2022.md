# OpenXDR GSoC 2022

## Project Abstract
Detection time and response time are the major critical accepts of all detection and response systems. Considering the vast amount of system logs collectors, network logs collectors and external IOC systems bring vast amounts of data to process within a short amount of time and uncover the anomalies. Although this process should not be flooded with false positive alerts which we identified as alert fatigue. Considering processing vast amounts of boundless stream data and doing a less false positive detection rate is a system engineering challenge that should stand side by side with cybersecurity expert knowledge. Building state of the art systems required several major components divisions. There are Data Sources (IDS, sys logs, net logs, firewall logs, files) , External intelligence (IOC, SIEM), Processing and detection unit(s) (batch or streaming processing, deployed ML/DL models) , Data storages (databases, flat files, object storages) and visualizations (index, dashboards). Recreating each of above divisions are equivalent to reinventing the wheel, therefore openXDR focuses intergaterabiltiy to work with available tools out there which leads users to use existing systems without hassle but with the power of detection and response time of openXDR. In general, it seamlessly integrates with any EDR, NDR, SIEM, or IDS through a modular integrated architecture.

### [GSoC Project Page](https://summerofcode.withgoogle.com/programs/2022/projects/B7KUMyWw)

### [GSoC Project Proposal](https://drive.google.com/file/d/1PJwZzdWDxqEuZg6WnjLX5uggoV-HDSkr/view?usp=drivesdk)

### [GitHub Organization Repo](https://github.com/scorelab/OpenXDR)

### [GitHub Personal Repo](https://github.com/piumalkulasekara/OpenXDR)

### [Commits during GSoC 2022](https://github.com/piumalkulasekara/OpenXDR/commits/node)

### [Project Demo Video](https://drive.google.com/file/d/1yG3OsZtywoqR5JWnnAvpp81tNCCuo7co/view?usp=drivesdk)

### [GSoC Blog](https://medium.com/scorelab/gsoc-2022-with-score-lab-2c0994907650)

## Work Summary And What Covered

* Create few data collecting probes (EDR, NDR, ISD, SIEM one for each)
* Create Flink stateful stream processing modules
* Create a DB to retrieve processed historical data using mysql.

## What left
* Create automatically setup scripts and create an interface to intergate with other datastores
