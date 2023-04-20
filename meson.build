project(
  'cfg-if',
  'rust',
  version : '1.0',
  license :'MIT OR Apache-2.0',
  default_options : ['rust_std=2018'],
)

rc = meson.get_compiler('rust')

rust_args = [
  '--cfg', 'feature="default"',
  '--cfg', 'feature="derive"',
  '--cfg', 'feature="printing"',
  '--cfg', 'feature="clone-impls"',
  '--cfg', 'feature="cfg-if"',
  '--cfg', 'feature="use_cfg_if"',
]

lib = static_library(
  'cfg_if',
  'src/lib.rs',
  rust_args : rust_args,
  link_with : [],
  rust_crate_type : 'rlib'
)
