# Installation des modules requis

* Télécharger et installer [Java](https://www.java.com/en/download/ "Java").
* Télécharger et installer [Minecraft](https://minecraft.net/en-us/store/minecraft/ "Minecraft").
* Télécharger et installer [Git for Windows](https://gitforwindows.org/, "Git for Windows").
* Télécharger BuiltTools.jar à partir de SpigotMC: 
    + Aller au menu démarrer de Windows, et taper "git bash" et faites enter.
      Une fenêtre de commandes MINGW64 devrait apparaître.
    + Maintenant, il faut copier/coller les commandes suivantes pour télécharger BuilTools automatiquement au bon endroit.
        
```
mkdir .\cmp
mkdir .\cmp\buildtools
cd cmp\buildtools
curl -o BuildTools.jar https://hub.spigotmc.org/jenkins/job/BuildTools/lastSuccessfulBuild/artifact/target/BuildTools.jar

```
