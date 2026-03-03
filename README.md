# Krunker Admin Panel

This project provides an admin panel for managing maps and players in Krunker. It includes functionalities for both map makers and map admins.

---

## Screenshots



---

## Functionalities

### General Features
- **Open Admin Panel**: Press `0` to open the admin panel.
- **Navigate Menu**: Use `J` (down) and `K` (up) to navigate through the menu options.
- **Select Option**: Press `L` to select an option.
- **Go Back**: Press `H` to return to the previous menu.
- **Close Admin Panel**: Press `C` to close the admin panel.

### Map Admin Functionalities
- **Kill**: Instantly eliminate a player.
- **Freeze**: Temporarily freeze a player.
- **Teleport To Player**: Teleport yourself to a specific player.
- **Summon Player**: Bring a player to your location.
- **Go To Point of Interest (POI)**: Teleport to predefined map locations.
- **Switch Team**: Change a player's team.
- **Kick Player**: Remove a player from the game.
- **Ban Player**: Permanently ban a player from the game.

### Map Maker Functionalities
- **Define Points of Interest (POI)**: Add predefined locations on the map for quick teleportation.
- **Customize Admin Options**: Modify the available admin options in the `client.krnk` file.
- **Player Management**: Use the admin panel to manage players during map testing.

---

## How to Use

### As a Map Maker
1. Open the `client` side.
2. Add or modify Points of Interest (POI) in the `ADMIN_POI` object. Example:
   ```krnk
   obj[] ADMIN_POI = obj[{
       name: 'Spawn Point',
       position: { x: 0, y: 0, z: 0 }
   }, {
       name: 'Sniper Tower',
       position: { x: 100, y: 50, z: 100 }
   }];
   ```
   You can also customize the keybindings with the 'ADMIN_OPEN', 'ADMIN_UP', 'ADMIN_DOWN', 'ADMIN_SELECT', 'ADMIN_BACK', and 'ADMIN_CLOSE' keys, and available admin options in the `admin.options` array.
3. Test the map by running the game and using the admin panel to navigate and manage players.

### As a Map Admin
1. Start the game and press `0` to open the admin panel.
2. Use the navigation keys (`J`, `K`, `L`, `H`, `C`) to manage players and interact with the map.
3. Select options like `Kill`, `Freeze`, `Kick`, or `Ban` to manage players.
4. Use the `Go To` option to teleport to predefined Points of Interest (POI).

---

## Notes
- Ensure the `client` side is properly configured before starting the game.
- The admin panel is designed to be intuitive and responsive, with support for cycling through menu options when the list exceeds the visible area.
- For any issues or feature requests, contact the development team.

---

Enjoy managing your Krunker players with ease!
