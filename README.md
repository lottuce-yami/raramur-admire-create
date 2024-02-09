# Raramur: Admire & Create modpack
![modpack logo](icon.png)

## Description
This modpack is my attempt to create something vanilla-friendly, but exciting to explore and to build creative projects in - a combination of sandbox and RPG, as Minecraft should be. It is my first serious modpack and I am not familiar with all of the mods to a 100% extent, but I play this modpack myself and refine it, one step at a time, as I explore. You can read more about the features of the modpack and get the spirit that I am trying to create on the [CurseForge](https://www.curseforge.com/minecraft/modpacks/raramur-admire-create) page, but the best way to familiarize yourself is, of course, to play it!

## How to build
To make use of certain metadata, like optional mods and external files, you will need to build using **packwiz-installer**. This way you can exclude the largest (and, by coincidence, cosmetic) mods to reduce the modpack's size drastically.
> [!IMPORTANT]
> You will need to extract any .zip files in the `emotes` folder, because those cannot be read by the mod in compressed format.

> [!WARNING]
> This will install the modpack with the latest changes from this repository. If you want a more stable approach, consider downloading a release and replacing the URL with a local file path.  

### Client-side
1. Prepare the folder where you want to install the modpack: create an empty Prism Launcher or MultiMC instance with Minecraft of version `1.20.1` and Forge of version `47.2.0`.
2. Download the latest release of [packwiz-installer-bootstrap](https://github.com/packwiz/packwiz-installer-bootstrap) and put it in the instance folder (`.minecraft`).
3. Run `java -jar packwiz-installer-bootstrap.jar -s client https://lottuce-yami.github.io/raramur-admire-create/pack.toml`.
4. Proceed with the GUI, check the desired optional mods, and manually install any mods that are excluded from the API.

### Server-side
1. Prepare the folder where you want to install the modpack: download the Forge server core of version `47.2.0` and install it.
2. Download the latest release of [packwiz-installer-bootstrap](https://github.com/packwiz/packwiz-installer-bootstrap) and put it in the server folder.
3. Run `java -jar packwiz-installer-bootstrap.jar -g -s server https://lottuce-yami.github.io/raramur-admire-create/pack.toml`.
4. Read the console and manually install any mods that are excluded from the API.

> [!TIP]
> If you simply want to check the integrity of the repository, download [packwiz](https://github.com/packwiz/packwiz) and run `packwiz cf export -o raramur-admire-create.zip` to get the modpack in CurseForge format and compare it with the released version.
