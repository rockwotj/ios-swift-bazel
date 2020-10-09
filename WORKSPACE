load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive", "http_file")

RULES_APPLE_VERSION = '0.20.0'

http_archive(
    name = "build_bazel_rules_apple",
    sha256 = "55f4dc1c9bf21bb87442665f4618cff1f1343537a2bd89252078b987dcd9c382",
    url = "https://github.com/bazelbuild/rules_apple/releases/download/{0}/rules_apple.{0}.tar.gz".format(RULES_APPLE_VERSION),
)

RULES_SWIFT_VERSION = '0.15.0'

http_archive(
    name = "build_bazel_rules_swift",
    sha256 = "d2f38c33dc82cf3160c59342203d31a030e53ebe8f4c7365add7a549223f9c62",
    url = "https://github.com/bazelbuild/rules_swift/releases/download/{0}/rules_swift.{0}.tar.gz".format(RULES_SWIFT_VERSION),
)

load(
    "@build_bazel_rules_apple//apple:repositories.bzl",
    "apple_rules_dependencies",
)

apple_rules_dependencies()

load(
    "@build_bazel_rules_swift//swift:repositories.bzl",
    "swift_rules_dependencies",
)

swift_rules_dependencies()

load(
    "@build_bazel_apple_support//lib:repositories.bzl",
    "apple_support_dependencies",
)

apple_support_dependencies()


load(
    "@build_bazel_rules_swift//swift:repositories.bzl",
    "swift_rules_dependencies",
)

swift_rules_dependencies()

load(
    "@build_bazel_rules_swift//swift:extras.bzl",
    "swift_rules_extra_dependencies",
)

swift_rules_extra_dependencies()
