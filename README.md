
## Android-PickerView



### [English Document](https://github.com/Bigkoo/Android-PickerView/blob/master/README-en.md)

### 注意事项、详请使用方式、更新日志等，请查看 [Wiki文档](https://github.com/Bigkoo/Android-PickerView/wiki)
**Wiki文档，Wiki文档，Wiki文档 !~ 重要的事情说三遍**

### 有兴趣研究3D滚轮效果的实现机制，希望把源码研究透彻的可以看看这篇博客：
### [Android-PickerView系列之源码解析篇（二）](http://blog.csdn.net/qq_22393017/article/details/59488906)

参考https://github.com/Bigkoo/Android-PickerView时间选择器添加时间段，使用方式建议将pickerview作为moudle注入项目使用。
具体使用可参考https://github.com/Bigkoo/Android-PickerView/wiki文档。区别在于时间选择器初始化时需传入7个Boolean值，
setType(new boolean[]{true, true, true, false, false, false, true})，同时选择回调添加时间段item position回调。
根据position与时间段数组判断处于哪个时间段。

时间段定义在pickerview/res/attrs.xml中，可更换时间段。
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <string-array name="timePart">
        <item>8点之前</item>
        <item>8~10点 </item>
        <item>10~12点</item>
        <item>12~14点</item>
        <item>14~16点</item>
        <item>16~18点</item>
        <item>18点之后</item>
    </string-array>

</resources>

### Thanks

## License

```
Copyright 2014 Bigkoo
Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
