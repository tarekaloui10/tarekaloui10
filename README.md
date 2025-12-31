<h1 align ="center "> welcome to tarekaloui's profile</h1>
<p>
  <img src="https://skillicons.dev/icons?i=react,html,css,js,tailwind,bootstrap,vite,java,mysql,git,github,python,c,c#,linkedin,discord,vscode,eclipse,sqloracle,php"
</p>
![snake animation](https://github.com/tarekaloui10/tarekaloui10/blob/output/github-contribution-grid-snake.svg)
.github/workflows/snake.yml
name: Generate Snake

on:
  schedule: 
    - cron: "0 0 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@master
        with:
          github_user_name: YOUR_USERNAME
          outputs: dist/snake.svg

      - name: Push
        uses: actions/upload-artifact@v2
        with:
          name: snake
          path: dist




