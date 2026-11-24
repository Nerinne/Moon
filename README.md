
rayitas -> vcs -> share project on github
vcs cambia a git -> hacer commit (si se necesita) -> hacer push

encima de cualquier boton -> refactor -> style -> marcar todo y ponerle nombre
app -> res -> values -> styles.xml

dentro de styles.html:

<style name="BotonSignup" parent="Widget.MaterialComponents.Button.OutlinedButton">
        <item name="android:layout_width">0dp</item>
        <item name="android:layout_height">60</item>
        <item name="android:backgroundTint">@color/Doreja1</item>
        <item name="android:textColor">@color/Doreja2</item>
    </style>
    
    <style name="BotonCancel" parent="Widget.MaterialComponents.Button.OutlinedButton">
        <item name="android:layout_width">0dp</item>
        <item name="android:layout_height">wrap_content</item>
        <item name="android:textColor">@color/Doreja1</item>
        <item name="cornerRadius">8dp</item>
        <item name="strokeColor">@color/Doreja1</item> //android:color/uwu <- de la libreria de android de colores
        <item name="strokeWidth">1dp</item>
    </style>

crear una nueva activity
file -> new -> activity -> emptyViewsActivity -> signup (añadir el git)
Copiar todo (menos la cabecera) de main.xml a signup

signup.xml:
  imageview
  3 text imput
  2 botones: signup y cancel
  opcional añadir fotos a los fondos de pantalla

<Button
        android:id="@+id/botonSignup"
        android:layout_height="wrap_content"
        android:layout_width="0dp"
        app:layout_constraintStart_toEndOf="@id/guideline1"
        app:layout_constraintEnd_toEndOf="@id/guideline2"
        app:layout_constraintTop_toBottomOf="@id/logo"
        android:text="SignUp"
        style="@style/BotonSignup"
        />

    <Button
        android:id="@+id/botonCancel"
        android:layout_height="wrap_content"
        android:layout_width="0dp"
        app:layout_constraintStart_toEndOf="@id/guideline1"
        app:layout_constraintEnd_toEndOf="@id/guideline2"
        app:layout_constraintTop_toBottomOf="@id/botonSignup"
        android:text="Cancel"
        style="@style/BotonCancel"
        />
