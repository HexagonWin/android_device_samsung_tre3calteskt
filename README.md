## TWRP device tree for Samsung Galaxy Note 4 Exynos 3CAL-LTE KOR N916S/L/K (tre3calteskt)

 Copyright (C) 2019 Ananjaser1211 Open-Source

 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at

      http://www.apache.org/licenses/LICENSE-2.0

 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.


Add to `.repo/local_manifests/tre3calteskt.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project name="universal5433/android_device_samsung_tre3calteskt" path="device/samsung/tre3calteskt" remote="github" revision="android-7.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_tre3calteskt-eng
make -j5 recoveryimage
```

Kernel source: https://github.com/ananjaser1211/RefinedNougat
