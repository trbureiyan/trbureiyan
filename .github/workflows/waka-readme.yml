name: Waka Readme

on:
  # manual workflow trigger
  workflow_dispatch:
  schedule:
    # runs at 12 AM UTC (5:30 AM IST)
    - cron: "0 0 * * *"

jobs:
  update-readme:
    name: WakaReadme DevMetrics
    runs-on: ubuntu-latest
    steps:
        # this action name
      - uses: athul/waka-readme@master # do NOT replace with anything else
        with:
          GH_TOKEN: ${{ secrets.GH_TOKEN }}
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
          
          ### meta
          # API_BASE_URL: https://wakatime.com/api # optional
          REPOSITORY: trbureiyan/trbureiyan
          
          ### content
          SHOW_TITLE: true
          SECTION_NAME: waka
          BLOCKS: ░▒▓█
          # CODE_LANG: rust
          TIME_RANGE: all_time
          # LANG_COUNT: 10
          SHOW_TIME: true
          SHOW_TOTAL: true
          SHOW_MASKED_TIME: false # optional
          STOP_AT_OTHER: true # optional
          IGNORED_LANGUAGES: JSON YAML TXT TOML
          SHOW_SHORT_INFO: true
          
          ### commit
          COMMIT_MESSAGE: Updated waka-readme graph with new metrics # optional
          # TARGET_BRANCH: master # optional
          # TARGET_PATH: README.md # optional
          COMMITTER_NAME: GitHubActionBot # optional
          COMMITTER_EMAIL: action-bot@github.com # optional
          AUTHOR_NAME: trbureiyan
          AUTHOR_EMAIL: trbureiyan@duck.com
