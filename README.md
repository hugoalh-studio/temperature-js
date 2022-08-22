# Temperature (NodeJS)

[`Temperature.NodeJS`](https://github.com/hugoalh-studio/temperature-nodejs)
[![GitHub Contributors](https://img.shields.io/github/contributors/hugoalh-studio/temperature-nodejs?label=Contributors&logo=github&logoColor=ffffff&style=flat-square)](https://github.com/hugoalh-studio/temperature-nodejs/graphs/contributors)
[![GitHub Issues](https://img.shields.io/github/issues-raw/hugoalh-studio/temperature-nodejs?label=Issues&logo=github&logoColor=ffffff&style=flat-square)](https://github.com/hugoalh-studio/temperature-nodejs/issues)
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr-raw/hugoalh-studio/temperature-nodejs?label=Pull%20Requests&logo=github&logoColor=ffffff&style=flat-square)](https://github.com/hugoalh-studio/temperature-nodejs/pulls)
[![GitHub Discussions](https://img.shields.io/github/discussions/hugoalh-studio/temperature-nodejs?label=Discussions&logo=github&logoColor=ffffff&style=flat-square)](https://github.com/hugoalh-studio/temperature-nodejs/discussions)
[![GitHub Stars](https://img.shields.io/github/stars/hugoalh-studio/temperature-nodejs?label=Stars&logo=github&logoColor=ffffff&style=flat-square)](https://github.com/hugoalh-studio/temperature-nodejs/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/hugoalh-studio/temperature-nodejs?label=Forks&logo=github&logoColor=ffffff&style=flat-square)](https://github.com/hugoalh-studio/temperature-nodejs/network/members)
![GitHub Languages](https://img.shields.io/github/languages/count/hugoalh-studio/temperature-nodejs?label=Languages&logo=github&logoColor=ffffff&style=flat-square)
[![CodeFactor Grade](https://img.shields.io/codefactor/grade/github/hugoalh-studio/temperature-nodejs?label=Grade&logo=codefactor&logoColor=ffffff&style=flat-square)](https://www.codefactor.io/repository/github/hugoalh-studio/temperature-nodejs)
[![License](https://img.shields.io/static/v1?label=License&message=MIT&style=flat-square)](./LICENSE.md)

| **Release** | **Latest** (![GitHub Latest Release Date](https://img.shields.io/github/release-date/hugoalh-studio/temperature-nodejs?label=%20&style=flat-square)) | **Pre** (![GitHub Latest Pre-Release Date](https://img.shields.io/github/release-date-pre/hugoalh-studio/temperature-nodejs?label=%20&style=flat-square)) |
|:-:|:-:|:-:|
| [**GitHub**](https://github.com/hugoalh-studio/temperature-nodejs/releases) ![GitHub Total Downloads](https://img.shields.io/github/downloads/hugoalh-studio/temperature-nodejs/total?label=%20&style=flat-square) | ![GitHub Latest Release Version](https://img.shields.io/github/release/hugoalh-studio/temperature-nodejs?sort=semver&label=%20&style=flat-square) | ![GitHub Latest Pre-Release Version](https://img.shields.io/github/release/hugoalh-studio/temperature-nodejs?include_prereleases&sort=semver&label=%20&style=flat-square) |
| [**NPM**](https://www.npmjs.com/package/@hugoalh/temperature) ![NPM Total Downloads](https://img.shields.io/npm/dt/@hugoalh/temperature?label=%20&style=flat-square) | ![NPM Latest Release Version](https://img.shields.io/npm/v/@hugoalh/temperature/latest?label=%20&style=flat-square) | ![NPM Latest Pre-Release Version](https://img.shields.io/npm/v/@hugoalh/temperature/pre?label=%20&style=flat-square) |

## 📝 Description

A NodeJS module to convert temperature units.

Units of temperature are from [Wikipedia - Conversion of scales of temperature](https://en.wikipedia.org/wiki/Conversion_of_scales_of_temperature).

| **Unit** | **Symbol** | **Symbol Lowercase** | **Name** | **Name Lowercase** |
|:-:|:-:|:-:|:-:|:-:|
| Celsius | `C` | `c` | `Celsius` | `celsius` |
| Fahrenheit | `F` | `f` | `Fahrenheit` | `fahrenheit` |
| Kelvin | `K` | `k` | `Kelvin` | `kelvin` |
| Rankine | `R` | `r` | `Rankine` | `rankine` |
| Delisle | `De` | `de` | `Delisle` | `delisle` |
| Sir Isaac Newton's degree of temperature (Newton) | `N` | `n` | `Newton` | `newton` |
| Réaumur | `Re` | `re` | `Reaumur` | `reaumur` |
| Rømer | `Ro` | `ro` | `Roemer`, `Romer` | `roemer`, `romer` |

> **📋 Note**
>
> - Degree symbol (`°`) is not used in here.
> - In order to fulfill the JavaScript namespace naming requirement, some characters are replaced (e.g.: `é` to `e`, `ø` to `o`).

## 📚 Documentation

### Getting Started

#### Install

- NodeJS >= v6.9.0
- NPM >= v3.10.8

```sh
npm install @hugoalh/temperature
```

#### Use In CommonJS

```js
const Temperature = require("@hugoalh/temperature");
```

#### Use In ModuleJS

```js
import Temperature from "@hugoalh/temperature";
```

### API

#### Class

```ts
Temperature(value: number, unit?: string = "K")
```

### Example

```js
new Temperature(25, "C").K
//=> 298.15

new Temperature(298.15).C
//=> 25
```
