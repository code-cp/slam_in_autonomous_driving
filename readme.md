## SLAM in Autonomous Driving book (SAD book)

- use in docker 

```bash
docker build -t sad:v1 .
./docker/docker_run.sh
```
进入docker容器后
```bash
cd ./thirdparty/g2o
mkdir build
cd build
cmake ..
make -j8
cd /sad
mkdir build
cd build
cmake ..
make -j8
```

- solve g2o issues by https://github.com/gaoxiang12/slam_in_autonomous_driving/issues/95
- on host, need to run `xhost +`
- to run the examples, go to `bin` folder, and run `./motion`