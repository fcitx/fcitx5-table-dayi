set(ICON48
    fcitx-dayi3.png)

install(FILES
    ${ICON48}
    DESTINATION share/icons/hicolor/48x48/apps)

foreach(icon ${ICON48})
    string(REPLACE "fcitx-" "" icon_new ${icon})
    install(FILES ${icon} RENAME ${icon_new} DESTINATION share/fcitx/imicon)
endforeach()
