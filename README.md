CrystalCraftMC Infrastructure
=============================

[![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
[![Build Status](https://travis-ci.org/CrystalCraftMC/infrastructure.svg?branch=main)](https://travis-ci.org/CrystalCraftMC/infrastructure)

Set of scripts, Ansible playbooks/roles, and other tools to automate and manage CrystalCraftMC infrastructure


## About

This repository contains various scripts and other automation tools to manage CrystalCraftMC infrastructure.
Important changes to any infrastructure configurations or settings should be made as a [Pull Request](https://opensource.guide/how-to-contribute/#opening-a-pull-request) to this repository.


## How to use

To synchronize the state of the CrystalCraftMC Legacy Minecraft server, run the following playbook:

```sh
ansible-playbook --user $USER --ask-become-pass playbooks/main.yml
```


## Legal

Licensed under [BSD 2-Clause License](https://opensource.org/licenses/BSD-2-Clause).
Not a lawyer?
This basically means that you are free to:

* **Use commercially**:
  Permitted to use software for commercial purposes.
* **Modify**:
  Permitted to modify the software and make derivatives/remixes.
* **Distribute**:
  Permitted to distribute original or modified (derivative) works.

Provided you meet the following terms:

* **Attribution**:
  You must give appropriate credit, provide a link to the license, and indicate if changes were made.
  You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
* **Include license**:
  Include a full copy of the [BSD 2-Clause License text](https://github.com/CrystalCraftMC/infrastructure/blob/main/LICENSE.txt) in modified software attributions.

### Attributions

This repository is largely influenced by others like it:

* [jwflory/infrastructure](https://github.com/jwflory/infrastructure)
* [FOSSRIT/infrastructure](https://github.com/FOSSRIT/infrastructure)
* [jwflory/swiss-army](https://github.com/jwflory/swiss-army)
