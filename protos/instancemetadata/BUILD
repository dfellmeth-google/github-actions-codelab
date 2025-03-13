# instance metadata proto

load("//third_party/protobuf/bazel:proto_library.bzl", "proto_library")
load("//tools/build_defs/go:go_proto_library.bzl", "go_proto_library")

package(
    default_applicable_licenses = ["//third_party/sapagent:license"],
    default_compatible_with = ["//buildenv/target:non_prod"],
    default_visibility = [
        "//third_party/sapagent:__subpackages__",
    ],
)

proto_library(
    name = "instancemetadata_proto",
    srcs = ["instancemetadata.proto"],
    deps = ["//third_party/sapagent/protos/instanceinfo:instanceinfo_proto"],
)

go_proto_library(
    name = "instancemetadata_go_proto",
    deps = [":instancemetadata_proto"],
)
