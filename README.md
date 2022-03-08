# 각종 가이드
ff

## 터미널, gpu usage

kill -9 PID (nvidia-smi 에 PID 나올시)


for i in $(sudo lsof /dev/nvidia* | grep python | awk '{print $2}' | sort -u); do kill -9 $i; done (안나올때 파이썬 사용하는 process 싹다 죽임 *는 gpu #)

## conda

conda create -n 가상환경이름 python=버전


conda remove -n 가상환경이름 --all
