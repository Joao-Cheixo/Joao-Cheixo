- 👋 Hi, I’m @Joao-Cheixo 
- 👀 I’m interested in alot of things
- 🌱 I’m currently learning python in a Bioinformatics course
- 💞️ I’m looking to collaborate on some big project
- 📫 How to reach me jonas4777@gmail.com

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/Joao-Cheixo)](https://github.com/anuraghazra/github-readme-stats)

(https://github-readme-stats.vercel.app/api/Joao-Cheixo](https://github.com/anuraghazra/github-readme-stats)

name: Waka Readme

on:
  workflow_dispatch:
  schedule:
    - cron: "0 0 * * *"

jobs:
  update-readme:
    name: WakaReadme DevMetrics
    runs-on: ubuntu
    steps:
      - uses: athul/waka-readme@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
          
