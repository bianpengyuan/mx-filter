workspace(name = "istio_stats_filter")

local_repository(
    name="istio_wasm_sdk", 
    path="/home/bianpengyuan_google_com/workspace/istio-wasm-sdk",
)

load("@istio_wasm_sdk//bazel:sdk_dependencies.bzl", "sdk_dependencies")

sdk_dependencies()

load("@istio_wasm_sdk//bazel:sdk_dependency_imports.bzl", "sdk_dependency_imports")

sdk_dependency_imports()
