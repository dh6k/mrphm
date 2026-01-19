# mrph builder
[![Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/morphe_magisk)
[![CI](https://github.com/dh6k/mrph/actions/workflows/ci.yml/badge.svg?event=schedule)](https://github.com/dh6k/mrph/actions/workflows/ci.yml)

Extensive Morphe builder for personal use, compatible with [Obtainium](https://github.com/ImranR98/Obtainium)

Get the [latest CI release](https://github.com/dh6k/mrph/releases).

Use [**zygisk-detach**](https://github.com/j-hc/zygisk-detach) to detach YouTube and YT Music from Play Store if you are using magisk modules. 

<details><summary><big>Features</big></summary>
<ul>
 <li>Support all present and future <a href="https://github.com/MorpheApp/morphe-patches">Morphe</a> apps</li>
 <li> Can build Magisk modules and non-root APKs</li>
 <li> Updated daily with the latest versions of apps and patches</li>
 <li> Optimize APKs and modules for size</li>
 <li> Modules</li>
    <ul>
     <li> recompile invalidated odex for faster usage</li>
     <li> receive updates from Magisk app</li>
     <li> do not break safetynet or trigger root detections</li>
     <li> handle installation of the correct version of the stock app and all that</li>
     <li> support Magisk and KernelSU</li>
    </ul>
</ul>
Note that the <a href="../../actions/workflows/ci.yml">CI workflow</a> is scheduled to build the modules and APKs everyday using GitHub Actions if there is a change in Morphe patches. You may want to disable it.
</details>

## To build

 * Run the build [workflow](../../actions/workflows/build.yml)
 * Grab your modules and APKs from [releases](../../releases)

also see here [`CONFIG.md`](./CONFIG.md)

## Building Locally
### On Termux
```console
bash <(curl -sSf https://raw.githubusercontent.com/dh6k/mrph/main/build-termux.sh)
```

### On Desktop
```console
$ git clone https://github.com/dh6k/mrph
$ cd mrph
$ ./build.sh
```
