workspace(name = "cyber_ros_bridge")

# googletest (GTest and GMock)
new_http_archive(
    name = "gtest",
    build_file = "third_party/gtest.BUILD",
    sha256 = "58a6f4277ca2bc8565222b3bbd58a177609e9c488e8a72649359ba51450db7d8",
    strip_prefix = "googletest-release-1.8.0",
    url = "file:///home/tmp/googletest-release-1.8.0.tar.gz",
)

# gflags
git_repository(
    name = "com_github_gflags_gflags",
    commit = "28f50e0fed19872e0fd50dd23ce2ee8cd759338e",
    remote = "https://github.com/gflags/gflags.git",
)

bind(
    name = "gflags",
    actual = "@com_github_gflags_gflags//:gflags",
)

# glog
new_local_repository(
    name = "glog",
    build_file = "third_party/glog.BUILD",
    path = "/usr/local/include/glog",
)

# Google Benchmark
new_http_archive(
    name = "benchmark",
    build_file = "third_party/benchmark.BUILD",
    sha256 = "e7334dd254434c6668e33a54c8f839194c7c61840d52f4b6258eee28e9f3b20e",
    strip_prefix = "benchmark-1.1.0",
    url = "file:///home/tmp/benchmark-1.1.0.tar.gz",
)

# cpplint from google style guide
new_local_repository(
    name = "google_styleguide",
    build_file = "third_party/google_styleguide.BUILD",
    path = "/home/tmp/google_styleguide",
)

# eigen
new_http_archive(
    name = "eigen",
    build_file = "third_party/eigen.BUILD",
    sha256 = "04f8a4fa4afedaae721c1a1c756afeea20d3cdef0ce3293982cf1c518f178502",
    strip_prefix = "eigen-eigen-b9cd8366d4e8",
    url = "file:///home/tmp/eigen-3.2.10.tar.gz",
)

# CivetWeb (web server)
new_http_archive(
    name = "civetweb",
    build_file = "third_party/civetweb.BUILD",
    sha256 = "de7d5e7a2d9551d325898c71e41d437d5f7b51e754b242af897f7be96e713a42",
    strip_prefix = "civetweb-1.11",
    url = "file:///home/tmp/v1.11.tar.gz",
)

# curlpp
new_http_archive(
    name = "curlpp",
    build_file = "third_party/curlpp.BUILD",
    sha256 = "97e3819bdcffc3e4047b6ac57ca14e04af85380bd93afe314bee9dd5c7f46a0a",
    strip_prefix = "curlpp-0.8.1",
    url = "file:///home/tmp/curlpp-0.8.1.tar.gz",
)

#ros
new_local_repository(
    name = "ros",
    build_file = "third_party/ros.BUILD",
    path = "/home/tmp/ros",
)

#ros_indigo
new_local_repository(
    name = "ros_indigo",
    build_file = "third_party/ros_indigo.BUILD",
    path = "/opt/ros/indigo",
)

#ros_pkgs
new_local_repository(
    name = "ros_pkgs",
    build_file = "ros_bazel_builds/ros_pkgs.BUILD",
    path = "ros_pkgs/devel",
)

# PCL 1.7
# =======
# This requires libpcl-dev to be installed in your Ubuntu/Debian.
new_local_repository(
    name = "pcl",
    build_file = "third_party/pcl.BUILD",
    path = "/usr/local/include/pcl-1.7",
)

new_local_repository(
    name = "glew",
    build_file = "third_party/glew.BUILD",
    path = "/usr/include",
)

new_local_repository(
    name = "opengl",
    build_file = "third_party/opengl.BUILD",
    path = "/usr/include",
)

new_local_repository(
    name = "glfw",
    build_file = "third_party/glfw.BUILD",
    path = "/usr/include",
)

new_local_repository(
    name = "vtk",
    build_file = "third_party/vtk.BUILD",
    path = "/usr/include/vtk-5.8",
)

# Caffe
new_local_repository(
    name = "caffe",
    build_file = "third_party/caffe.BUILD",
    path = "/usr/include/caffe",
)
## tensorrt
new_local_repository(
    name = "tensorrt",
    build_file = "third_party/tensorrt.BUILD",
    path = "/usr/include/tensorrt",
)

