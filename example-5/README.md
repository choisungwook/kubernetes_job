# 개요
* activeDeadlineSeconds를 설정하여 job실행시간을 제한
* activeDeadlineSeconds로 종료된 job은 실패처리 되고 pod가 삭제됨

# 디버깅
*

```bash
$ kubectl describe job example-5-infinity-daedline
...
Pods Statuses:            0 Active (1 Ready) / 0 Succeeded / 1 Failed
...
Warning  DeadlineExceeded  16s   job-controller  Job was active longer than specified deadline
```
