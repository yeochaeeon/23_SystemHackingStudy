### PIE write-up

- 가장먼저 봐야하는 것 :
    - fgets 랑 buf 의 크기 
    - ret 어드레스를 덮는다 ??

    - ```file ``` 으로 몇비트인지 확인 
    - ```checksec``` 으로 어떤 보호기법이 걸려있는지 확인
    - pie 보호기법이 걸려있으니까 베이스 주소를 구해야 할 것이다 ....
    - buf의 실제 위치를 찾는다 ->  fgets 보고 찾으면 됨 
    - ```ROPgadget```     
