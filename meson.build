project(
  'fmt', ['cpp'],
  default_options : ['cpp_std=c++20'],
  version : '8.1.1',
)

fmt_include = include_directories('include')

subdir('src')

fmt_lib = static_library(
  'fmt',
  fmt_src,
  include_directories : fmt_include,
)

fmt_dep = declare_dependency(
  link_with : fmt_lib,
  include_directories : fmt_include,
)

