# nvidia

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&amp;logoColor=white)](https://github.com/rolehippie/nvidia)
[![General Workflow](https://github.com/rolehippie/nvidia/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/nvidia/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/nvidia/actions/workflows/readme.yml/badge.svg)](https://github.com/rolehippie/nvidia/actions/workflows/readme.yml)
[![Galaxy Workflow](https://github.com/rolehippie/nvidia/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/nvidia/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/nvidia)](https://github.com/rolehippie/nvidia/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.nvidia-blue)](https://galaxy.ansible.com/rolehippie/nvidia)

Ansible role to install nvidia graphics drivers.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [nvidia_enable_i386](#nvidia_enable_i386)
  - [nvidia_packages](#nvidia_packages)
  - [nvidia_version](#nvidia_version)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.10`


## Default Variables

### nvidia_enable_i386

Enable installation of i386 packages

#### Default value

```YAML
nvidia_enable_i386: true
```

### nvidia_packages

List of packages to install

#### Default value

```YAML
nvidia_packages:
  - nvidia-driver-{{ nvidia_version }}
  - libvulkan1
  - libvulkan1:i386
```

### nvidia_version

Version of Nvidia graphics driver

#### Default value

```YAML
nvidia_version: '525'
```

## Discovered Tags

**_nvidia_**


## Dependencies

- None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
