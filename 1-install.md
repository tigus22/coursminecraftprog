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
curl -o ./plugins/scriptcraft.jar https://scriptcraftjs.org/download/latest/scriptcraft-3.2.1/scriptcraft.jar
curl -o server.properties 
```

# Tester votre installation
Afin de tester si votre installation fonctionne il faut démarrer votre serveur spigot et démarrer Minecraft par la suite.

Alors dans la même fenêtre gitbash que précédemment, copier cette commande pour démarrer le serveur spigot:  
```
java -Xms1G -Xmx1G -XX:+UseConcMarkSweepGC -jar spigot-1.12.2.jar
```
Ensuite vous pouvez démarrer Minecraft en multiplayer.
Cliquez sur `Add server`, puis dans la case `Server address` inscrivez `localhost`
Rejoignez le serveur, et ouvrez une ligne de commande avec la touche `é`
Vous verrez alors une ligne de commande commençant par un ` / `.
Essayez une commande comme `js echo("Ça sent la nature!")` 

Vous devriez voir votre message apparaître à l'écran.

Si c'est le cas, votre installation est réussie!

## Vérifier installation de Node.js

```
node -v
```
