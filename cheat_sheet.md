# vim cheat sheet

inspired by [this](http://npcode.com/blog/archives/665) blog post.

## split control

* `:sp file` : `file`을 새 분할 윈도우(상하)에서 연다.
* `:vsp file` : `file`을 새 분할 윈도우(좌우)에서 연다.
* `^w ^w` : 분할된 윈도우 간 커서 이동
* `^w h,j,k,l` : 분할된 윈도우 간 커서 이동
* `^w H,J,K,L` : 현재 윈도우를 옮긴다.
* `^w _,|` : 현재 커서가 위치한 윈도우를 최대화 (나머지는 최소화)
* `^w -,+` : 현재 커서가 위치한 윈도우의 크기를 줄이거나(-), 키운다(+)
* `^w =` : 최소화, 최대화된 윈도우들을 원상복귀 시킨다.
* `:qa` : 분할된 모든 윈도우를 닫는다.