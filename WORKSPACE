workspace(name = "mx_filter")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "istio_wasm_sdk",
    strip_prefix = "istio-wasm-sdk-032a1d2be96648edaf31c95b65011bc81118bd53",
    url = "https://github.com/bianpengyuan/istio-wasm-sdk/archive/032a1d2be96648edaf31c95b65011bc81118bd53.tar.gz",
)

load("@istio_wasm_sdk//bazel:sdk_dependencies.bzl", "sdk_dependencies")

sdk_dependencies()

load("@istio_wasm_sdk//bazel:sdk_dependency_imports.bzl", "sdk_dependency_imports")

sdk_dependency_imports()
