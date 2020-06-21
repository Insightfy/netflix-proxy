
仅支持树莓派等ARM设备。


    apt-get update\
	  && apt-get -y install vim dnsutils curl sudo\
	  && curl -fsSL https://get.docker.com/ | sh || apt-get -y install docker.io\
	  && mkdir -p ~/netflix-proxy\
	  && cd ~/netflix-proxy\
	  && curl -fsSL https://github.com/insightfy/netflix-proxy/archive/latest.tar.gz | gunzip - | tar x --strip-components=1\
