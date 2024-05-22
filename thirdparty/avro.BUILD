load("@rules_foreign_cc//foreign_cc:defs.bzl", "cmake")

filegroup(
    name = "avro_srcs",
    srcs = glob(["**"]),
)

cmake(
    name = "libavro",
    lib_source = ":avro_srcs",
    working_directory = "lang/c++",
    cache_entries = {
      "CMAKE_SKIP_INSTALL_ALL_DEPENDENCY": "ON",
      "BUILD_SHARED_LIBS": "ON",
    },
    targets = ["avrocpp", "avrocpp_s", "avrogencpp"],
    out_shared_libs = ["libavro.so"],
    visibility = [
        "//visibility:public",
    ],
)
