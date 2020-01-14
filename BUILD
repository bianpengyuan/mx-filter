cc_binary(
    name = "plugin.wasm",
    srcs = [
        "plugin.cc",
        "plugin.h",
        "base64.h",
    ],
    additional_linker_inputs = ["@envoy_wasm_api//:jslib"],
    linkopts = [
        "--js-library",
        "external/envoy_wasm_api/proxy_wasm_intrinsics.js",
        "-UHAVE_PTHREAD",
    ],
    deps = [
        "@envoy_wasm_api//:proxy_wasm_intrinsics",
        "@istio_wasm_sdk//:context",
        "@com_google_absl//absl/strings",
    ],
)
