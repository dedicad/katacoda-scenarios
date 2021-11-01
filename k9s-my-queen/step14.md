Let's test our new skills on gojob Clusters !

**Plizz on gojob cluster, use safe readonly mode !** (add alias, or whatever, but only use other for precise actions !)

This step is designed to be performed on **review** cluster, so quit this UI and just write down the answer here progressively !!

>>How many nodes do we have on cluster ?<<
=== 16

>>What is the oldest node of our cluster ? (last 4 characters is enough)<<
=~= ob21

>>What is the newest namespace created ?<<
( ) kirigami
( ) monitoring
(x) gateway


>>How many namespaces contains "ad" in their names ?<<
( ) 5
(x) 3
( ) 1

>>How many namespaces does not contain the letter "o" in their names ?<<
(x) 14
( ) 12
( ) 18

>>Look at the pod kirigami-staging, what is the last event on this pod ?<<
=~= none

>>What value of env variable API_V2_URL does hris staging uses ?<<
=== https://ipa.gojob.com

>>How many cronjobs do we have running on our cluster ?<<
[ ] 50-60
[x] 60-70
[ ] 70-80

>>What service account is used by kirigami-staging ?<<
=== kirigami-project

>>Do you see a weird container in gateway namespace ? What is its first log line ?<<
=== Hello from Docker !

