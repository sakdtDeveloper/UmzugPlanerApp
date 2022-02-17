# UmzugPlanerApp

## Navigation Component

Navigation graph + NavHost + NavController

###Safe Args Plugin:
a Gradle plugin that will assist you with type safety when passing data between fragments.
un plugin Gradle qui vous aidera à assurer la sécurité des types lors du passage de données entre fragments.
ein Gradle-Plugin, das Sie bei der Typsicherheit unterstützt, wenn Sie Daten zwischen Fragmenten übergeben.





### Navigation Dependency

build.gradle(Project)
buildscript {
    ext {
     nav_version = "2.3.1"
        }
     dependencies {
             classpath "androidx.navigation:navigation-safe-args-gradle-plugin:$nav_version"
         }
        }

build.gradle(Module)
plugins {
     id 'androidx.navigation.safeargs.kotlin'
}
dependencies {
        implementation "androidx.navigation:navigation-fragment-ktx:$nav_version"
        implementation "androidx.navigation:navigation-ui-ktx:$nav_version"
}
### Navigation Graph

The navigation graph is an XML file that provides a visual representation of navigation in your app.
The file consists of destinations which correspond to individual activities and fragments as well as actions between them which can be used in code to navigate from one destination to another.

Graphique de navigation : Le graphique de navigation est un fichier XML qui fournit une représentation visuelle de la navigation dans votre application.
Le fichier se compose de destinations qui correspondent à des activités et à des fragments individuels, ainsi que d'actions entre eux qui peuvent être utilisées dans le code pour naviguer d'une destination à une autre.

Der Navigationsgraph: Der Navigationsgraph ist eine XML-Datei, die eine visuelle Darstellung der Navigation in Ihrer Anwendung bietet.
Die Datei besteht aus Destinationen, die einzelnen Aktivitäten und Fragmenten entsprechen, sowie aus Aktionen zwischen ihnen, die im Code verwendet werden können, um von einem Destination zu einem anderen zu navigieren.

### NavHost

A NavHost is used to display destinations from a navigation graph within an activity.
When you navigate between fragments, the destination shown in the NavHost is updated.

Un NavHost est utilisé pour afficher les destinations d'un graphique de navigation dans une activité.
Lorsque vous naviguez entre les fragments, la destination affichée dans le NavHost est mise à jour.

Ein NavHost wird verwendet, um Destinationen aus einem Navigationsdiagramm innerhalb einer Aktivität anzuzeigen.
Wenn Sie zwischen Fragmenten navigieren, wird das im NavHost angezeigte Navigationsziel aktualisiert.

### NavController

The NavController object lets you control the navigation between destinations displayed in the NavHost.
With the Navigation component, you can call the NavController's navigate() method to swap the fragment that's displayed.

L'objet NavController vous permet de contrôler la navigation entre les destinations affichées dans le NavHost.
Avec le composant Navigation, vous pouvez appeler la méthode navigate() du NavController pour changer le fragment qui s'affiche.

Mit dem NavController-Objekt können Sie die Navigation zwischen den im NavHost angezeigten Zielen steuern.
Mit der Komponente Navigation können Sie die Methode navigate() des NavControllers aufrufen, um das angezeigte Fragment zu wechseln.