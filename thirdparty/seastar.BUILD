load("@rules_foreign_cc//foreign_cc:defs.bzl", "cmake")

filegroup(
    name = "seastar_srcs",
    srcs = glob(["**"]),
)

cmake(
    name = "libseastar",
    lib_source = ":seastar_srcs",
    cache_entries = {
        "CMAKE_CXX_STANDARD": "20",
        "Seastar_API_LEVEL": "6",
        "Seastar_LOGGER_COMPILE_TIME_FMT": "OFF"
    },
    out_static_libs = ["libseastar.a"],
    deps = [
        "@boost//:boost",
    ],
    visibility = [
        "//visibility:public",
    ],
)
