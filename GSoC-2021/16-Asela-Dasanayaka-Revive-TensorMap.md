# Revive TensorMap

## Student Informations

* Name - Asela Dasanayaka
* Email - aselarbd@gmail.com
* Github - https://github.com/aselarbd
* LinkedIn - https://www.linkedin.com/in/aseladasanayaka/

# Project Abstract

TensorMap is a web application that will allow the users to create machine learning algorithms visually. TensorMap supports reverse engineering of the visual layout to a Tensorflow implementation in preferred languages. The goal of the project is to let the beginners play with machine learning algorithms in Tensorflow without less background knowledge about the library.

## [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#6699415781244928)

## [GSoC Project Proposal](https://docs.google.com/document/d/1AY_mf4rnHsf6TzAiGJOpA3BJnF33aNGkMpJNq-aB004/edit?usp=sharing)

## [GitHub Organization Repo](https://github.com/scorelab/tensormap)

## [GitHub Personal Repo](https://github.com/aselarbd/tensormap)

## [Commits during GSoC 2021](https://github.com/scorelab/tensormap/commits?author=aselarbd)

## [Project Demo Video](http://LinkToDemoVideo)

## [Project Wiki](https://github.com/scorelab/tensormap/wiki)

## [GSoC Blog](https://aselarbd.medium.com/journey-of-gsoc21-1-e20d49871852)

# Work Summary

In Google Summer of Code 2021, I have restructured and revamped the TensorMap Project, flask-based back-end and react base front-end  Application. 

In the beginning, the project was in an unusable state. I defined new scalable architecture for the project that can do incremental feature addition in future and established a solid foundational project.

Here are some important insights:-

### Implementations of the Features

