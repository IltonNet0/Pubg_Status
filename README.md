# PUBG Weapon Stats Viewer (Django Project)

This Django-based application is designed to manage and visualize statistics of firearms used in the game **PUBG (PlayerUnknown's Battlegrounds)**.

The main goal of this project is to provide a structured and interactive way to analyze and compare different guns and attachments, and see how each accessory impacts weapon performance.

## 🚀 Features (Phase 1)

- **Weapons database** with detailed attributes such as:
  - Damage per bullet and per second
  - Rate of fire, stability, reload speed, bullet velocity, and more
  - Weapon type and bullet type

- **Attachments models**:
  - **Grips**, **Muzzles**, **Magazines**, and **Stocks**
  - Each attachment has its own effects on weapon stats (e.g., recoil, ADS time, hip fire accuracy, etc.)

- **Relationships**:
  - Guns are connected to attachments via `ManyToMany` relationships
  - Each gun can support multiple compatible accessories

- **Dynamic calculation**:
  - Methods inside the `Guns` model calculate final weapon stats based on selected attachments

## 🧠 Example Usage

With the data structure in place, the application can:
- Allow users to select a weapon and equip different attachments
- Automatically calculate the final stats with the applied effects
- Provide useful insights for players to optimize their weapon loadouts

## 🛠 Tech Stack

- **Python 3.12+**
- **Django 4+**
- **SQLite** (for development)

## 🔄 Upcoming Features

- Interactive frontend to select guns and attachments visually
- Map with hidden spots and vehicle spawns
- User accounts and saved loadouts
- JSON data import/export for gun and attachment information

## 📂 Project Structure (Relevant Part)

```bash
statusArmas/
├── models.py         # Models for Guns, Grips, Muzzles, Mags, and Stocks
├── admin.py          # Django admin registration
├── views.py          # (Coming soon)
├── ...