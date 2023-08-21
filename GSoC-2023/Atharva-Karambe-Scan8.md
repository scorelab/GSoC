# Scan8
## Student Info
- Name : Atharva Karambe
- Email : atharvakarambe262@gmail.com
- Profiles : [Github](https://github.com/Atharva-karambe) | [Medium](https://medium.com/@atharvakarambe262) | [LinkedIn](https://linkedin.com/in/atharva-karambe-ba77a3227/)

# Project Abstract
Scan8 is a distributed scanning system for detecting trojans, viruses, malware, and other malicious threats embedded in files. The system will allow one to submit a list of URLs or files and get the scan results in return.

The project is divided into various modules namely Dashboard, Coordinator Node, Worker Node, and Testing.
The Dashboard provides a responsive web interface for uploading files for new scans and tracking the status of all the submitted scans.
The Coordinator Node listens to updates for new scans, subsequently creating and adding scan jobs to the Redis Queue.
The Worker Node listens to updates for new jobs in Redis Queue and executes them.
The Testing module helps in maintaining the application and facilitating the CI/CD process for the same.

## [GSoC Project Page](https://summerofcode.withgoogle.com/programs/2023/organizations/score-lab)

## [GSoC Project Proposal](https://drive.google.com/file/d/1Peygk6bIy1-EqfWBx-iRVDi5JfYOeStc/view?usp=sharing)

## [GitHub Organization Repo](https://github.com/c2siorg/Scan8)

## [GitHub Personal Repo](https://github.com/Atharva-karambe/Scan8)

## [Commits during GSoC 2023](https://github.com/c2siorg/Scan8/commits/main?author=Atharva-karambe)

## [Project Demo Video](https://youtu.be/u55EvwUkNDk)

## [Project Tracker During GSoC](https://drive.google.com/file/d/15iM1QnKRXWfbXAlF5lUDcnu0HFmXhfe-/view?usp=sharing)

## GSoC Blogs
- [GSoC’22 Week 0 & 2: Early Initiations](https://medium.com/@atharvakarambe262/google-summer-of-code-2023-scan8-43ff8dd7c131)
- [GSoC’22 Week 2 & 4: Colorful Permutations](https://medium.com/@atharvakarambe262/google-summer-of-code-2023-scan8-d2560687ac09)


# Work Summary
<h3> Fixed all bugs </h3>
There were many bugs in scan8 such as the first scan getting stuck in queue due to an incorrect sequence in database update, some scans getting stuck in running status because all files are being scanned but not being updated properly, and another bug causing variable too long exception due to uploaded files having too many directories, all of which have been fixed.
<h3>Made scan result visible</h3>
I successfully addressed no scan result issue and then I fixed the code and ensured that scan results are now displayed and made visible to users.
<h3>Webcrawler</h3>
As per the instructions, I successfully developed a Webcrawler capable of scanning and extracting all links from web pages. Users can initiate a link scan directly from the frontend, and the Webcrawler efficiently crawls through the provided link, extracting not only the links present but also any scripts embedded within the page.
<h3>Proxy integration</h3>
Afterwards, I integrated a proxy into the Webcrawler class, allowing users to provide links that are only accessible through a proxy. This enhancement enables the Webcrawler to seamlessly scan and extract links from websites that require proxy access, making the link scanning process even more versatile and effective.

## Pull Requests Created
| Pull Request | Link | Linked Issues |
|---|---|---|
| BugFixed, ResultVisible and Webcrawler| [(#116)](https://github.com/c2siorg/Scan8/commit/b0fe498948557ce6098ffae38e0fa7688ede0e20) | [(#111)](https://github.com/c2siorg/Scan8/issues/111)
| Proxy added | [(#120)](https://github.com/c2siorg/Scan8/commit/7dfd3765450677d5029b7d1d586cb54a0f10e118) | [(#118)](https://github.com/c2siorg/Scan8/issues/118)



# What is Covered
- Bug fixed
- Webcrawler integration
- Proxy integration



