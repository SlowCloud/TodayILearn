
# 파일 저장 및 관리

## 저장 후 나가기
- :wq
- ZZ

## 저장하지 않고 나가기
- :q!
- ZQ

ZQ에 잘못 익숙해지면 기껏 열심히 작성한 것들을 저장하지 않고 날려버리는 수가 있으니 유의

# 줄 이동

## 문서의 처음으로
- gg
- H

## 문서의 끝으로
- G
- L

## 특정 줄로 이동하기
- :{숫자}
- {숫자}gg
- {숫자}G

## 특정 횟수만큼 줄 이동하기
- {숫자}j
- {숫자}k
- {숫자}-
- {숫자}+
- -{숫자}
- +{숫자}

## 빈 줄로 이동하기
- {
- }

# 복사 붙여넣기

## 레지스터
- "{레지스터}y

레지스터에 문자열을 저장한다. "ay를 하면 a 레지스터에 문자열을 저장한다. "by를 하면 b 레지스터에 저장한다. "1y라면 1 레지스터에 저장한다.

- "{레지스터}p

레지스터에 저장된 문자열을 붙여넣는다. @{레지스터}를 해도 된다.

- "+

시스템 클립보드와 연결되는 레지스터. 해당 레지스터에 문자열을 저장하면 Vim 외부에서도 복사한 내용을 사용할 수 있다.  
[해당 기능을 사용 가능한지 확인하는 방법](https://hyoje420.tistory.com/49)

# 편의성

## 숫자 조절
- Ctrl + a

커서가 위치한 숫자를 1 늘린다.

- Ctrl + x

커서가 위치한 숫자를 1 줄인다.

## 오타 변경
- z=

해당 단어와 유사한 다른 단어들을 추천해준다. 단어를 선택하면 해당 단어로 변경해준다.


# 옵션

### number | nu
줄 번호 표시

### relativenumber | rnu
상대적 줄 번호 표시

### clipboard=unnamedplus
Vim의 기본 클립보드를 시스템 클립보드로 설정  
[unnamed와 unnamedplus의 차이](https://stackoverflow.com/questions/30691466/what-is-difference-between-vims-clipboard-unnamed-and-unnamedplus-settings)

# 매크로

vim의 꽃.

## 마지막 행동 반복
- .

A;\<Esc> 후 .를 누르면 해당 줄의 마지막에 세미콜론을 작성한다.  
여러 줄에 세미콜론을 붙여야 한다면 j.j.j.을 연타해서 해결할 수도 있다.

## 매크로 @@@
- q{레지스터}

레지스터에 매크로를 녹화한다. q를 누르면 녹화가 끝난다. @{레지스터}로 매크로를 실행할 수 있다. @@로 직전 매크로를 실행할 수 있다.  

qaA;\<Esc>jq9@@  
위 입력을 따라하면 10줄의 끝에 세미콜론을 작성할 수 있다.

a1\<Esc>qayyp<Ctrl+a>q998@a  
위 입력을 따라하면 1부터 오름차순으로 1000줄의 숫자를 입력할 수 있다.

## 매크로 매핑

.vimrc 혹은 init.vim에서 매크로를 미리 작성해둘 수 있다. Vim 매핑/노테이션에 대해 잘 모른다면 미리 읽고 오는 것을 추천한다.

# 플러그인

VSCode에서도 플러그인 쓰고 있잖아요? Vim에서도 깔아보자구요!

## 작동방식

vim script로 플러그인을 작성할 수 있으며, Vim의 runtimepath 내부에 넣어두면 플러그인을 사용할 수 있다.  

플러그인 관리자는 이 runtimepath를 조작하여 플러그인의 활용 여부를 관리할 수 있게 해준다.

## 플러그인 관리자

Vim 버전 8+에서는 빌트인 패키지 관리자가 존재합니다.  
[Vim 8의 native package support](https://dgkim5360.tistory.com/entry/vim-8-native-package-support)

마음에 드시는 걸로 쓰시면 됩니다.  
깃허브 Star는 Vundle이 가장 많습니다.

### [Native Package Management](https://vimhelp.org/repeat.txt.html#packages)
~/.vim/pack/{grp}/start/ 디렉터리에 패키지를 설치(git clone)하시면 됩니다.  
grp 구간에는 아무 이름이나 적으셔도 됩니다.   
[더 자세한 설명](https://learnvim.irian.to/customize/vim_packages)

### [Pathogen](https://github.com/tpope/vim-pathogen)
README에서, 새로운 사용자들은 빌트인 패키지 매니지를 사용하는 것을 추천하고 있다.  
기능이 빌트인 패키지와 동일하다.

### [Vundle](https://github.com/VundleVim/Vundle.vim)
플러그인 관리 기능과 더불어 플러그인 설치 및 업데이트까지 해준다.

### [Vim-Plug](https://github.com/junegunn/vim-plug)
Vundle과 비슷하다. 커맨드도 같다.

## [NERDTree](https://github.com/preservim/nerdtree)
파일 익스플로러. VSCode를 포함한 웬만한 편집기에는 기본적으로 달려있는 필수적인 기능.

## [fzf.vim](https://github.com/junegunn/fzf.vim)
빠른 파일 검색. 윈도우즈의 Everything을 생각하시면 좋습니다.  
Vim 버전 말고 그냥 [fzf](https://github.com/junegunn/fzf)도 추천드립니다.  
[더 자세한 설명](https://github.com/occidere/TIL/issues/140)  

## [lightline](https://github.com/itchyny/lightline.vim)
Vim의 statusline/tabline을 이쁘게 꾸며주는 플러그인.

## [emmet-vim](https://github.com/mattn/emmet-vim)
html 작성에 크게 도움을 주는 플러그인
