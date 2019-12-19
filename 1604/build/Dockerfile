from ct:16.04

RUN git clone http://github.com/dtmoodie/ct
RUN cd ct && git submodule update --init
RUN cd ct && mkdir build && cd build && cmake .. && make
