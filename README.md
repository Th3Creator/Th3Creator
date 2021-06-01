# Hello! All good?? My name is Christian Louzada

### 🌍"We are all time travelers on a journey into the mold of tomorrow" 👨‍💻

```javascript
let AboutMe = {
    age: 18,
    country: 'Brazil',
    city: 'Vespasiano, MG',
    interest: ['Python', 'SQL', 'Redes', 'Ruby'],
    hobbies: ['Chess', 'Sport', 'Reading', 'Scientific Content', 'Philosophy']
};
```

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=Th3Creator&show_icons=true&theme=tokyonight)

name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: Th3Creator
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Th3Creator&layout=compact)
