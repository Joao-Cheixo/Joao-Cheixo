- 👋 Hi, I’m @Joao-Cheixo 
- 👀 I’m interested in alot of things
- 🌱 I’m currently learning python in a Bioinformatics course
- 💞️ I’m looking to collaborate on some big project
- 📫 How to reach me jonas4777@gmail.com

<!---
Joao-Cheixo/Joao-Cheixo is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->name: Work Stats Readme

on:
  workflow_dispatch:
  schedule:
    # Runs every 2 hours
    - cron: "0 */2 * * *"

jobs:
  update-readme:
    name: Update this repo's README
    runs-on: ubuntu-latest
    steps:
      - uses: athul/waka-readme@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
