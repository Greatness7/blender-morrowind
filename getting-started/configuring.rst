Configuring
===========

Addon Preferences
-----------------

.. image:: ../_static/preferences.png

- **Check for updates**
    Allows you to quickly and conveniently update the plugin to the latest version. This button requires a working internet connection, and will simply check the plugin repository for a newer version than is currently installed. If an update is available you will then be able to upgrade and view the changelog with an additional button press. Be sure to restart Blender after updating any addon!
- **Scale Correction**
    Adjusts how assets will be scaled upon import and export. Imported assets will be scaled down by the given value and exported assets will be scaled up by the same amount. This is useful as the very large native scale of Morrowind assets can cause issues such as viewport clipping. In most cases there is no need to change this value from the default ``0.01``.
- **Texture Paths**
    Provides a way to specify where the importer should look for texture files. This is necessary as Blender requires absolute paths for texture access despite Morrowind assets only providing relative paths. Multiple texture paths can be specified and the importer will always start with the top of the list and move downward until it resolves a valid texture.


Import Options
--------------

- **Vertex Precision**
    Rounding precision used when optimizing vertex data. This feature is similar to Blender's native *Merge by Distance*, but differs in that it respects additional vertex data such as normals, uv coordinates, and vertex colors. In most cases there is no need to change this value from the default ``0.001``.
- **Attach Keyframe Data**
    Attach animations from the corresponding .kf file. Requires file names to be an exact match. (e.g. when enabled importing 'xbase_anim.nif' will attach animations from 'xbase_anim.kf')
- **Discard Root Transforms**
    Discard the root object's transformations. In-game root transforms are overwriten with the values provided by individual cell references. Despite this some meshes do define root transformations, which can lead to unintended results if accidentally applied before exporting.
- **Preserve Material Names**
    Preserve material names from the source file. If unchecked materials will be renamed based on their assigned textures.


Export Options
--------------

- **Vertex Precision**
    Rounding precision used when optimizing vertex data. This feature is similar to Blender's native *Merge by Distance*, but differs in that it respects additional vertex data such as normals, uv coordinates, and vertex colors. In most cases there is no need to change this value from the default ``0.001``.
- **Only Collection**
    Only export objects from the active collection.
- **Only Selected**
    Only export objects that are selected.
- **Export Animations**
    Uncheck to skip all animation data during export.
- **Extract Keyframe Data**
    Extract animations and visuals to corrosponding 'x.kf' and 'x.nif' files. (e.g. exporting 'base_anim.nif' will create additional 'xbase_anim.nif' and 'xbase_anim.kf' files)
- **Preserve Material Names**
    Preserve material names from the source file. If unchecked materials will be renamed based on the assigned textures.
