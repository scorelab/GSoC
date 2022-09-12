# SCoRe Lab: OpenMF Analytics API and UI Development

<p align="center">
<img src="https://summerofcode.withgoogle.com/assets/media/gsoc-2022-badge.svg" height=300px>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://raw.githubusercontent.com/scorelab/OpenMF/master/Logo.png" width=300px> 
</p>

# Contributor Info

<div container>
<table>

<tr width="560px">
<td width="400px">
 Name - Prerak Mathur<br>
 User Name - PrerakMathur20<br>
 Email - mathur.prerak@gmail.com<br>
GitHub Profile - <a href="https://github.com/PrerakMathur20">PrerakMathur20 </a><br>
 Medium - <a href="https://medium.com/@prerakmathur">@prerakmathur </a><br>
 Twitter - <a href="https://twitter.com/pm_hai_hum">@pm_hai_hum</a><br>
  Linkedin - <a href="https://www.linkedin.com/in/PrerakMathur20">Prerak Mathur</a><br>
</td>
<td width="260px">
<a href="https://github.com/PrerakMathur20"><img src="https://avatars.githubusercontent.com/u/76054330?v=4" height="260px" width="260px;" alt=""/></a>
</td>
</tr>
</table>
</div>

# Project Abstract

OpenMF is an open-source forensic tool for Android smartphones that helps digital forensic investigators throughout the life cycle of digital forensic investigation. It is a collection of tools that can be used to extract and analyze data from Android smartphones. It is a part of the SCoRe Lab. The project aims to develop an analytics API and UI for OpenMF. The analytics API will be used to extract and analyze data from Android smartphones. The analytics UI will be used to visualize the data extracted from the smartphones. The project will be developed using Python and JavaScript.

## [GSoC Project Page](https://summerofcode.withgoogle.com/programs/2022/projects/gnn8Hro3)

## [GSoC Project Proposal](https://github.com/PrerakMathur20/OpenMF/blob/Proposal/PrerakProposalOpenMF.pdf)

## [GitHub Organization Repo](https://github.com/scorelab/openmf)

## [GitHub Personal Repo](https://github.com/PrerakMathur20/openmf)

## [Commits during GSoC 2022](https://github.com/scorelab/OpenMF/commits?author=PrerakMathur20)

## [Project Demo Video](https://youtube.com/playlist?list=PLA0bgXZugdjcxcn3kprNTW9LvzaAyvUAV)

## [Project Wiki](https://github.com/scorelab/OpenMF/wiki)

<!-- ## [GSoC Blog](http://GSoCBlog) -->

# Work Summary

OpenMF is an open-source forensic solution for Android smartphones that assists digital forensic investigators throughout the investigation life cycle. The purpose is to enhance the user experience and expedite a new user's understanding of the software. Since the conclusion of the Google Summer of Code 2022, OpenMF has completed numerous unfinished frontend and backend functionalities. Multiple new features have been added to improve the user experience and facilitate better management and control. Below is a summary of all the software additions. [Here](https://github.com/scorelab/OpenMF/wiki), you can also find the project's wiki and additional information.

# Work Covered

The following are the major features that have been added to OpenMF:

- Authentication with Google OAuth for
  - Admin
  - Management
  - Extractor
- Missing Routes and Pages added such as -
  - Home (Hover)
  - Login
  - Register
  - Contact
  - About
- Allow Admin to Create new Management and Extractor users with Google OAuth
- Added the incomplete functionality to mark tasks as completed
- Added the incomplete functionality in Sidebar for -
  - Search User
  - Download list of Users and their details in `.csv` and `.pdf` format
  - Sort and Filter by details and Columns
  - Abstract the data in the table to show only the required details
- Created pages and modals on **Pre-Declared** Routes for -
  - Home and About Page to display information about the Software itself.
  - Login and Register page to be replaced by Login Modal with Google OAuth
  - Contact Page created to contact the Admin and Management
- Created a Profile Card component for the User to view their details
- Created **Dashboard** for all Users which displays -
  - The Current User's Details
  - If Admin, list of all Management and Extractor Users' Tasks and their details
  - If Extractor or Management, list of all the Tasks assigned to the User and their details
- Enabled the feature to Locally Open routes in generated in Management's Analytics Page's Filter and Keyword Search.
- Removed Irrelevant Profile Route and Page from Navbar
- Fixed the issue of the Navbar showing the wrong User's Options on specific tabs
- Created End-routes, Frontend and API to Edit the following details of the User -
  - Task Title
  - Task Descreption
  - Task Status
  - Task Due Date
- Added Fucntionality to download Case Tree and its details in the following formats-
  - `.xml`
  - `.json`

# Demo

