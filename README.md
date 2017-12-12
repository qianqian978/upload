# upload
H5文件api实现移动端图片的裁剪、翻转及预览效果

一：jquery.cropit.js：<br/>
使用html5的文件api，FileReader接口读取文件，将文件读取为DataURL，实现图片的预览

二：exif_min.js:<br/>
HTML5+canvas进行移动端手机照片上传时，发现iOS手机上传竖拍照片会逆时针旋转90度，横拍照片无此问题；Android手机没这个问题。

因此解决这个问题的思路是：获取到照片拍摄的方向角，对非横拍的ios照片进行角度旋转修正。

利用exif.js读取照片的拍摄信息，这里主要用到Orientation属性。

