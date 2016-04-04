# Logstash-Config

https://elijahpaul.co.uk/monitoring-pfsense-2-1-logs-using-elk-logstash-kibana-elasticsearch/

https://elijahpaul.co.uk/updated-monitoring-pfsense-logs-using-elk-elasticsearch-logstash-kibana-part-1/

https://gist.githubusercontent.com/mikedevita/ff927c5a8fdb138bca35/raw/f0f7d41f62016beb4a11d38e381360e05dbf52b1/pfsense-firewall.json

http://www.505forensics.com/who-have-your-logs-been-talking-to/


#SNORT

http://www.fastfire.org/2015/12/18/visualize-pfsense-snort-logs-on-kibana/

https://discuss.elastic.co/t/logstash-snort-implementation/32386

http://www.fastfire.org/2015/12/18/visualize-pfsense-snort-logs-on-kibana/

#SURICATA

https://blog.reboost.net/suricata-on-pfsense-to-elk-stack/

https://www.bilgiguvenligi.gov.tr/saldiri-tespit-sistemleri/saldiri-tespit-sistemleri-snort-suricata-bro.html

# NSM
http://nidofortified.blogspot.com.tr/2014/06/suricata-with-logstash-part-3-setup-and.html
https://github.com/sysforensics/LogstashConfigs

# SELKS
S - Suricata IDPS - http://suricata-ids.org/

E - Elasticsearch - http://www.elasticsearch.org/overview/

L - Logstash - http://www.elasticsearch.org/overview/

K - Kibana - http://www.elasticsearch.org/overview/

S - Scirius - https://github.com/StamusNetworks/scirius

https://github.com/StamusNetworks/SELKS

#Logstash
https://cinhtau.net/wp/tag/logstash/

# Logstash Parse
https://blog.lanyonm.org/articles/2014/01/12/logstash-multiline-tomcat-log-parsing.html

https://www.loggly.com/docs/logstash-custom-parsing-loggly/

https://github.com/elastic/logstash/blob/v1.4.2/patterns/grok-patterns

http://grokdebug.herokuapp.com/

https://home.regit.org/2014/01/a-bit-of-logstash-cooking/

Mcafee Log
==========

%{WORD:hostname} %{WORD:action} %{WORD:attack} %{WORD} %{WORD:service_type}%{SPACE=:} %{GREEDYDATA:attack_type} [%{SPACE=)}]%{WORD} %{SPACE==} %{WORD:severity}%{DATA}%{DATA} %{IPV4:kaynak_ip}%{SPACE=:}%{INT:kaynak_port} %{SPACE=->} %{IPV4:hedef_ip}%{SPACE=:}%{INT:hedef_port} %{DATA} %{SPACE==} %{DATA}%{GREEDYDATA:result}[%{SPACE=)}]

