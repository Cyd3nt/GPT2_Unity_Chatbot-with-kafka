Chatbots using the KoGPT2 model in a metaverse virtual space (GPT2_Unity_Chatbot-with-kafka)
✔ In the Unitiy virtual space, a chatbot based on the KoGPT2 model was implemented in conjunction with Kafka.
✔ The KoGPT2 model is a learning model that predicts the next word from a given word. It is optimized for sentence generation.

✔ Project Duration: 22/03/14 ~ 22/04/01
✔ Final PPT Link: https://drive.google.com/file/d/1zLnQs3izegjii2x778iMkhbLdDm77Y7-/view?usp=sharing

Implementation features
1️⃣ Unity implemented a metaverse based on various characters in the virtual space. You can move your character around and enjoy the visual effects as if you were playing a game. Han, we also implemented the ability to go to the website through the portal.
2️⃣ In a virtual space, you can have everyday and emotional conversations with chatbots trained by machine learning.
3️⃣ Conversations between clients and chatbots are sent and received through Kafka.
4️⃣ Repeat the cycle to save the conversation to Spark and Hadoop. Retrain the chatbot based on the stored data. 
   
   
Role Sharing
🔹 Sejin Kim: Retraining deep learning code to Spark (sparkML), storing large DBs in Hadoop clusters
🔹 Ye Bin Kim: Artificial Intelligence NLP AI design and learning, implementation of retraining code with chat history, sending and receiving Kafka data, PPT
🔹 Kyuho Jang: Storing large amounts of DB in Hadoop clusters, selecting training datasets, and processing extracts
🔹 Seo Hyun Jang: Developing Unity Environments, Sending and Receiving Kafka Data, Adding Photon Server Client Environments, Visualizing with ELK
   
   
## 역할 분담
🔹 김세진: 딥러닝 코드를 Spark로 재학습 (sparkML), Hadoop 클러스터에 대용량 DB저장   
🔹 김예빈: 인공지능 NLP AI 설계 및 학습, 채팅 내역으로 재학습 코드 구현, Kafka 데이터 송수신, PPT   
🔹 장규호: Hadoop 클러스터에 대용량 DB저장, 학습 데이터셋 선정 및 추출 가공  
🔹 장서현: Unity 환경 개발, Kafka 데이터 송수신, Photon 서버 클라이언트 환경 추가, ELK로 시각화   
   
## 구성도
<img width="65%" src="https://user-images.githubusercontent.com/50973139/160983406-2f64d241-2593-45e1-b540-a86a5a3e6d50.png"/>
   
     
System (Preferences)
system	CPU	memory	HDD	Program Version	Remarks
Kafka broker	1	2.0GB	20GB	2.13	Vmware
Kafka Producer 1	2	16.0GB	100GB	2.13	Vmware
Kafka Consumer 1	1	4.0GB	20GB	2.13	Vmware
Kafka Producer 2	1	1GB	20GB	2.13	Vmware
Kafka Consumer 2	1	1.0GB	20GB	2.13	Vmware
Spark master	4	16.0GB	422GB	3.1.3	computer
Spark worker1	2	8.0GB	50GB	3.1.3	Vmware
Spark worker2	2	8.0GB	50GB	3.1.3	Vmware
Hadoop master	4	16.0GB	421.0GB	3.2.2	computer
Hadoop worker1	2	8.0GB	50.0GB	3.2.2	Vmware
Hadoop worker2	2	8.0GB	50.0GB	3.2.2	Vmware
Unity	2	16.0GB	100GB	2020.3.30f1	notebook
Photon	2	16.0GB	100GB	photon unity networking2	notebook
Logstash	4	8.0GB	100GB	7.17.1	notebook
Elasticsearch	2	4.0GB	20GB	7.17.1	Vmware
Kibana	2	4.0GB	20GB	7.17.1	Vmware

Producer 1 and Consumer 1 are used when asked a question, and Producer 2 and Consumer 2 are used to send an answer
   

## Unity & Photon
* 
* 
*  
   
Apache Kafka
Topic	Producer	Consumer	Context	Remarks
bot_question	Unity Server	Machine learning test	Client Questions	Question
ChatbotA	Machine learning test	Unity Server	Chatbot Answers	Answer
ChatbotB	Machine learning test	Unity Server	Chatbot Answers	Answer
ChatbotC	Machine learning test	Unity Server	Chatbot Answers	Answer
Python (Machine Learning)
   
