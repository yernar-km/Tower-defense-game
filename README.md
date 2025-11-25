<img width="1496" height="1321" alt="изображение" src="https://github.com/user-attachments/assets/085b3208-26b8-4f47-b272-782421f3f8cd" />

# Tower Defense Game

A 2D Tower Defense game built using Java and Swing. The game features multiple tower types, a map editor, sound effects, and a settings menu. Players must strategically place towers to defend against waves of enemies.

## Features

- **Three Tower Types**:
  - **Basic Tower**: High damage, single target.
  - **Area Tower**: Medium damage, area of effect.
  - **Slow Tower**: Low damage, slows enemy speed.

- **Map Editor**: Create and edit maps with different tile types (grass, road, start, finish, water).

<img width="1495" height="1246" alt="изображение" src="https://github.com/user-attachments/assets/ae638dbf-eb7d-4fe4-b409-ec736f21e074" />

- **Sound Effects**: Includes sound effects for tower placement, enemy damage, and background music.

- **Settings Menu**: Adjust sound volume and enable/disable sound.
<img width="1186" height="887" alt="изображение" src="https://github.com/user-attachments/assets/f4bc006b-c7af-4330-86d7-521b2b40baad" />

<img width="1167" height="882" alt="изображение" src="https://github.com/user-attachments/assets/cfcdca48-094a-40ee-ab19-0c936bfa332f" />



- **Wave System**: Progress through 10 increasingly difficult waves with stronger enemies.

- **HUD**: Displays money, lives, current wave, and score.
<img width="1496" height="1321" alt="изображение" src="https://github.com/user-attachments/assets/7aae8580-898f-45a8-bac8-d4fb3df33e92" />



## Project Structure

```
TowerDefense/
├── Yernar_map/
│   ├── GamePanel.java
│   ├── GamePanelWithPath.java
│   ├── MainMenu.java
│   ├── EditorPanel.java
│   ├── Editor.java
│   ├── SoundPlayer.java
│   
├── Tamerlan_towers/
│   ├── Tower.java
│   ├── BasicTower.java
│   ├── AreaTower.java
│   ├── SlowTower.java
│   ├── Enemy.java
│   
├── TowerDefenseWindow.java
├── MainMenu.java
├── SettingsMenu.java
├── TextureManager.java
├── Main.java
└── res/
    ├── tower images
    ├── enemy images
    ├── sound effects
    └── background music
```

## How to Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yernar-km/Tower-defense-game.git
   ```

2. **Ensure the following directory structure**:
   ```
   TowerDefense/
   ├── res/
   │   ├── tower images (basictower.png, areatower.png, slowtower.png)
   │   ├── enemy images (enemy1.png, enemy2.png, enemy3.png)
   │   ├── sound effects (BUYING.mp3, coin.wav, damage.wav, etc.)
   │   └── background music (background_music.wav)
   └── src/
       └── (all Java files)
   ```

3. **Compile and run**:
   ```bash
   javac -d . Main.java
   java Main
   ```

4. **Alternatively, run using an IDE**:
   - Import the project as a Java project.
   - Run the `Main` class.

## Controls

- **Main Menu**:
  - `PLAY`: Start the game.
  - `EDITOR`: Open the map editor.

- **In-Game**:
  - `1-3`: Select tower type to build.
  - `SPACE`: Start the next wave.
  - `P`: Toggle path preview (in editor mode).

- **Map Editor**:
  - Left-click: Place selected tile.
  - Drag: Place multiple tiles.
  - `S`: Save the map.

- **Settings Menu**:
  - Adjust volume slider to change sound volume.
  - Toggle sound on/off.

## Known Issues

- Some sound files may not play correctly depending on system configuration.
- Map editor does not validate paths between start and finish tiles.
- Enemy images may not display if the `res/enemy*.png` files are missing.
.

## Technologies Used

- Java (SE)
- Java Swing for GUI
- Java Sound API for audio
- ImageIO for image loading

## License

MIT License

---

This project is a collaborative effort between Yernar and Tamerlan, showcasing Java programming skills in game development.



