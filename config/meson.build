if omx_target == 'rpi'
  sub = 'rpi'
elif omx_target == 'bellagio'
  sub = 'bellagio'
elif omx_target == 'zynqultrascaleplus'
  sub = 'zynqultrascaleplus'
elif omx_target == 'tizonia'
  sub = 'tizonia'
elif omx_target == 'hisilicon'
  sub = 'hisilicon'
else
  # No config file defined for the 'generic' target
  sub = ''
endif

if sub != ''
  subdir (sub)
  # Used by tests to load the proper conf file
  omx_config_dir = join_paths (meson.current_source_dir(), sub)
else
  omx_config_dir = ''
endif
