# Mac OS X 개발 환경 설정

## 시스템 설정
**Apple 아이콘 > 시스템 환경설정:**
- 트랙패드 > 탭하여 클릭하기
- Dock > 자동으로 Dock 가리기와 보기
- Mission Control > 핫 코너 > (좌측 상단) 화면 보호기 시작
- Mission Control > 핫 코너 > (우측 상단) 디스플레이 잠자기
- 키보드 > 단축키 > 입력 소스 > 이전 입력 소스 선택 (command + space)
- 키보드 > 단축키 > Spotlight > Spotlight 검색 보기 비활성화

**Command Line:**
- 숨김파일 보기
```sh
$ defaults write com.apple.finder AppleShowAllFiles -bool true
```

- .DS_Store 생성 방지
```sh
$ defaults write com.apple.desktopservices DSDontWriteNetworkStores -bool true
```

## Homebrew
```sh
$ /bin/bash -c "$(curl -fsSL https://gist.githubusercontent.com/nrubin29/bea5aa83e8dfa91370fe83b62dad6dfa/raw/48f48f7fef21abb308e129a80b3214c2538fc611/homebrew_m1.sh)"
$ eval $(/opt/homebrew/bin/brew shellenv)
$ brew update
$ brew tap caskroom/cask
$ brew install git
```

## iTerm2
- zsh
```sh
$ chsh -s `which zsh`
```

- oh-my-zsh
```sh
$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

$ vim ~/.zshrc

# 테마 수정
ZSH_THEME="agnoster"
```

- [D2 font](https://github.com/naver/d2codingfont)

- iTerm2 > Preferencs > Profiles > Text > Change font > Roboto Mono Light for Power line

- [iterm2 커스텀 참조](https://ooeunz.tistory.com/21)
