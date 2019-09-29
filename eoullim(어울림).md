# eoullim(어울림)
어울림 레포지터리입니다.

## ★1일차★
깃허브에 대해서 모르는 멤버들이 많아서 모르는 19학번 친구들에게 깃허브에 대해 간단하게 설명하고 사용법을 익혀보는 시간을 가졌습니다.

깃허브란 버전 관리와 협업을 위한 코드 호스팅 플랫폼입니다.  repository,branch,commit,pull request와 같은 개념을 통해 깃에 대해서 알아봅시다.

먼저,  깃허브를 사용하려면 회원가입과 git bash를 까는 것이 필수겠죠?

그럼 시작하도록 합시다.

#### git 최초 설정

```git:
$ git config --global user.name "soohyun"
$ git config --global user.email sss4920@naver.com
```

이처럼 최초설정이 맞춰지고 나서 혹시 모르니 마지막 확인 삼아서

`$ git config --list`해주면 맨밑에 자신의 이름과 이메일이 나와있으면 성공!

![캡처2](https://user-images.githubusercontent.com/49307946/65829096-901ccd80-e2dc-11e9-8c1e-f6a8f67a5132.JPG)

#### 레포지터리 생성

![1569659915017](https://user-images.githubusercontent.com/49307946/65829078-6d8ab480-e2dc-11e9-97ef-b95e8d769129.png)

오른쪽에 초록색 new버튼을 누르고 레포지터리를 만들어줍시다. 

![1569660054175](https://user-images.githubusercontent.com/49307946/65829110-b3477d00-e2dc-11e9-98a6-87887589fdc6.png)


readme파일을 얘기하기전에 pull과 push의 개념을 얘기해보도록 하겠습니다.

##### pull과 push

`github는 우리가 협업등을 할 때 편리한 원격저장소라고 할 수 있는데 우리가 협업을 한다고 하면 우리 local에 저장되어있는 정보를 저장소로 업데이트(push)시켜줘야 할 것이고, 반대로 다른 친구들이 업데이트한 내용을 끌어와서(pull) 최신버전의 프로젝트에서 나의 작업을 수행해야 할 것입니다.`

`  즉, 말그대로 pull은 최신 업데이트된 저장소의 내용을 우리의 local로 끌어온다는 뜻이고 push는 원격저장소로 내가 업데이트한 정보를 올리는 것을 의미합니다`

readme파일은 프로젝트의 목적과 협업방식등을 기록하는 문서인데 이를 생성하기 버튼을 누르면 우리 로컬에선 없는 새 파일이 생성됩니다. 한마디로 우리 컴퓨터에는 빈폴더 밖에 없는데 저장소의 폴더에는 파일 하나가 있는 것입니다. 따라서 로컬로 그 파일을 먼저 옮겨와 저장소와 로컬의 상태를 같게 해준다음 작업을 하는게 충돌나지 않게 해주는 좋은 방법이기 때문에 우리는 pull을 프로젝트 시작 전 계속 해주는 버릇을 들여야합니다.

![1569660838955](https://user-images.githubusercontent.com/49307946/65829125-c9edd400-e2dc-11e9-8222-c8ee6a948791.png)


레포지터리를 생성하고 나면 이런것이 보일텐데요. url부분을 복사해서 이따가 써먹도록합시다.

내가 올릴 폴더안에 들어가서 마우스 우클릭을 눌러 git bash here을 눌러주고 여기 안에 다음과 같은 명령어를 적으면 됩니다.

```git
$ git init 		//.git파일 생성 local에서의 임시데이터등을 잠깐 보관하는 파일을 생성합니다.
$ git remote add origin 주소	//주소라고 써져있는 곳에 url을 복붙하면 되는데 ctrl+v
가 안되므로 shift + insert를 눌러주시면 됩니다
$ git pull origin master //최신 업데이트된 내용을 로컬로 끌고옵니다.
$ git add .  //.git파일에 임시로 업데이트 된 내용을 저장합니다.
$ git commit -m"업데이트한 내용"  //내가 업데이트 될 내용에 대한 설명을 작성합니다.
$ git push origin master  //push를 함으로써 로컬의 내용을 github에 올립니다.
```

`pull`은 막상 내가 혼자서 만드는 포트폴리오 같은 느낌이면 딱히 해줄 필요는 없습니다! 

