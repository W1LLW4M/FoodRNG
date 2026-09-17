# 🍔 FoodRNG — Development & Changelog

**FoodRNG** is a browser-based luck and collection game where players roll for different food squishies, discover new rarities, build their collection, and try to find the rarest foods. The project started as a very simple game and gradually grew into a much larger RNG game with hundreds of mechanics packed into a single HTML file.

### 🎮 How to Play

Playing the game is simple: press the **ROLL** button and wait for the rolling animation to finish. The game chooses a food and rarity using its RNG system before displaying the final result. Every food has its own ID, name, emoji, and rarity, and discovering a food for the first time adds it to your collection. Players can also earn coins, increase their Luck level, complete quests, unlock achievements, use Auto-Roll, and equip foods they have discovered.

### 💻 How It Was Coded

The game was built as a **single HTML file**, meaning the HTML, CSS, JavaScript, food data, animations, and game systems are all contained inside one file. HTML was used to create the game's structure and different screens, CSS was used for the visual design, animations, glowing effects, buttons, panels, backgrounds, and responsive layout, while JavaScript controls the actual gameplay and RNG system.

The food database is stored inside the JavaScript as an array of food objects. Each food has information such as its unique ID, name, emoji, and rarity, allowing the game to randomly select foods while also keeping track of which ones the player has discovered.

The RNG system uses different probability weights for each rarity. Common foods have much higher chances of appearing, while Legendary, Mythic, Divine, and Secret foods become extremely difficult to obtain. The Luck system modifies some of the rarity chances, giving players a reason to keep upgrading their Luck.

### 💾 Saving System

The game uses **localStorage** to save progress directly inside the browser. This means things such as coins, rolls, Luck, discovered foods, Shiny foods, Golden foods, equipped foods, quests, achievements, streaks, and other progress can remain saved after closing and reopening the game. There is no account, server, or database required.

### ✨ Special Variants

The game also includes special versions of foods. **Shiny** foods have a special ✨ effect and are tracked separately from normal discoveries, while **Golden** foods have their own special effects and tracking. These variants make already-rare foods even more exciting because players can potentially get an unusual version of a food they already discovered.

### 📖 Collection System

The Collection works like a digital food book. Every food has its own entry, and undiscovered foods remain locked until the player rolls them. Players can search the collection, filter foods by rarity, see discovered and undiscovered foods, identify Shiny and Golden variants, and equip foods they have already discovered.

### 🏆 Progression

As the game developed, more progression systems were added. Players can earn coins from rolling and discovering foods, complete quests for additional rewards, unlock achievements for reaching different milestones, build streaks, claim daily rewards, and upgrade their Luck. V3 also introduced Auto-Roll, allowing players to automatically roll after unlocking the required milestone.

### 📜 Changelog

**V1 — The Beginning**
V1 was the original simple version of **FoodRNG**. It contained only **15 food squishies** and focused mainly on rolling, seeing the result, and collecting foods. It was intentionally simple and acted as the foundation for the later versions.

**V2 — The Big Expansion**
V2 increased the collection from 15 foods to **50 unique food squishies**. It added more rarities, Shiny and Golden variants, Luck upgrades, coins, quests, achievements, daily rewards, streaks, statistics, collection filters, and better animations. V2 also introduced a much more complete saving system using localStorage.

**V3 — The Massive Upgrade**
V3 expanded the collection to **167 unique food squishies** and introduced the new **Secret** rarity, which is even rarer than Divine. Legendary, Mythic, Divine, and Secret pulls received increasingly impressive animations and visual effects. V3 also expanded the collection system, progression, Auto-Roll, quests, achievements, variants, statistics, and overall UI.

**V3.1 Lightweight — The Enlightening**
V3.1 Lightweight added a light mode feature, allowing users to choose between a light and dark background.

### 🛠️ Development Team

The game was developed as a collaborative project. **W1LLW4M** worked on editing and improving the game, including helping shape the versions and features as the project expanded. **Dino** helps code more minor updates such as bug fixes and accessibility features. **Kuro** tested the game and helped find bugs, glitches, and things that needed improvement. **Kuro** is also the Admin in the Discord server.

The development process was basically: **build → test → find bugs → fix → add features → test again → improve the design**. 🧪

One example was a bug where the food emoji could sometimes remain stuck on a previous result after rolling a different food. The game's display system was changed so that the most recent roll is stored separately and shown correctly, preventing the equipped food from accidentally overwriting the latest roll.

Overall, **FoodRNG** went from a tiny **15-food experiment in V1** into a much larger RNG collection game by V3, while still keeping the original idea simple: **roll, discover, collect, upgrade, and chase the rarest food squishies.**

