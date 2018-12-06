## MNIST Flask
![image](https://github.com/johnli-zr/mnist-flask/blob/master/Screen%20Shot%202018-12-02%20at%2015.59.09.png)
### 运行方式：
#### 一、
 1.本地运行
 
 1⃣️安装必要的环境：
 
 sudo pip install -r requirements.txt
 
 2⃣️运行：
 
 python app.py
 
 2.虚拟环境

1⃣️下载virtualenv，并构建虚拟环境，见：https://www.liaoxuefeng.com/wiki/0014316089557264a6b348958f449949df42a6d3a2e542c000/001432712108300322c61f256c74803b43bfd65c6f8d0d0000

2⃣️进入虚拟环境后按照本地安装的步骤

3.使用docker

1⃣️安装docker，docker入门见：https://docs.docker.com/install/overview/

2⃣️docker build -t IMAGE_NAME .

3⃣️docker run -d -p 4000:5000 IMAGE_NAME

### 二、连接cassandra

docker run --name some-cassandra -p 9042:9042 -d cassandra:latest

docker run -it --link some-cassandra:cassandra --rm cassandra cqlsh cassandra


