# NOTE DEV

版本號碼命名規則, 基於 djy/3.2.2 branch:
``` 
3.2.2 
  => 3.2.2a-SNAPSHOT => 3.2.2a
  => 3.2.2b-SNAPSHOT => 3.2.2b 
依此類推
```

```shell
# 本機進入 docker container(Hadoop Developer build environment)
hadoop$ ./start-build-env.md

# 在 build env 執行 mvn 進行 build
~/hadoop$ /usr/bin/mvn -Dmaven.repo.local=~/.m2/repository install -Pdist,src,yarn-ui -DskipTests -Dtar > ~/hadoop/patchprocess/mvn_install.log 2>&1
```
