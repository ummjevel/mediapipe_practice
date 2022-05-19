# Description:
#   OpenCV libraries for video/image processing on MacOS

licenses(["notice"])  # BSD license

exports_files(["LICENSE"])

cc_library(
    name = "opencv",
    srcs = glob(
        [
            "local/lib/libopencv_core.dylib",
            "local/lib/libopencv_highgui.dylib",
            "local/lib/libopencv_imgcodecs.dylib",
            "local/lib/libopencv_imgproc.dylib",
            "local/lib/libopencv_video.dylib",
            "local/lib/libopencv_videoio.dylib",
        ],
    ),
    hdrs = glob(["local/include/opencv3/opencv2/**/*.h*"]),
    includes = ["local/include/opencv3/"],
    linkstatic = 1,
    visibility = ["//visibility:public"],
)
