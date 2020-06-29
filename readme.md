说明
==========================================================

这个工程是 [官方KxMovie](https://github.com/kolyvan/kxmovie)的个人定制版，因为源工程多年不更新了，本工程旨在修复编译错误和一些自己的定制内容。

### 查看Demo效果

1. 编译按自己需求定制的ffmpeg，可食用https://github.com/kewlbear/FFmpeg-iOS-build-script.git进行自动化编译。
2. 将编译后的FFmpeg-iOS拖入工程，即可编译运行。如果遇到错误，请检查Header Search Path是否与自己的真实情况对应。

### 集成到自己的项目

1. 同样，你需要自己编译后的ffmpeg静态库。
2. 将kxmovie部分源码导入自己的工程。
3. API使用如下:

	ViewController *vc;
	vc = [KxMovieViewController movieViewControllerWithContentPath:path parameters:nil];
	[self presentViewController:vc animated:YES completion:nil];

### 截屏

<img src="https://raw.github.com/atelierdumobile/FFmpegPlayer-iOS/master/readme-media/screenshot-movie.png" alt="Movie View" width="50%">
<img src="https://raw.github.com/atelierdumobile/FFmpegPlayer-iOS/master/readme-media/screenshot-info.png" alt="Info View" width="50%">
<img src="https://raw.github.com/atelierdumobile/FFmpegPlayer-iOS/master/readme-media/screenshot-movie-landscape.png" alt="Movie View Landscape" width="50%">