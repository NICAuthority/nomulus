package(
    default_testonly = 1,
    default_visibility = ["//java/google/registry:registry_project"],
)

licenses(["notice"])  # Apache 2.0

load("//java/com/google/testing/builddefs:GenTestRules.bzl", "GenTestRules")

java_library(
    name = "registrar",
    srcs = glob(["*.java"]),
    resources = glob(["testdata/*"]),
    deps = [
        "//java/google/registry/braintree",
        "//java/google/registry/config",
        "//java/google/registry/export/sheet",
        "//java/google/registry/model",
        "//java/google/registry/request",
        "//java/google/registry/request/auth",
        "//java/google/registry/security",
        "//java/google/registry/ui/server/registrar",
        "//java/google/registry/ui/soy/registrar:soy_java_wrappers",
        "//java/google/registry/util",
        "//javatests/google/registry/security",
        "//javatests/google/registry/testing",
        "//third_party/objectify:objectify-v4_1",
        "@com_braintreepayments_gateway_braintree_java",
        "@com_google_appengine_api_1_0_sdk//:testonly",
        "@com_google_flogger",
        "@com_google_flogger_system_backend",
        "@com_google_guava",
        "@com_google_guava_testlib",
        "@com_google_truth",
        "@com_google_truth_extensions_truth_java8_extension",
        "@com_googlecode_json_simple",
        "@javax_servlet_api",
        "@joda_time",
        "@junit",
        "@org_joda_money",
        "@org_mockito_all",
    ],
)

GenTestRules(
    name = "GeneratedTestRules",
    test_files = glob(["*Test.java"]),
    deps = [":registrar"],
)
