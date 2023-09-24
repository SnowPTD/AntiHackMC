# AntiHackMC Minecraft plugins

[![Version](https://img.shields.io/badge/版本-v1.2.2-blue.svg)](https://github.com/yourusername/antihackmc)
[![Minecraft Version](https://img.shields.io/badge/Minecraft-1.20.1-green.svg)](https://www.minecraft.net/)

AntiHackMC is an anti-cheating plug-in for Minecraft servers, which aims to provide a safe and fair gaming environment. This plugin uses various detection techniques to check whether players have used any cheating programs or illegal modifications.

## Features

- **Anti Hack**：AntiHackMC Can prevent fast cheats
- **Custom configuration**：you can customize the plug-in configuration according to the needs of the server to achieve the best gaming experience and detection results.
- **Simple and easy to use**：Installing and configuring AntiHackMC is very simple, just put the plug-in file into the server's plug-in directory to start using it.

## download

1. Download the latest version of the AntiHackMC plugin.
2. Place the plugin file (usually a file ending in `.jar`) into the plugins directory of your Minecraft server.
3. Restart the server and the plugin will automatically load and initialize.

## Configuration

You can find the `config.yml` file in the plugin directory, which is the configuration file of the plugin. You can open this archive with any text editor for custom configuration.

Here are some common configuration options:

```yaml
# Whether to enable anti-cheating function
enabled: true

# Threshold for detecting values
AntiHack:
    enabled: true
    threshold:
        fly: 0.3 # hreshold for detecting values
        speed: 0.78 # This is speed, This will not calculate the potion speed.
        speed_Level1: 0.8 #Threshold after using speed effect(Level 1)
        speed_Level2: 0.84 #Threshold after using speed effect(Level 2)
        Level3UP: 0.25 #Every time the effect rises by 1 level, this value will be used to increase the threshold.

GameMode:
    enabled: true
    SPECTATOR: "!c"
    SURVIVAL: "!s"
```


## Death record
If you die in the game, the plugin will send you a message
The message like this: [AntiHackMC] You die in X:00 Y:00 Z:00 World:World
