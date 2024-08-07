load("@rules_python//python:defs.bzl", "py_library")

py_library(
    name = "all_modules",
    srcs = ["__init__.py"],
    visibility = [
        "//visibility:public",
    ],
    deps = [
        ":json_message_converter",
        ":message_converter",
    ],
)

py_library(
    name = "json_message_converter",
    srcs = ["json_message_converter.py"],
    visibility = [
        "//visibility:public",
    ],
    deps = [
        ":message_converter",
    ],
)

py_library(
    name = "message_converter",
    srcs = ["message_converter.py"],
    visibility = [
        "//visibility:public",
    ],
    deps = [
        "@com_github_mvukov_rules_ros//:py_roslib_slim",
        "@ros_comm//:rospy",
    ],
)
