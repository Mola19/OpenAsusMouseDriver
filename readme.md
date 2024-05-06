# OpenAsusMiceDriver

This is a library to control modern Asus mice

- [OpenAsusMiceDriver](#openasusmicedriver)
	- [Supported Devices](#supported-devices)
    - [Building](#building)

## Supported Devices

| Symbol | Meaning                                                 |
| :----: | ------------------------------------------------------- |
|   ✔    | This device is fully implemented.                       |
|   ⚙    | This device is partially implemented. Work in progress. |

| Device                           | Support |
| -------------------------------- | :-----: |
| Asus ROG Chakram X[^1]           |    ⚙    |
| Asus ROG Spatha X                |    ⚙    |
| Asus ROG Keris Wireless AimPoint |    ⚙    |
| Asus ROG Pugio                   |    ⚙    |

[^1]: Also available as Asus ROG Chakram X Origin, but exactly the same besides lacking Qi charging

Feature support for every device is specified [here](supported_devices.md)

## Building

### Unix / Mac

To install into /usr/local, run:

```
mkdir build; cd build
cmake ..
make
sudo make install
```

The install directory can be changed using the `-DCMAKE_INSTALL_PREFIX` parameter for `cmake`.
If you want to dynamically link the library in a project, use the option `-DCMAKE_INSTALL_PREFIX=/usr`

