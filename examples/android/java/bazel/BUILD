filegroup(
    name = "srcs",
    srcs = glob(["**"]),
    visibility = ["//examples:__pkg__"],
)

android_library(
    name = "lib",
    srcs = ["Lib.java"],
)

android_binary(
    name = "hello_world",
    srcs = glob([
        "MainActivity.java",
    ]),
    manifest = "AndroidManifest.xml",
    resource_files = glob(["res/**"]),
    deps = [
        ":lib",
        "@androidsdk//com.android.support:appcompat-v7-25.0.0",
    ],
)
