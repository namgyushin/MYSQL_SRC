## 💗 MYSQL 수업 내용 정리 💗

### 🌼git_linux<br/><br/>


▶ 터미널에 폴더를 만들어줄 경로로 들어간다<br/>
ex) cd /home/test/Desktop/MYSQL_SRC/

▶ nano로 파일 만들기 <br/>
ex) nano README.md

▶ .git 폴더만들기 로컬저장소라 부름 <br/>
(혹여나 잘못생성했을시 rm -rf .git 으로 지울수있다)<br/>
: git init (git 초기화과정)<br/>
: ls -al 입력으로 잘 생성되었는지 확인

▶ 정보등록하기 : 한번 등록시 안해도된다<br/>
: git config --global user.email "mignon5612@naver.com"<br/>
: git config --global user.name "mignon5612"<br/>
✔️ 잘 등록됐는지 확인할때는 : git config --list 로 확인할수있다

▶ 내용변경하고 변경된 새로운 버전으로 저장할때<br/>
: git add README.md<br/>
✔️ 특정한 파일이 아닌 폴더 전체를 올릴때는 : git add .(현재폴더)<br/>

▶ 변경된 자료단위로 올릴때<br/>
: git commit -m "설명 업데이트" (큰 따옴표에 부가적인 설명을 써주면됨)<br/>

▶ 지금까지 만든 커밋 확인<br/>
: git log<br/>
✔️ git log는 최신 커밋부터 보여줌

▶ 원하는 커밋으로 되돌리기<br/>
: git checkout ex) a0e7f76<br/>
✔️ git log 확인시 commit 뒤에 쭉 나오는 숫자, 알파벳 조합이 커밋 아이디<br/>
여기서 앞 7자리까지 넣으면 가능 전체를 넣어도 가능하다<br/>
✔️ git checkout - :커밋아이디를 안넣어도 최신 커밋으로 이동 가능<br/>

▶ 로컬저장소(.git)에 만들었던 커밋들을 원격저장소(git)로 올리기<br/>
: git remote add origin https://github.com/mignon5612/MYSQL_SRC.git (원격저장소 git주소넣기)<br/>

▶ 지금까지 만든 커밋을 둘 장소 이름 짓고 만들기<br/>
: git branch -M main<br/>

▶ 원격저장소의(origin) main이라는 방에 내 커밋올리기<br/>
: git push origin main<br/>
✔️ 리눅스에서는 이 작업시 토큰방식 사용<br/>
비밀번호 넣는 칸에 전에 미리 저장해둔 토큰을 넣고 엔터<br/>
└ 비밀번호 입력시 안보이는게 정상<br/>

▶ 원격저장소 주소를 입력하여 내 컴퓨터 로컬저장소로 내려받기<br/>
: git clone https://github.com/mignon5612/MYSQL_SRC.git . (원격저장소 git주소넣기)<br/>
✔️ 맨 끝에 꼭 한 칸 띄고 .을 넣어준다 (.은 현재폴더)<br/>

▶ 수정시 수정 후 올리기<br/>
: git add README.md<br/>
: git commit -m "설명 업데이트"<br/>
: git push origin main<br/>

▶ 원격저장소에 새로운 커밋이 있다면 그 커밋을 내 로컬저장소로 받아오기<br/> 
(폴더에서 확인시 아직 반영이안되었을때)   
: git pull origin main<br/>

# 😻
