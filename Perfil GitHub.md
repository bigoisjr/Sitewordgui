
### Olá Mundo, eu sou o Juan Bigois!✌

[![Istagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/bigois.jr/)
[![facebook](https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/jcrbigois)
[![linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/juan-bigois/)
[![Whatsapp](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://api.whatsapp.com/send?phone=5511951174665&text=Ol%C3%A1%20Dev%2C%20vim%20pelo%20GitHub%20e%20gostaria%20de%20falar%20com%20voc%C3%AA.)


![Bigois GitHub stats](https://github-readme-stats.vercel.app/api?username=Bigois&show_icons=true&theme=onedark)



✔ cobrinha

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
          github_user_name: Bigois
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

© 2022 GitHub, Inc.
Terms
Privacy
Security
Status