
# 파일 저장 및 관리

## 저장 후 나가기
- :wq
- ZZ

## 저장하지 않고 나가기
- :q!
- ZQ

ZQ에 잘못 익숙해지면 기껏 열심히 작성한 것들을 저장하지 않고 날려버리는 수가 있으니 유의

# 줄 이동

## 특정 줄로 이동하기
- :{숫자}
- {숫자}gg

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

# 편의성

## 숫자 조절
- Ctrl + a

커서가 위치한 숫자를 1 늘린다.

- Ctrl + x

커서가 위치한 숫자를 1 줄인다.

## 오타 변경
- z=

해당 단어와 유사한 다른 단어들을 추천해준다. 단어를 선택하면 해당 단어로 변경해준다.

# 검색
- /

단어 검색

- f{letter}

앞으로 단어 검색. ;를 눌러 다음 단어로 넘어간다. F{letter}는 역방향.

- t{letter}

위와 같으나, 단어의 앞에서 멈춘다.

# 치환


# 옵션

## number - nu
줄 번호 표시

## relativenumber - rnu
상대적 줄 번호 표시

## colorscheme
스키마 변경  
:colorscheme을 작성하고 띄워쓰기 후 Ctrl + d를 누르면 사용 가능한 스키마 목록을 확인할 수 있다.

# 매크로

vim의 꽃.

## 마지막 행동 반복
- .

A;\<Esc> 후 .를 누르면 해당 줄의 마지막에 세미콜론을 작성한다.  
여러 줄에 세미콜론을 붙여야 한다면 j.j.j.을 연타해서 해결할 수도 있다.

## 매크로 @@@
- q{레지스터}

레지스터에 매크로를 녹화한다. q를 누르면 녹화가 끝난다. @{레지스터}로 매크로를 실행할 수 있다. @@로 직전 매크로를 실행할 수 있다.  
qaA;<Esc>jq 입력 후, 10@@를 하면 10줄의 끝에 세미콜론을 작성할 수 있다.