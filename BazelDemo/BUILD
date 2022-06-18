load("@build_bazel_rules_apple//apple:ios.bzl", "ios_application")



objc_library(

    name = "SkeletonLib",

    srcs = glob(["*.m"]),

    hdrs = glob(["*.h"]),

    data = [

        "Base.lproj/Main.storyboard",

        "Base.lproj/LaunchScreen.storyboard"

    ],
    deps = ["@AFNetworking//:AFNetworking"],

)



ios_application(

    name = "BazelDemo",

    bundle_id = "com.Sharker.Tec.BazelDemo",

    families = ["iphone", "ipad",],

    minimum_os_version = "11.0",

    infoplists = ["Info.plist"],

    deps = [":SkeletonLib"],

)