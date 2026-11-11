if get_option('blob')
  subdir('blob')
elif get_option('windows_only')
  subdir('rizin')
  subdir('rz-bin')
  subdir('rz-asm')
else
  subdir('rz-ar')
  subdir('rz-hash')
  subdir('rz-run')
  subdir('rz-asm')
  subdir('rz-bin')
  subdir('rizin')
  subdir('rz-gg')
  subdir('rz-diff')
  subdir('rz-find')
  subdir('rz-sign')
  subdir('rz-ax')
endif
if get_option('enable_rz_test') and not get_option('windows_only')
  subdir('rz-test')
endif

if get_option('windows_only')
  install_man(
    'man/rz-bin.1',
    'man/rizin.1',
    'man/rz-asm.1',
  )
else
  install_man(
    'man/rz-ar.1',
    'man/rz-bin.1',
    'man/rizin.1',
    'man/rz-diff.1',
    'man/rz-find.1',
    'man/rz-gg.1',
    'man/rz-hash.1',
    'man/rz-run.1',
    'man/rz-asm.1',
    'man/rz-ax.1',
    'man/rz-sign.1',
    'man/rz-test.1',
    'man/rz-esil.7',
  )
endif
