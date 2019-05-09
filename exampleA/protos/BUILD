load("@build_stack_rules_proto//python:python_proto_library.bzl", "py_proto_library")

package(default_visibility=["//visibility:public"])

proto_library(
  name = "common_proto",
  srcs = ["common.proto"],
)

proto_library(
  name = "something_proto",
  srcs = ["something.proto"],
  deps = [":common_proto"],
)

py_proto_library(
  name = "py_something_proto",
  deps = [":something_proto"],
)
