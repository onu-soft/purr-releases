# Purr — 릴리스

[Purr](https://github.com/onu-soft/purr) 의 설치 파일과 자동 업데이트 매니페스트를 두는 곳입니다.

- **설치**: [Releases](https://github.com/onu-soft/purr-releases/releases) 에서 최신 `Purr.dmg`(맥) 또는 `Purr-setup.exe`(윈도우)
- **자동 업데이트**: 앱이 `latest.json` 을 읽습니다. 🚨 앱이 보는 곳은 **main 브랜치의 이 파일**이지 릴리스 자산이 아닙니다.

`latest.json` 은 `scripts/generate-latest-json.sh` 가 만들고 `pnpm upload:publish` 가 올립니다.
플랫폼마다 따로 빌드해 `platforms` 를 **머지**합니다 — 새로 만들어 덮으면 다른 OS 사용자가 업데이트를 못 받습니다.
