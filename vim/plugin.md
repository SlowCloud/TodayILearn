
# 플러그인

VSCode에서도 플러그인 쓰고 있잖아요? Vim에서도 깔아보자구요!

### 작동방식

vim script로 플러그인을 작성할 수 있으며, Vim의 runtimepath 내부에 넣어두면 플러그인을 사용할 수 있다.  

플러그인 관리자는 이 runtimepath를 조작하여 플러그인의 활용 여부를 관리할 수 있게 해준다.

### 플러그인 관리자

[Vim 버전 8부터 빌트인 패키지 관리자가 생겼다.]((https://dgkim5360.tistory.com/entry/vim-8-native-package-support))

깃허브 Star는 Vundle이 가장 많습니다.  
Vundle 또는 Vim 네이티브를 추천드립니다.

#### [Native Package Management](https://vimhelp.org/repeat.txt.html#packages)
~/.vim/pack/{grp}/start/ 디렉터리에 패키지를 설치(git clone)하시면 됩니다.  
grp 구간에는 아무 이름이나 적으셔도 됩니다.   
[더 자세한 설명](https://learnvim.irian.to/customize/vim_packages)

#### [Pathogen](https://github.com/tpope/vim-pathogen)
README에서 빌트인 패키지 매니지를 사용하는 것을 추천하고 있다.  
기능이 빌트인 패키지와 동일하다.

#### [Vundle](https://github.com/VundleVim/Vundle.vim)
플러그인 관리 기능과 더불어 플러그인 설치 및 업데이트까지 해준다.  
여기에서도 빌트인 패키지의 존재를 알리고 있다.

#### [Vim-Plug](https://github.com/junegunn/vim-plug)
Vundle과 비슷하다. 커맨드도 비슷하다.

## 플러그인

### [NERDTree](https://github.com/preservim/nerdtree)
파일 익스플로러. VSCode를 포함한 웬만한 편집기에는 기본적으로 달려있는 필수적인 기능.

### [vim-startify](https://github.com/mhinz/vim-startify)
Vim Start Screen을 추가해주는 플러그인

### [vim-easymotion](https://github.com/easymotion/vim-easymotion)
커서 이동에 편의성을 추가해주는 플러그인

### [vim-surround](https://github.com/tpope/vim-surround)
중괄호, 따옴표, html 태그 등등 단어/문장을 감싸는 내용 작성을 도와주는 플러그인.

### [fzf.vim](https://github.com/junegunn/fzf.vim)
빠른 파일 검색. 윈도우즈의 Everything을 생각하시면 좋습니다.  
Vim 버전 말고 그냥 [fzf](https://github.com/junegunn/fzf)도 추천드립니다.  
[더 자세한 설명](https://github.com/occidere/TIL/issues/140)  

### [lightline](https://github.com/itchyny/lightline.vim)
Vim의 statusline/tabline을 이쁘게 꾸며주는 플러그인.

### [emmet-vim](https://github.com/mattn/emmet-vim)
html 작성에 크게 도움을 주는 플러그인

### [vimwiki](https://github.com/vimwiki/vimwiki)
Vim으로 빠르고 간편하게 로컬 위키를 만들 수 있게 해주는 플러그인  
[해당 링크](https://johngrib.github.io/wiki/my-wiki/)를 참고하시면 정적 웹 위키를 만들 수도 있어요!