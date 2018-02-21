# Installation des modules requis

* Télécharger et installer [Visual Studio Code](https://code.visualstudio.com/download).
* Télécharger et installer [Java](https://www.java.com/en/download/ "Java").
* Télécharger et installer [Minecraft](https://minecraft.net/en-us/store/minecraft/ "Minecraft").
* Télécharger et installer [Git for Windows](https://gitforwindows.org).
* Télécharger et installer [Node.js](https://nodejs.org/en/download/).
* Télécharger BuiltTools.jar à partir de SpigotMC.  Ne vous en faites pas, juste à suivre le tuto ci-dessous, ça devrait bien se passer: 
    + Aller au menu démarrer de Windows, et taper "git bash" et faites enter.
      Une fenêtre de commandes MINGW64 devrait apparaître.
    + Maintenant, il faut copier/coller les commandes suivantes pour télécharger BuildTools automatiquement au bon endroit.
    *Attendez que l'installation soit terminée avant de continuer!*
        
```
mkdir ./cmp
mkdir ./cmp/buildtools
cd cmp/buildtools
curl -o BuildTools.jar https://hub.spigotmc.org/jenkins/job/BuildTools/lastSuccessfulBuild/artifact/target/BuildTools.jar
java -jar BuildTools.jar
mkdir ../minecraft-server
cp spigot*.jar ../minecraft-server/
cp craftbukkit*.jar ../minecraft-server/
cd ../minecraft-server
echo "eula=true">eula.txt
java -jar spigot-1.12.2.jar
```
