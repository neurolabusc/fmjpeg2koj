# fmjpeg2koj
Windows [![Build status](https://ci.appveyor.com/api/projects/status/h3hv3qayr4obik87/branch/master?svg=true)](https://ci.appveyor.com/project/DraconPern/fmjpeg2koj/branch/master) OS X [![Build Status](https://travis-ci.org/DraconPern/fmjpeg2koj.svg?branch=master)](https://travis-ci.org/DraconPern/fmjpeg2koj)

[DCMTK](https://dicom.offis.de/dcmtk.php.en) includes many open source tools for working with DICOM data. Unfortunately, the [dcmcjp2k](https://support.dcmtk.org/docs-products/dcmcjp2k.html) and [dcmdjp2k](https://support.dcmtk.org/docs-products/dcmdjp2k.html) tools are not provided as open source because they use a proprietary library for handling JPEG2000. 

This repository resolves this limitation, adopting the JPEG2000 codec for DCMTK based on [OpenJPEG](https://www.openjpeg.org). Be aware that [OpenJPEG's JPEG2000](https://crnl.readthedocs.io/jpeg_formats/index.html) is slow relative to other options, such as the lossless JPEG supported by [dcmcjpeg](https://support.dcmtk.org/docs/dcmcjpeg.html) and  [dcmdjpeg](https://support.dcmtk.org/docs/dcmdjpeg.html). Therefore, the tools provided in this repository may be useful for decoding DICOM images provided by others, but probably should not be used intentionally for encoding data.

## Download
Source https://github.com/DraconPern/fmjpeg2koj

## Requirements
- CMake http://www.cmake.org/download/

## Third party dependency
- DCMTK http://dicom.offis.de/
- openjpeg http://www.openjpeg.org/

## Author
Ing-Long Eric Kuo <draconpern@hotmail.com>

## License
Copyright 2015-2017 Ing-Long Eric Kuo

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

