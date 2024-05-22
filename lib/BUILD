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
        "@krb5//:krb5",
        "@re2",
        "@rapidjson",
        "@hdrhistogram_c",
        "@liburing",
        "@zlib",
        "@fmt",
        #"@c-ares",
        "@lz4",
        "@xz//:libxz",
        "@xml2//:libxml2",
        "@cryptopp//:libcryptopp",
        "@base64//:libbase64",
        "@ada//:libada",
        "@openssl//:libopenssl",
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

