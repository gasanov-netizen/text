package(default_visibility = ["//visibility:public"])
licenses(["notice"])

cc_library(
    name = "tf_op_shim",
    srcs = [
      "tensorflow/lite/kernels/shim/tf_op_shim.cc",
      "tensorflow/lite/kernels/shim/tf_tensor_view.cc",
      "tensorflow/lite/kernels/shim/shape.cc",
    ],
    hdrs = [
        "tensorflow/lite/kernels/shim/op_kernel.h",
        "tensorflow/lite/kernels/shim/shape.h",
        "tensorflow/lite/kernels/shim/status_macros.h",
        "tensorflow/lite/kernels/shim/tensor_view.h",
        "tensorflow/lite/kernels/shim/tf_op_shim.h",
        "tensorflow/lite/kernels/shim/tf_tensor_view.h",
    ],
    includes = ["."],
    deps = [
        "@com_google_absl//absl/algorithm:container",
        "@com_google_absl//absl/base",
        "@com_google_absl//absl/container:btree",
        "@com_google_absl//absl/container:flat_hash_map",
        "@com_google_absl//absl/container:flat_hash_set",
        "@com_google_absl//absl/hash",
        "@com_google_absl//absl/meta:type_traits",
        "@com_google_absl//absl/utility",
        "@com_google_absl//absl/utility:if_constexpr",
        "@com_google_absl//absl/base:core_headers",
        "@com_google_absl//absl/log:absl_check",
        "@com_google_absl//absl/log:absl_log",
        "@com_google_absl//absl/log:check",
        "@com_google_absl//absl/status",
        "@com_google_absl//absl/status:statusor",
        "@com_google_absl//absl/strings",
        "@com_google_absl//absl/types:span",
        "@com_google_absl//absl/types:variant",
        "@release_or_nightly//:tensorflow_tf_header_lib",
    ],
)
