package(default_visibility = ["//visibility:public"])

load("@io_bazel_rules_go//go:def.bzl", "go_binary", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["main.go"],
    deps = [
        "//tests/integration/example/environment/appOnlyEnv:go_default_library",
        "//tests/integration/framework:go_default_library",
    ],
)

go_binary(
    name = "app_only_env",
    library = ":go_default_library",
)
