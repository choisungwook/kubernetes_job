# 개요
* RestartPolicy Never vs Onfailure 비교

# 내용
* Never는 pod가 실패하면 새로운 pod가 생성되어 다시 작업 실행
* 반면, Onfailure는 기존 pod가 Restart되어서 작업 실행

# 어느 것을 사용하는게 좋을까?
* 실패로그를 남기려면 Never을 사용한다.
* job이 실행한 pod를 목록에서 표시하고 싶지 않으면 Onfailure를 사용한다.
