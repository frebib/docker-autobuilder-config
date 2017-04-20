# [frebib/autobuilder](https://github.com/frebib/docker-autobuilder) Configuration Files

This repository is a collection of personally used configuration files for the autobuilder Docker image. Configuration files should be mounted at `/config` inside the container.

# Example

Below is an example directory structure showing the possible layout functionality with images, builds, hooks and overrides for both hooks & environment files

```
/config
├── image-name/
│   ├── build/
│   │   ├── stable/
│   │   │   ├── env
│   │   │   └── hooks/
│   │   │       └── post_checkout*
│   │   └── testing/
│   │       └── env
│   ├── compare-version*
│   ├── depends
│   ├── env
│   ├── get-release*
│   └── hooks/
│       ├── pre_push*
│       ├── tag*
│       └── test*
│
├── another-image/
...
```
