cc_library(
  name = 'lib',
  extra_cppflags = [
    '-Wno-float-equal',
  ],
  srcs = [
    'lapi.c',
    'lauxlib.c',
    'lbaselib.c',
    'lbitlib.c',
    'lcode.c',
    'lcorolib.c',
    'lctype.c',
    'ldblib.c',
    'ldebug.c',
    'ldo.c',
    'ldump.c',
    'lfunc.c',
    'lgc.c',
    'linit.c',
    'liolib.c',
    'llex.c',
    'lmathlib.c',
    'lmem.c',
    'loadlib.c',
    'lobject.c',
    'lopcodes.c',
    'loslib.c',
    'lparser.c',
    'lstate.c',
    'lstring.c',
    'lstrlib.c',
    'ltable.c',
    'ltablib.c',
    'ltm.c',
    'lundump.c',
    'lvm.c',
    'lzio.c',
  ],
  deps = [
    '#dl',
    '#rt',
  ]
)

cc_binary(
  name = 'luac',
  srcs = [
    'luac.c',
  ],
  deps = [
    '#readline',
    ':lib',
  ]
)

cc_binary(
  name = 'lua',
  srcs = [
    'lua.c',
  ],
  deps = [
    '#readline',
    ':lib'
  ]
)
