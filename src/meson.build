gobj_dep   = dependency('gobject-2.0', version : '>=2.44.0')
glib_dep   = dependency('glib-2.0',    version : '>=2.44.0')
glibmm_dep = dependency('glibmm-2.4',  version : '>=2.44.0')
gtkmm_dep  = dependency('gtkmm-3.0',   version : '>=3.4.0')
xml_dep    = dependency('libxml-2.0',  version : '>=2.7.8')
curl_dep   = dependency('libcurl',     version : '>=7.24.0')
secret_dep = dependency('libsecret-1', version : '>=0.12')
sigcpp_dep = dependency('sigc++-2.0',  version : '>=2.2.11')
thread_dep = dependency('threads')

malgtk_deps = [gobj_dep, glib_dep, glibmm_dep, gtkmm_dep, xml_dep, curl_dep, secret_dep, thread_dep]

malgtk_src = files(['main.cpp',
                    'application.cpp',
                    'user_info.cpp',
                    'mal.cpp',
                    'malitem.cpp',
                    'anime.cpp',
                    'manga.cpp',
                    'xml_reader.cpp',
                    'xml_writer.cpp',
                    'anime_serializer.cpp',
                    'manga_serializer.cpp',
                    'text_util.cpp',
                    'gui/malgtk_cellrenderer_score.c',
                    'gui/cellrendererscore.cpp',
                    'gui/main_window.cpp',
                    'gui/password_dialog.cpp',
                    'gui/malitem_list_view.cpp',
                    'gui/anime_list_view.cpp',
                    'gui/manga_list_view.cpp',
                    'gui/increment_entry.cpp',
                    'gui/fancy_label.cpp',
                    'gui/date_widgets.cpp'])

malgtk = executable('mal-gtk', malgtk_src,
                    include_directories : libmalgtk_inc,
                    dependencies : malgtk_deps,
                    install      : true)  
