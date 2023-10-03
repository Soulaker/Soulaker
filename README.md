https://img.shields.io/badge/python-3.9-orange?style=for-the-badge&logo=python&logoColor=orange
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
          <!--START_SECTION:waka-->
<!--END_SECTION:waka-->
