# README - Application de localisation avec OpenStreetMap

## Objectif du TP

L’objectif de ce TP est de créer une application Android capable d’afficher une carte interactive et de récupérer la position actuelle de l’utilisateur en temps réel.

L’application permet :

* d’afficher une carte OpenStreetMap,
* de demander la permission de localisation,
* d’écouter les changements de position,
* d’ajouter un marker sur la position actuelle,
* de zoomer automatiquement sur la localisation,
* d’afficher une boîte de dialogue si le GPS est désactivé.

---

# Technologies utilisées

* Android Studio
* Java
* OpenStreetMap (OSMdroid)
* LocationManager Android

---

# Fonctionnalités réalisées

## Affichage de la carte

L’application utilise la bibliothèque OSMdroid pour afficher une carte OpenStreetMap sans utiliser Google Maps API.

## Permission de localisation

L’application demande dynamiquement la permission ACCESS_FINE_LOCATION afin d’accéder à la position de l’utilisateur.

## Géolocalisation en temps réel

Le service LocationManager écoute les changements de position via NETWORK_PROVIDER.

## Ajout d’un marker

À chaque changement de position, un marker est ajouté ou déplacé sur la carte.

## Zoom automatique

La caméra se centre automatiquement sur la position actuelle avec un niveau de zoom adapté.

## Vérification du GPS

Si le GPS est désactivé, une boîte de dialogue s’affiche pour demander à l’utilisateur de l’activer.

---

# Permissions utilisées

```xml
<uses-permission android:name="android.permission.INTERNET"/>
<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION"/>
<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION"/>
```

---

# Dépendance Gradle

```gradle
implementation("org.osmdroid:osmdroid-android:6.1.18")
```

---

# Résultat obtenu

L’application affiche correctement :

* la carte OpenStreetMap,
* la position actuelle de l’utilisateur,
* le marker dynamique,
* le déplacement automatique de la caméra,
* les mises à jour de localisation en temps réel.

---

# Conclusion

Ce TP a permis de découvrir l’utilisation des services de géolocalisation Android ainsi que l’intégration d’une carte interactive avec OpenStreetMap.
L’application réalisée fonctionne sans Google Maps API et permet de suivre la position de l’utilisateur en temps réel de manière simple et efficace.


https://github.com/user-attachments/assets/62b55cd9-00ee-4849-b8ca-7c1fabd808d0



