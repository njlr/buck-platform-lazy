genrule(
  name = 'always-fails', 
  out = 'never.h', 
  cmd = 'exit 1', 
)

cxx_binary(
  name = 'app', 
  header_namespace = '', 
  platform_headers = [
    ('nosuchplatform', { 'never.h': ':always-fails' }), 
    # ('.*', { 'never.h': ':always-fails' }), 
  ], 
  srcs = [
    'app.cpp', 
  ], 
)
