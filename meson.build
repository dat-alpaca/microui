project('microui', 'c', meson_version: '>=1.2.0')

microui_includes = include_directories('src/')

microui = static_library(
    'microui',
    sources: files(
        'src/microui.h',
        'src/microui.c'
    ),
    include_directories: microui_includes
)

microui_dep = declare_dependency(
    link_with : microui,
    include_directories : microui_includes
)

meson.override_dependency('microui', microui_dep)