FROM abevoelker/ruby
RUN useradd -m echosrv
USER echosrv
WORKDIR /home/echosrv/
RUN git clone https://github.com/dbrady/echoserver.git
WORKDIR /home/echosrv/echoserver
RUN bundle install
ADD supervisor.conf /etc/supervisor/conf.d/echosrv.conf