# YAML-CPP
new_http_archive(
    name = "yaml_cpp",
    build_file = "third_party/yaml_cpp.BUILD",
    strip_prefix = "yaml-cpp-yaml-cpp-0.5.3",
    url = "https://github.com/jbeder/yaml-cpp/archive/yaml-cpp-0.5.3.zip",
)

new_http_archive(
    name = "qpOASES",
    build_file = "third_party/qpOASES.BUILD",
    sha256 = "e70b49586b58b8f5fd348e951f3c3094ed0ad371a96097a499f343a7aeec7dbe",
    strip_prefix = "qp-oases-3.2.1-1",
    url = "file:///home/tmp/qp-oases-3.2.1-1.zip",
)

# OSQP
new_local_repository(
    name = "osqp",
    build_file = "third_party/osqp.BUILD",
    path = "/usr/local/include/osqp/include",
)

# IpOpt
new_local_repository(
    name = "ipopt",
    build_file = "third_party/ipopt.BUILD",
    path = "/usr/local/ipopt/include/coin",
)

# ADOL-C
new_local_repository(
    name = "adolc",
    build_file = "third_party/adolc.BUILD",
    path = "/usr/local/adolc/include",
)

# Cuda
new_local_repository(
    name = "cuda",
    build_file = "third_party/cuda.BUILD",
    path = "/usr/local/cuda",
)

# Local-integ
new_local_repository(
    name = "local_integ",
    build_file = "third_party/local_integ.BUILD",
    path = "/usr/local/apollo/local_integ",
)

# Proj.4
new_http_archive(
    name = "proj4",
    build_file = "third_party/proj4.BUILD",
    strip_prefix = "proj.4-4.9.3",
    url = "file:///home/tmp/proj.4-4.9.3.zip",
)

# tinyxml2
new_http_archive(
    name = "tinyxml2",
    build_file = "third_party/tinyxml2.BUILD",
    strip_prefix = "tinyxml2-5.0.1",
    url = "file:///home/tmp/tinyxml2-5.0.1.zip",
)

#protobuf 3.3
http_archive(
    name = "com_google_protobuf",
    strip_prefix = "protobuf-3.3.0",
    url = "file:///home/tmp/protobuf-3.3.0.tar.gz",
)

#jsoncpp .so for adv_plat
new_local_repository(
    name = "jsoncpp",
    build_file = "third_party/jsoncpp.BUILD",
    path = "/usr/local/apollo/jsoncpp/",
)

#adv_plat
new_http_archive(
    name = "adv_plat",
    build_file = "third_party/adv_plat.BUILD",
    sha256 = "0a58dadab924b520d5b5a58ef82fc0f76c2aa4feaaabd49ec9873228c125d513",
    url = "https://github.com/ApolloAuto/apollo-contrib/releases/download/v3.0.0/plat-sw-3.0.0.1.zip",
)

# qt
new_local_repository(
    name = "qt",
    build_file = "third_party/qt.BUILD",
    path = "/usr/local/Qt5.5.1/5.5/gcc_64",
)

new_local_repository(
    name = "fastrtps",
    build_file = "third_party/fastrtps.BUILD",
    path = "/usr/local/fast-rtps",
)

# grpc
http_archive(
    name = "com_github_grpc_grpc",
    url = "https://github.com/grpc/grpc/archive/v1.14.2.tar.gz",
    strip_prefix = "grpc-1.14.2",
)

load("@com_github_grpc_grpc//bazel:grpc_deps.bzl", "grpc_deps")

grpc_deps()

# python
new_local_repository(
    name = "python27",
    build_file = "third_party/python27.BUILD",
    path = "/usr",
)

# PyTorch
new_local_repository(
    name = "pytorch",
    build_file = "third_party/pytorch.BUILD",
    path = "/usr/local/apollo/libtorch",
)

# PyTorch GPU
new_local_repository(
    name = "pytorch_gpu",
    build_file = "third_party/pytorch_gpu.BUILD",
    path = "/usr/local/apollo/libtorch_gpu",
)

