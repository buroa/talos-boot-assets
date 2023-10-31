# talos-boot-assets

## Overview

This repository contains a [GitHub Actions](https://docs.github.com/en/actions) workflow that runs on a cronjob every hour to check and see if a new official [Talos Linux](https://github.com/siderolabs/talos) release has been pushed.

If it detects a newer version is available _(compared to the tag(s) in this repo)_ it will use [Talos Imager](https://github.com/siderolabs/talos/tree/main/pkg/imager) to build new [Boot Assets](https://www.talos.dev/v1.5/talos-guides/install/boot-assets/) used in my [k8s-gitops](https://github.com/buroa/k8s-gitops) environment.
