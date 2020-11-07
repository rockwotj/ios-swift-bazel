load("@build_bazel_rules_apple//apple:ios.bzl", "ios_application")
load("@build_bazel_rules_swift//swift:swift.bzl", "swift_library")

swift_library(
    name = "app",
    srcs = ["App.swift"],
    data = [],
    deps = [],
)

ios_application(
    name = "ios",
    app_icons = [],
    bundle_id = "com.example.app",
    families = [
        "iphone",
        "ipad",
    ],
    infoplists = [":Info.plist"],
    minimum_os_version = "14.0",
    deps = [":app"],
)
