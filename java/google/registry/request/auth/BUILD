package(
    default_visibility = ["//visibility:public"],
)

licenses(["notice"])  # Apache 2.0

java_library(
    name = "auth",
    srcs = glob(["*.java"]),
    deps = [
        "//java/google/registry/config",
        "//java/google/registry/security",
        "@com_google_appengine_api_1_0_sdk",
        "@com_google_auto_value",
        "@com_google_code_findbugs_jsr305",
        "@com_google_dagger",
        "@com_google_flogger",
        "@com_google_flogger_system_backend",
        "@com_google_guava",
        "@javax_servlet_api",
    ],
)
