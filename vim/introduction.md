# Vim

vi에서부터 시작된, 오늘날에도 여전히 사랑받고 있는 CLI 텍스트 편집기.   
윈도우에 메모장이 있다면, 유닉스에는 Vim이 있다.

## Vim의 장점

### Vim의 단축키가 제공하는 기능이 강력합니다.

마우스에 손을 쓰지 않고도 에디터의 모든 기능을 활용할 수 있습니다.   
특히 매크로와 정규표현식 기능이 강력하게 작동합니다.

### 마우스를 덜 써도 됩니다.

마우스로 손을 옮기는 횟수가 크게 줄어듭니다. 편집 과정의 자잘한 번거로움이 줄어들고, 생산성이 오릅니다. 오늘날 IDE에서 여러 단축키를 제공하는 이유이기도 합니다.

## 단점은 없나요?

### 높은 진입장벽

Vim을 제대로 활용하기 위해 알아야 하는 선행지식이 많습니다. 이동 모드, 명령 모드에서 사용할 수 있는 단축키와 명령어를 어느 정도 꿰고 있어야 Vim을 잘 활용할 수 있습니다.

### 비직관적인 단축키의 존재

]] 단축키의 경우, 다음 중괄호의 **첫** 위치로 이동합니다. ][ 단축키는 다음 중괄호의 **끝** 위치로 이동합니다. 두 기능이 반대로 되어야 이해하기 쉽지 않을까요?

### 편집기 바깥 기능과의 충돌

클립보드가 좋은 예가 될 것 같습니다. 시스템 클립보드에 있는 내용을 Vim에 붙여넣기하거나, Vim 내의 클립보드의 내용을 시스템 클립보드로 옮기는 과정이 굉장히 뻣뻣합니다.   
근래에는 [해당 부분을 해결할 수 있는 옵션](https://blog.naver.com/nfwscho/220390257384)이 생겼지만, 여러 줄 복사 붙여넣기는 마우스를 쓰는 편이 훨 빠르죠. 

### Vim 편집기 자체로는 한없이 모자란 생산성

Vim이 강력하다고 불리는 이유는 단축키와 매크로, 정규표현식 등의 기능들 때문이었지, Vim 자체의 생산성이 뛰어나서는 결코 아닙니다.   
인텔리제이나 비주얼 스튜디오와 같은 IDE를 쓰는 것이 백번 낫습니다.

## 그럼에도 Vim을 쓰는 이유

### 편집기로써 강력한 성능

그럼에도 Vim이 오늘날까지 살아남고 있는 이유는, 편집기로의 성능이 뛰어나기 때문입니다.   
인텔리제이, 비주얼 스튜디오와 같은 IDE에서도 플러그인을 통해 Vim의 기능들이 제공되고 있고, 오늘날에도 Vim 키배열을 사용하는 도구나 Vim-like editor가 생산되고 있을 정도입니다.

## 그래서 어떻게 시작하죠?

- [vimtutor](https://github.com/vim/vim/blob/master/runtime/tutor/tutor.ko.utf-8)
  - [vimtutor 오버뷰](https://wormwlrm.github.io/2023/04/16/Learn-Vim-with-Vimtutor.html)
- [vim cheatsheet](https://vim.rtorr.com/lang/ko)
- [vimhelp](https://vimhelp.org/)
- [important vim options](https://linuxhint.com/important_vim_settings/)
- [vim.html](https://www.phys.hawaii.edu/~mza/PC/vim.html)

## 관련 링크

- [Vim 도대체 왜 쓰는가](https://bengi.kr/1349)
- [neovim documentation](https://neovim.io/doc/user/)
  - 개인적으로 이쪽을 추천합니다.   
  Vim을 리팩터링하는 프로젝트이고, 가장 많이 쓰이고 있습니다.   
  [Vim 리포지토리](https://github.com/vim/vim)보다 [큰 인기를 끌고 있습니다.](https://github.com/neovim/neovim)