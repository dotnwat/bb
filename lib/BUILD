cc_binary(
    name = "main",
    srcs = ["main.cc"],
    deps = [
        "@abseil-cpp//absl/container:flat_hash_set",
        "@abseil-cpp//absl/functional:any_invocable",
        "@nettle//:libnettle",
        "@gmp//:libgmp",
        "@gnutls//:libgnutls",
        "@numactl//:libnumactl",
        "@libpciaccess//:libpciaccess",
        "@hwloc//:hwloc",
    ],
)

cc_test(
    name = "main_test",
    srcs = ["main.cc"],
    deps = [
        ":main",
        "@googletest//:gtest",
        "@googletest//:gtest_main",
    ],
)

