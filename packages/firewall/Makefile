all:
	iptables-restore < /etc/iptables

	# HTTP
	iptables -I INPUT  6 -p tcp --dport 8088 -j ACCEPT

	# HTTPS
	iptables -I INPUT  7 -p tcp --dport 8089 -j ACCEPT

	# Skinny
	iptables -I INPUT  8 -p tcp --dport 2000 -j ACCEPT

	# AMI connections should be accepted only from private IPs
	iptables -I INPUT  9 -p tcp -s 10.0.0.0/8 --dport 5038 -j ACCEPT
	iptables -I INPUT 10 -p tcp -s 172.16.0.0/12 --dport 5038 -j ACCEPT
	iptables -I INPUT 11 -p tcp -s 192.168.0.0/16 --dport 5038 -j ACCEPT

	# AMIS connections should be accepted only from private IPs
	iptables -I INPUT 12 -p tcp -s 10.0.0.0/8 --dport 5039 -j ACCEPT
	iptables -I INPUT 13 -p tcp -s 172.16.0.0/12 --dport 5039 -j ACCEPT
	iptables -I INPUT 14 -p tcp -s 192.168.0.0/16 --dport 5039 -j ACCEPT

	# chan_sip TCP
	iptables -I INPUT 15 -p tcp --dport 5060 -j ACCEPT

	# chan_sip TLS
	iptables -I INPUT 16 -p tcp --dport 5061 -j ACCEPT

	# RTP/RTCP multimedia streaming
	iptables -I INPUT 17 -m multiport -p udp --dports 5000:31000 -j ACCEPT

	iptables-save -f /etc/iptables
