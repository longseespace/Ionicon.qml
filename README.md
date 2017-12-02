# Ionicon.qml

Ionicon.qml bundle Ionicon font and icon table into a single module for QML
project.

## Features

1. Installable by qpm
2. Work well with Qt Quick Designer. Able to show icons in "Design" mode
3. Auto completion of icon name works in Qt Creator.

![Screenshot](https://raw.githubusercontent.com/longseespace/Ionicon.qml/master/docs/designmode.png)

## Installation

The package is provided as a qpm package,
[`co.podzim.ionicon`](https://www.qpm.io/packages/co.podzim.ionicon/index.html).
To install:

1. Install qpm (See
   [GitHub - Installing](https://github.com/Cutehacks/qpm/blob/master/README.md#installing),
   for **windows** see below)
2. In your projects root directory, run `qpm install co.podzim.ionicon`
3. Include qpm to your project by adding `include(vendor/vendor.pri)` to your
   `.pro` file

## QML Usage

1. Add `IoniconLoader` to your `main.qml`

```
import QtQuick 2.0
import Ionicon 1.0

IoniconLoader {}
```

2. Use `Iconicon` in other views

```
import QtQuick 2.5
import Ionicon 1.0

Ionicon {
    id: icon
    x: 162
    y: 162
    source: "heart"
    size: 64
    color: 'black'
}
```

## Icon Table

See
[ionicons.js](https://github.com/longseespace/Ionicon.qml/blob/master/Ionicon/ionicons.js)
