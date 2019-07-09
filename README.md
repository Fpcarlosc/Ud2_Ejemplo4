# Ud2_Ejemplo4
_Ejemplo 4 de la Unidad 2._ 

Vemos un ejemplo del ViewGroup _FrameLayout_ al que le añadimos texto, una imagen y un botón.
Modificando el valor del atributo _visibility_ (_visible_, _invisible_ o _gone_) podemos ver cómo los elementos se muestran u ocultan dejando su espacio libre o no.

Sólo hemos de fijarnos en el fichero _main_activity.xml_:

```
<FrameLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="@string/uno" />

    <ImageView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:src="@drawable/android_black"
        android:visibility="gone"/>

    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="@string/boton"
        android:visibility="invisible"/>

</FrameLayout>
```
Los textos del _TextView_ y del _Button_ se han insertado en el fichero _values/strings.xml_ y accedemos a él usando el símbolo @:
```
<resources>
    <string name="app_name">Ud2_Ejemplo4</string>
    <string name="uno">Uno</string>
    <string name="boton">Botón</string>
</resources>
```

_Imagen de material.io/tools/icons (Licencia Apache 2.0)_

