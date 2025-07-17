# AWS + GIT + GITHUB + GIT ACTION + AWS Developer Q + SageMaker + Bedrock
    - 위의 키워드 기술 반영 목표

# 목표
    - AWS Developer Q 구독(pro)을 통한 `바이브(Vibe) 코딩` 스타일 익힘
        - 인간 + AI 협업하여 프로젝트 수행
        - 코파일럿을 AWS Developer Q를 통해서 IDE에 설치
        - 채팅 스타일을 통해서 대화형으로 프로젝트 수행
    - SageMaker | Bedrock
        - 직접 훈련시킨 모델(SageMaker) 혹은 llm(Bedrock)을 이용하여 ai 서비스 제공
    - CI/CD
        - GIT, GITHUB : 저장소, 형상관리, 협업
        - GIT ACTION  : CI/CD 
            - access key : AWS SDK 사용 (경우에 따라서는 필요 없을수 있음)
                - 로컬(dev 환경) 필요함
                - 서비스 환경시 불필요한
                - .env 관리 (주의, 절대로 공유 금지, git 업로드 금지)
                    - .gitignore 파일 -> 해당 파일 등록되어야 함.
            - *.pem : ec2 접속
    - AWS
        - EC2 : 가상 서버 제공(서비스 제공)
        - VPC
        - s3 : 모델 저장, 서빙


# CI
    - 지속적 개발
    - 도구
        - git, github, git action
    - 구조
        ```
            /
            L .github
                L workflows
                    L deploy.yml
        ```

# CD
    - 지속적 배포