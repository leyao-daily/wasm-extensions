load("@proxy_wasm_cpp_sdk//bazel/wasm:wasm.bzl", "wasm_cc_binary")

wasm_cc_binary(
    name = "ms.wasm",
    srcs = ["ms.cc", "utils.cc", "utils.h"],
    deps = [
        "@modsecurity//:lib",
        "@proxy_wasm_cpp_sdk//:proxy_wasm_intrinsics",
	"@com_google_absl//absl/strings",
        "@com_google_absl//absl/time",
        "@io_istio_proxy//extensions/common/wasm:json_util",
    ],
)

wasm_cc_binary(
    name = "plugin.wasm",
    srcs = ["ms.cc", "utils.cc", "utils.h"],
    deps = [
        "@modsecurity//:lib",
        "@proxy_wasm_cpp_sdk//:proxy_wasm_intrinsics",
        "@com_google_absl//absl/strings",
        "@com_google_absl//absl/time",
        "@io_istio_proxy//extensions/common/wasm:json_util",
    ],
)
