load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")



http_archive(

    name = "rules_pods",

    urls = ["https://github.com/pinterest/PodToBUILD/releases/download/0.25.2-8a5efa0/PodToBUILD.zip"],

)



load("@rules_pods//BazelExtensions:workspace.bzl", "new_pod_repository")

new_pod_repository(

  name = "AFNetworking",

  url = "https://github.com/AFNetworking/AFNetworking/archive/3.1.0.zip",

  enable_modules = False,

)


load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")


git_repository(

    name = "build_bazel_rules_apple",

    remote = "https://github.com/bazelbuild/rules_apple.git",

    tag = "0.21.2",

)



git_repository(

    name = "build_bazel_rules_swift",

    remote = "https://github.com/bazelbuild/rules_swift.git",

    tag = "0.17.0",

)



git_repository(

    name = "build_bazel_apple_support",

    remote = "https://github.com/bazelbuild/apple_support.git",

    tag = "0.9.1",

)



git_repository(

    name = "bazel_skylib",

    remote = "https://github.com/bazelbuild/bazel-skylib.git",

    tag = "1.0.3",

)