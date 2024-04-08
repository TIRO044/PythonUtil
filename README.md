파이선에 관련된 유틸 코드작업 뭉탱이

# ScriptImporter

- 유틸성 스크립트를 import 해서 사용하고 싶은데, 스크립트 마다 매번 경로 찾아 임포트 해야 함
- 그걸 해결하기 위한 스크립트를 만들자.
- 근데 이것도 결국 ScriptImpoter 라는 스크립트를 임포트를 매번 해줘야 함
  - 이건 어떻게 해결할지 좀 더 생각해보자
       
  ### TODO :
    - 경로를 config.json을 통해서 읽어 올 수 있도록 처리하기
    - 임의로 정의한, 디렉터리 구조안에서 ScriptImporter라는 기능을 전역적으로 사용할 수 있는 방법 구상하기





# LogBox
  - Log를 작업자들 마다 맘대로 찍기 떄문에 가독성이 매우 구리다.
  - 따라서, 이쁜 포멧을 지원하는 Log 유틸 스크립트를 만들자.

    ### TODO:
      - 서브 프로세스 print 후킹하기?

  이런 형태로 작업할 것..
  
  ### input
    name = "j"
    job = "programmer"
    
    LogBox.Input("myName {j}")
    LogBox.Input("job {job}")
    LogBox.Print()
    
  ### output
     ####      test    ###
     # myName : j        #
     # job : programmer  #
     #####################

# 라이브러리로만들기

짜증나니까 라이브러리로 만들어서 배포하든가.. 그런 식으로 해보자