| Milestone | #  | Feature                                                                                              | Status   | Commit | PR |
|-----------|----|------------------------------------------------------------------------------------------------------|----------|--------|----|
|     1     |  1 | setting up a basic backend application with Flask with  config management service and MySQL database | Merged ✅ |  [#1](https://github.com/scorelab/tensormap/commit/2183d4b418bad8908837ca94a1ae1a3ca5668dd4), [#2](https://github.com/scorelab/tensormap/commit/7b6fb5ad16581f628669d6cddf2858b211595195), [#3](https://github.com/scorelab/tensormap/commit/9b5914d42ba89e0c8ef348ecfc142ed30b8e92c2), [#4](https://github.com/scorelab/tensormap/commit/4431476e2227c849dff6ad1d349a0beff51aeb4f)     |  [#1](https://github.com/scorelab/tensormap/pull/163)  |
|     1     |  2 | Implement the data processing API and It services                                                    | Merged ✅ |   [#10](https://github.com/scorelab/tensormap/commit/c14b90060fe64b40ffab098d34a1b0fe01184789), [#11](https://github.com/scorelab/tensormap/commit/0ece5e12d862f6cd271a19d9b7d256c9424e9ebe), [#12](https://github.com/scorelab/tensormap/commit/3f615af61e3b392bbfd65bf2e46a04e18ff19840)     |  [#2](https://github.com/scorelab/tensormap/pull/164)  |
|     1     |  3 | Implement the data uploading API and its related services                                            | Merged ✅ |   [#5](https://github.com/scorelab/tensormap/commit/b31d89cb3ffe638446a566ddd6d8ab209b6c12cc), [#6](https://github.com/scorelab/tensormap/commit/4b64ff2cd56de0062acb112c7599a168f4d819c5), [#7](https://github.com/scorelab/tensormap/commit/fdb95f7d7c33a711117e7fa1b6f88aba75ce974b), [#8](https://github.com/scorelab/tensormap/commit/d5e6cfd926e731730ab138ed5cc39ea111805871), [#9](https://github.com/scorelab/tensormap/commit/3cce1f76069afd35d298d41fc65d4480474538f9)     |  [#2](https://github.com/scorelab/tensormap/pull/164)  |
|     1     |  4 | Implement the DL model generation service                                                            | Merged ✅ |  [#13](https://github.com/scorelab/tensormap/commit/6d1dc6127e7e047019c5446a6ed9a1f8cb0aad58), [#14](https://github.com/scorelab/tensormap/commit/b6eeb4e783de0058409d38b00a0edcafb7e0df96)      |  [#3](https://github.com/scorelab/tensormap/pull/165)  |
|     1     |  5 | Implement the DL model code generation service                                                       | Merged ✅ |   [#15](https://github.com/scorelab/tensormap/commit/ab63de46d359899a58d20163965bdd276f9ef347), [#16](https://github.com/scorelab/tensormap/commit/2d1afd41caee1052ea5f84ae17396f02294362c4)     |   [#3](https://github.com/scorelab/tensormap/pull/165)  |
|     1     |  6 | Implement the DL model execution service and tunneling the services with websockets                  | Merged ✅ |   [#17](https://github.com/scorelab/tensormap/commit/0bf3365854ddf54d805a93dd0a7bbc78b4705374), [#18](https://github.com/scorelab/tensormap/commit/c3307b509c24c87272f752188db8a3d0e7ac8dbf), [#19](https://github.com/scorelab/tensormap/commit/1726c2165ce9348a4b6afb8762954a2a1a27c4cd), [#20](https://github.com/scorelab/tensormap/commit/a9978ad1a5f64439bef8f0fd51c666e5b473dd71), [#21](https://github.com/scorelab/tensormap/commit/455f3203090573d452fce7558b71032709229fb0)     |  [#3](https://github.com/scorelab/tensormap/pull/165)  |
|     2     |  7 | Set up a frontend and implement the application template.                                            | Merged ✅ |   [#22](https://github.com/scorelab/tensormap/commit/f81531f1fe956c4a7324b44b375bbf3791c19083), [#23](https://github.com/scorelab/tensormap/commit/94e2c358a802e4db5002065901c9215a01cfbf3f)     |  [#4](https://github.com/scorelab/tensormap/pull/166)  |
|     2     |  8 | Implement the home page.                                                                             | Merged ✅ |    [#24](https://github.com/scorelab/tensormap/commit/60b8552c5f3edbfbb7ca0c4758f812117becd153), [#25](https://github.com/scorelab/tensormap/commit/91b9f2ccd3c9abd6886b856bc3555493af9b1da4)    |  [#4](https://github.com/scorelab/tensormap/pull/166)  |
|     2     |  9 | Implement the data upload page and connect the backend                                               | Merged ✅ |    [#26](https://github.com/scorelab/tensormap/commit/762ad4b6466a5096cc91ca6b689fbcbdb03c88ed)    |  [#4](https://github.com/scorelab/tensormap/pull/166)  |
|     2     | 10 | Implement the data process page and connect the backend                                              | Merged ✅ |    [#26](https://github.com/scorelab/tensormap/commit/762ad4b6466a5096cc91ca6b689fbcbdb03c88ed)   |  [#4](https://github.com/scorelab/tensormap/pull/166)  |
|     2     | 11 | Implement the Drag and drop feature for the DL model creation.                                       | Merged ✅ |    [#27](https://github.com/scorelab/tensormap/commit/1f0622b5f54c0a5db8503dce17fbf16e97442be9)    |  [#5](https://github.com/scorelab/tensormap/pull/167)  |
|     2     | 12 | Implement the dynamic properties sidebar                                                             | Merged ✅ |    [#28](https://github.com/scorelab/tensormap/commit/e506eccec994b0df9f7cf031f76b033eb33ef7e2), [#29](https://github.com/scorelab/tensormap/commit/8accfbe7180f0c9d166aca07d89d709db3611cac)    |  [#5](https://github.com/scorelab/tensormap/pull/167)  |
|     2     | 13 | Implement the Results panel                                                                          | Merged ✅ |    [#30](https://github.com/scorelab/tensormap/commit/a9978ad1a5f64439bef8f0fd51c666e5b473dd71), [#31](https://github.com/scorelab/tensormap/commit/b4e78564d353bd809df700f32296ea9bcb90f2d1), [#32](https://github.com/scorelab/tensormap/commit/1d448576f73f6ef2a1b7c98deb76fd95eaf413bf), [#33](https://github.com/scorelab/tensormap/commit/455f3203090573d452fce7558b71032709229fb0)    |  [#5](https://github.com/scorelab/tensormap/pull/167)  |
|     3     | 14 | Connected complete backend to frontend                                                               | Merged ✅ |    [#34](https://github.com/scorelab/tensormap/commit/455f3203090573d452fce7558b71032709229fb0), [#35](https://github.com/scorelab/tensormap/commit/b4e78564d353bd809df700f32296ea9bcb90f2d1)    |  [#5](https://github.com/scorelab/tensormap/pull/167)  |



# What Covered

All of the above-marked tasks are covered.  

# What left

* Improve documentation and instructions on how to add new features.
