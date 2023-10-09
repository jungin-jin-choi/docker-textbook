docker image build --tag {이미지-이름} .

// docker-credential-desktop not installed or not available in PATH 에러가 뜬다면 ~/.docker/config.json 을 점검해보자
https://stackoverflow.com/a/72888813 참고!

```
brew install docker-credential-helper
docker-credential-osxkeychain version

Set credsStore to osxkeychain in ~/.docker/config.json

{
  "auths": {
    "https://index.docker.io/v1/": {}
  },
  "credsStore": "osxkeychain",
  "experimental": "enabled",
  "stackOrchestrator": "swarm"
}
