cxx_library(
  name = 'fann',
  header_namespace = '',
  exported_headers = subdir_glob([
    ('src/include', '*.h'),
    ('src/include', '*.hpp'),
  ]),
  srcs = glob([
    'src/*.c',
    'src/*.cpp',
  ]),
  platform_compiler_flags = [
    ('default', ['-DDISABLE_PARALLEL_FANN']),
    ('^macos.*', ['-DDISABLE_PARALLEL_FANN']),
  ],
  visibility = [
    'PUBLIC',
  ],
)
