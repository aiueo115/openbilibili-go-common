load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["server.go"],
    importpath = "go-common/app/service/bbq/recsys-recall/server/grpc",
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
    deps = [
        "//app/service/bbq/recsys-recall/api/grpc/v1:go_default_library",
        "//app/service/bbq/recsys-recall/service:go_default_library",
        "//library/net/rpc/warden:go_default_library",
        "//library/time:go_default_library",
        "@org_golang_google_grpc//:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
