# msg_queue
###Setting up ZeroMQ on Ubuntu16.04 with C++ bindings####

git clone https://github.com/zeromq/libzmq.git

1. download and unzip the lib, cd to directory

2. mkdir build && cd build
3. cmake ..
4. sudo make -j4 install
5. git clone https://github.com/zeromq/cppzmq.git
6. sudo cp ./zmq.hpp /usr/local/include
7. Copy the example files hwclient.cpp and hwserver.cpp to your working directory from https://github.com/booksbyus/zguide/tree/master/examples/C%2B%2B

8. Compile hwserver.cpp g++ -Wall -o server myserver.cpp -lzmq
9. Run the server ./server
10. Compile hwclient.cpp g++ -Wall -o client myclient.cpp -lzmq

11. Run the client ./client


