package(default_visibility = ["//visibility:public"])

licenses(["notice"])

exports_files(["__init__.py"])

cc_binary(
    name = "_pywrap_fast_bert_normalizer_model_builder.so",
    srcs = ["pywrap_fast_bert_normalizer_model_builder.cc"],
    deps = [
        "//tensorflow_text/core/kernels:fast_bert_normalizer_model_builder",
        "@pybind11//:pybind11",
    ],
    linkshared = 1,
    copts = ["-fPIC"],
)

py_library(
    name = "pywrap_fast_bert_normalizer_model_builder",
    srcs = [],
    data = [":_pywrap_fast_bert_normalizer_model_builder.so"],
    visibility = ["//visibility:public"],
)

cc_binary(
    name = "_pywrap_fast_wordpiece_tokenizer_model_builder.so",
    srcs = ["pywrap_fast_wordpiece_tokenizer_model_builder.cc"],
    deps = [
        "//tensorflow_text/core/kernels:fast_wordpiece_tokenizer_model_builder",
        "@pybind11//:pybind11",
    ],
    linkshared = 1,
    copts = ["-fPIC"],
)

py_library(
    name = "pywrap_fast_wordpiece_tokenizer_model_builder",
    srcs = [],
    data = [":_pywrap_fast_wordpiece_tokenizer_model_builder.so"],
    visibility = ["//visibility:public"],
)

cc_binary(
    name = "_pywrap_model_converter.so",
    srcs = ["pywrap_model_converter.cc"],
    deps = [
        "//tensorflow_text/core/kernels/sentencepiece:model_converter",
        "@pybind11//:pybind11",
    ],
    linkshared = 1,
    copts = ["-fPIC"],
)

py_library(
    name = "pywrap_model_converter",
    srcs = [],
    data = [":_pywrap_model_converter.so"],
    visibility = ["//visibility:public"],
)

cc_binary(
    name = "_pywrap_phrase_tokenizer_model_builder.so",
    srcs = ["pywrap_phrase_tokenizer_model_builder.cc"],
    deps = [
        "//tensorflow_text/core/kernels:phrase_tokenizer_model_builder",
        "@pybind11//:pybind11",
    ],
    linkshared = 1,
    copts = ["-fPIC"],
)

py_library(
    name = "pywrap_phrase_tokenizer_model_builder",
    srcs = [],
    data = [":_pywrap_phrase_tokenizer_model_builder.so"],
    visibility = ["//visibility:public"],
)

cc_binary(
    name = "_pywrap_whitespace_tokenizer_config_builder.so",
    srcs = ["pywrap_whitespace_tokenizer_config_builder.cc"],
    deps = [
        "//tensorflow_text/core/kernels:whitespace_tokenizer_config_builder",
        "@pybind11//:pybind11",
    ],
    linkshared = 1,
    copts = ["-fPIC"],
)

py_library(
    name = "pywrap_whitespace_tokenizer_config_builder",
    srcs = [],
    data = [":_pywrap_whitespace_tokenizer_config_builder.so"],
    visibility = ["//visibility:public"],
)

cc_binary(
    name = "_tflite_registrar.so",
    srcs = ["tflite_registrar.cc"],
    deps = [
        "//tensorflow_text/core/kernels:tflite_ops",
        "@pybind11//:pybind11",
    ],
    linkshared = 1,
    copts = ["-fPIC"],
)

py_library(
    name = "tflite_registrar",
    srcs = [],
    data = [":_tflite_registrar.so"],
    visibility = ["//visibility:public"],
)
