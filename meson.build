project('flowtime', ['c', 'vala'],
          version: '6.1',
    meson_version: '>= 0.60.0',
  default_options: [ 'warning_level=2',
                   ],
)

app_id = 'io.github.diegoivanme.flowtime'
i18n = import('i18n')



subdir('data')
subdir('src')
subdir('po')

gnome.post_install(
  glib_compile_schemas: true,
  gtk_update_icon_cache: true,
  update_desktop_database: true,
)