- [Register Google OAuth (Admin)](https://youtu.be/L63swPPCTfg)
- [Adding New members ad Admin (Management and Extractor)](https://youtu.be/gxPdERIyvTg)
- [Search User](https://youtu.be/b1vBGXvVZns)
- [Update Tasks](https://youtu.be/kwehTiXTlAs)
- [Open Case File Routes Locally](https://youtu.be/2ufhgqsFv9k)

# What left

Add a more data visualizations to the Analytics Page, and show the data extracted in the form of table and graphs and from the extrcated data, implement OCR to extract text, Add Data classification cases for _WhatsApp_ and _Facebook_.
Implement the entire project in iOS environmet.

# Issues Opened and Linked PRs
For more details and information on Issues Opened and their respective, please refer the table and linkes below.

<table>
<tr>
<th>Issue Number</th>
<th>Issue</th>
<th>PR Number</th>
<th>PR</th>
</tr>

<tr>
<td><a href="https://github.com/scorelab/OpenMF/issues/265" target="_blank">#265</a></td>
<td>[Backend] Auth Required </td>
<td><a href="https://github.com/scorelab/OpenMF/pull/279" target="_blank">#279</a></td>
<td>Google Auth Implemented</td>
</tr>

<tr>
<td><a href="https://github.com/scorelab/OpenMF/issues/280" target="_blank">#280</a></td>
<td>[Frontend]Finish Incomplete Pages and Routes Links </td>
<td><a href="https://github.com/scorelab/OpenMF/pull/289" target="_blank">#289</a></td>
<td>Fixed Incomplete/Missing Pages, Routes</td>
</tr>

<tr>
<td><a href="https://github.com/scorelab/OpenMF/issues/281" target="_blank">#281</a></td>
<td>[Frontend][Backend]Search User Feature </td>
<td><a href="https://github.com/scorelab/OpenMF/pull/293" target="_blank">#293</a></td>
<td>Search User implementation</td>
</tr>

<tr>
<td><a href="https://github.com/scorelab/OpenMF/issues/283" target="_blank">#283</a></td>
<td>[Backend]Management and Extractor with Google Auth </td>
<td><a href="https://github.com/scorelab/OpenMF/pull/290" target="_blank">#290</a></td>
<td>Login and Add user with Google</td>
</tr>

<tr>
<td><a href="https://github.com/scorelab/OpenMF/issues/284" target="_blank">#284</a></td>
<td>[Frontend][Backend]Inaccessible Routes in cases </td>
<td><a href="https://github.com/scorelab/OpenMF/pull/294" target="_blank">#294</a></td>
<td>Open method to Open case files</td>
</tr>

<tr>
<td><a href="https://github.com/scorelab/OpenMF/issues/282" target="_blank">#282</a></td>
<td>[Frontend][Backend]Non-Interactive Tasks Blocks </td>
<td><a href="https://github.com/scorelab/OpenMF/pull/292" target="_blank">#292</a></td>
<td>Toggle Task's is_complete status</td>
</tr>

<tr>
<td><a href="https://github.com/scorelab/OpenMF/issues/301" target="_blank">#301</a></td>
<td>[Frontend] Add icons to task card </td>
<td><a href="https://github.com/scorelab/OpenMF/pull/302" target="_blank">#302</a></td>
<td>Task card icon</td>
</tr>

<tr>
<td><a href="https://github.com/scorelab/OpenMF/issues/304" target="_blank">#304</a></td>
<td>[Frontend]Hide Profile Option from Navbar </td>
<td><a href="https://github.com/scorelab/OpenMF/pull/305" target="_blank">#305</a></td>
<td>Commented Profile Option</td>
</tr>

<tr>
<td><a href="https://github.com/scorelab/OpenMF/issues/288" target="_blank">#288</a></td>
<td>[Frontend][Backend]Task Update </td>
<td><a href="https://github.com/scorelab/OpenMF/pull/306" target="_blank">#306</a></td>
<td>Task update</td>
</tr>

<tr>
<td><a href="https://github.com/scorelab/OpenMF/issues/295" target="_blank">#295</a></td>
<td>[Frontend][Backend] Create User DashBoard </td>
<td><a href="" target="_blank">-</a></td>
<td>Multiple PRs</td>
</tr>

<tr>
<td><a href="https://github.com/scorelab/OpenMF/issues/296" target="_blank">#296</a></td>
<td>[Frontend] Create Profile Card Component</a></td>
<td><a href="https://github.com/scorelab/OpenMF/pull/298" target="_blank">#298</a></td>
<td>Created User Dashboard</td>
</tr>

<tr>
<td><a href="https://github.com/scorelab/OpenMF/issues/297" target="_blank">#297</a></td>
<td>[Frontend] Add tasks to Dashboard</a></td>
<td><a href="https://github.com/scorelab/OpenMF/pull/298" target="_blank">#298</a></td>
<td>Created User Dashboard</td>
</tr>

<tr>
<td><a href="https://github.com/scorelab/OpenMF/issues/299" target="_blank">#299</a></td>
<td>[Frontend]Sidebar showing wrong options</a></td>
<td><a href="https://github.com/scorelab/OpenMF/pull/303" target="_blank">#303</a></td>
<td>Fixed Sidebar</td>
</tr>

<tr>
<td><a href="https://github.com/scorelab/OpenMF/issues/267" target="_blank">#267</a></td>
<td>[Backend][Frontend] Extraction of Data </a></td>
<td><a href="https://github.com/scorelab/OpenMF/pull/307" target="_blank">#307</a></td>
<td>Download the JSON as .json and .xml</td>
</tr>

</table>
