# Lomiri UI Toolkit

Lomiri UI Toolkit offers elements for graphical applications to make beautiful interfaces for your app. It is built on top of Qt5 & QML and offers support for a wide variety of form factors.

Your app can:

- Run on smartphones, tablets, laptops & desktops
- Use hardware acceleration by default
- Quickly allow for functional apps with less effort

Want to start magic? Use Lomiri UI Toolkit! 😊

To use this content snap in your apps, add the following description to your `snapcraft.yaml`:

```
plugs:
  lomiri-ui-toolkit:
    interface: content
    target: $SNAP/lomiri-ui-toolkit
    default-provider: lomiri-ui-toolkit-core24
```

And export the following environment variables for your app to find it:

```
export LD_LIBRARY_PATH=${SNAP}/usr/lib/${ARCH}:${SNAP}/lib/${ARCH}:${SNAP}/lomiri-ui-toolkit/usr/lib/${ARCH}
export QT_PLUGIN_PATH=${SNAP}/usr/lib/${ARCH}/qt5/plugins:${SNAP}/lomiri-ui-toolkit/usr/lib/${ARCH}/qt5/plugins
export QML2_IMPORT_PATH=${SNAP}/lib/${ARCH}:${SNAP}/usr/lib/${ARCH}/qt5/qml:${SNAP}/lomiri-ui-toolkit/lib/${ARCH}:${SNAP}/lomiri-ui-toolkit/usr/lib/${ARCH}/qt5/qml
export XDG_DATA_DIRS=$XDG_DATA_DIRS:${SNAP}/usr/share:${SNAP}/lomiri-ui-toolkit/usr/share
```

Lomiri is the continuation of the Unity8 efforts started by Canonical Ltd., maintained by the UBports community.
