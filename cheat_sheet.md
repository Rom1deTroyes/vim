# vim cheat sheet

inspired by [this](http://npcode.com/blog/archives/665) blog post.

## split control

* `:sp file` : `file`을 새 분할 윈도우(상하)에서 연다.
* `:vsp file` : `file`을 새 분할 윈도우(좌우)에서 연다.
* `^w ^w` : 분할된 윈도우 간 커서 이동
* `^w h,j,k,l` : 분할된 윈도우 간 커서 이동
* `^w H,J,K,L` : 현재 윈도우를 옮긴다.
* `^w _,|` : 현재 커서가 위치한 윈도우를 최대화 (나머지는 최소화)
* `^w -,+` : 현재 커서가 위치한 윈도우의 크기 조절
* `^w <,>` : vsplit 시 윈도우의 크기 조절
* `^w =` : 최소화, 최대화된 윈도우들을 원상복귀 시킨다.
* `^w q` : 현재 윈도우를 닫는다.
* `:qa` : 분할된 모든 윈도우를 닫는다.
* `:cw` : quickfix window 를 연다.

## tab control

* `:Te` : 새로운 탭을 생성하고 파일브라우저를 띄운다.
* `gt`, `gT` : 탭간 이동
* `^w gf` : 커서 위치의 단어와 관련된 파일을 새 탭에 연다.
* `$vim -p a.txt b.txt c.txt` : vim 실행시 a, b, c 파일을 개별 탭으로 연다.

## Visual mode & change

아래의 명령어에 `v` (visual mode) 와 `c` (change)를 조합하면 다양한 응용이 가능하다.

* V : select entire line
* . : repeat last command

### in

* v i w : select in word
* v i ' : select in single quote
* v i " : select in double quote
* v i [ : select in square brackets
* v i { : select in curly braces

> `c`도 동일하게 활용가능

### til

* v t , : select til comma
* v t ' : select til single quote
* v t = : select til equal

## move & edit

* A : move end of line & insert mode
* I : move start of line & insert mode
* `:jumps` : 커서가 이동했던 모든 위치 확인
  * `ctrl + o` : previous position
  * `ctrl + i` : forward position

## fold

* zc : fold
* zo : unfold
* zM : fold all
* zR : unfold all

## move with g

* gd : will take you to the local declaration.
* gD : will take you to the global declaration.
* g\* : search for the word under the cursor (like \*, but g\* on 'rain' will find words like 'rainbow').
* g# : same as g* but in backward direction.

## 버퍼 목록 기호

기호 | 설명
-----|-----
a | 활성화된 버퍼
% | 현재 편집중
# | 이전에 열었던 버퍼
+ | 변경부분이 있는 버퍼

## Vrapper 전용 명령어

[http://vrapper.sourceforge.net/home/](http://vrapper.sourceforge.net/home/)

* gr : eclipse `refact` 메뉴 표출
* gR : elcipse `rename` 모드
* gm : eclipse `source` 메뉴 표출
