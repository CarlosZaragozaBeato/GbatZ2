- 👋 Hi, I’m @GbatZ2
- 👀 I’m interested in ... learn all about the web
- 🌱 I’m currently learning ... CSS, Java, SQL, JS
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
GbatZ2/GbatZ2 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=Gapur&show_icons=true&hide_border=true&&count_private=true&include_all_commits=true" />
name: Waka Readme

on:
  workflow_dispatch:
  schedule:
    # Runs at 12am UTC
    - cron: "0 0 * * *"

jobs:
  update-readme:
    name: Update this repo's README
    runs-on: ubuntu-latest
    steps:
      - uses: athul/waka-readme@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
