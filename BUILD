cc_import(
    name = "bar",
    static_library = "bar.a",
)

cc_library(
    name = "foo",
    srcs = ["foo.cpp", "bar.hpp"],
    hdrs = ["foo.hpp"],
    deps = [":bar"],
)

cc_test(
    name = "test",
    srcs = ["main.cpp"],
    deps = [":foo"],
    linkstatic = False,
)
