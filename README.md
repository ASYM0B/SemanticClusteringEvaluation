# Evaluation of Semantic-base Clustering using Asym0b
## Introduction
ASYM0B (A framework for SYsteMatically assessment Of chatBots) is a framework to analyse and assess conversational agents or chatbots built in different tools. To support chatbots from different platforms, ASYM0B relies on a neutral chatbot definition called [CONGA](https://saraperezsoler.github.io/CONGA/).
In this [link](https://github.com/ASYM0B/tool) there are ASYM0B environments, which can be used with these chatbots files. 

This repository contains the data of a experiment to evaluate a Semantic-base Clustering of chatbots using Asym0b. To perfome the experiment we use 259 chatbots created
by third parties, from two differents tecnologies (Dialogflow and Rasa) and three sources code repositories like Github, predefined chatbots from the Dialogflow and Rasa platforms, and predefined chatbots from other platforms like [Kommunicate](https://www.kommunicate.io/). The complete dataset of the experiment is available in this [link](https://github.com/ASYM0B/Dataset). 

## Manual Labeling

In a first step, we manually labelled each of the chatbots. At the end of this process we obtained 43 groups, including 6 with only one element (singletons). Each label
represented a semantic field such as “hotels”, “basic conversations” or “food”. A chatbot can be classified using more than one label. For example a chatbot that offers services for searching restaurants is labelled both with “search” and “restaurant”. 
The following table shows the result of the labeling:

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-rsz4{background-color:#DDEBF7;text-align:left;vertical-align:bottom}
.tg .tg-m0vc{background-color:#DDEBF7;text-align:center;vertical-align:middle}
.tg .tg-bobw{font-weight:bold;text-align:center;vertical-align:bottom}
.tg .tg-wa1i{font-weight:bold;text-align:center;vertical-align:middle}
.tg .tg-7dy1{background-color:#DDEBF7;font-weight:bold;text-align:center;vertical-align:middle}
.tg .tg-nrix{text-align:center;vertical-align:middle}
.tg .tg-7zrl{text-align:left;vertical-align:bottom}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-wa1i">#</th>
    <th class="tg-wa1i">Label</th>
    <th class="tg-bobw">Chabots</th>
    <th class="tg-wa1i">#</th>
    <th class="tg-wa1i">Label</th>
    <th class="tg-bobw">Chabots</th>
    <th class="tg-wa1i">#</th>
    <th class="tg-wa1i">Label</th>
    <th class="tg-bobw">Chabots</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-7dy1" rowspan="4">1</td>
    <td class="tg-m0vc" rowspan="4">AIRPORTS</td>
    <td class="tg-rsz4">airportagent</td>
    <td class="tg-wa1i" rowspan="11">14</td>
    <td class="tg-nrix" rowspan="11">GAME</td>
    <td class="tg-7zrl">broken-sequence-jovo</td>
    <td class="tg-7dy1" rowspan="12">26</td>
    <td class="tg-m0vc" rowspan="12">SCHEDULING</td>
    <td class="tg-rsz4">AppointmentScheduler</td>
  </tr>
  <tr>
    <td class="tg-rsz4">airportagent_savelee</td>
    <td class="tg-7zrl">ChronoGG</td>
    <td class="tg-rsz4">enoreese</td>
  </tr>
  <tr>
    <td class="tg-rsz4">flight-booking</td>
    <td class="tg-7zrl">dialogflow-name-psychic</td>
    <td class="tg-rsz4">fulfillment-telephony</td>
  </tr>
  <tr>
    <td class="tg-rsz4">NLP_ChatBot</td>
    <td class="tg-7zrl">escaperoom</td>
    <td class="tg-rsz4">HR-Bot</td>
  </tr>
  <tr>
    <td class="tg-wa1i" rowspan="4">2</td>
    <td class="tg-nrix" rowspan="4">BANKS</td>
    <td class="tg-7zrl">BankPortal</td>
    <td class="tg-7zrl">first-project-test</td>
    <td class="tg-rsz4">keijiban</td>
  </tr>
  <tr>
    <td class="tg-7zrl">dialogflow-transaction</td>
    <td class="tg-7zrl">game-clock</td>
    <td class="tg-rsz4">TPCarBot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">kube-django-ng</td>
    <td class="tg-7zrl">name-that-tune</td>
    <td class="tg-rsz4">Meeting-Booking-Bot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">financial-demo</td>
    <td class="tg-7zrl">videogame-language-model</td>
    <td class="tg-rsz4">Ali</td>
  </tr>
  <tr>
    <td class="tg-7dy1" rowspan="32">3</td>
    <td class="tg-m0vc" rowspan="32">BASIC</td>
    <td class="tg-rsz4">anthrofy</td>
    <td class="tg-7zrl">VoiceClues</td>
    <td class="tg-rsz4">formoriginal</td>
  </tr>
  <tr>
    <td class="tg-rsz4">basic-slotfilling</td>
    <td class="tg-7zrl">QuizWithRasa</td>
    <td class="tg-rsz4">NLP_ChatBot</td>
  </tr>
  <tr>
    <td class="tg-rsz4">ConversAI</td>
    <td class="tg-7zrl">TheWitchat</td>
    <td class="tg-rsz4">rasa-hotel-chatbot</td>
  </tr>
  <tr>
    <td class="tg-rsz4">defaults-chatfuel</td>
    <td class="tg-7dy1" rowspan="10">15</td>
    <td class="tg-m0vc" rowspan="10">HEALTH CARE</td>
    <td class="tg-rsz4">AlexaSkill-PAB</td>
    <td class="tg-rsz4">BikeShop</td>
  </tr>
  <tr>
    <td class="tg-rsz4">defaults-manychat</td>
    <td class="tg-rsz4">enoreese</td>
    <td class="tg-wa1i" rowspan="27">27</td>
    <td class="tg-nrix" rowspan="27">SEARCH</td>
    <td class="tg-7zrl">foodfinder</td>
  </tr>
  <tr>
    <td class="tg-rsz4">dialogflow-quotes</td>
    <td class="tg-rsz4">elekdra01</td>
    <td class="tg-7zrl">mattermost-chatops</td>
  </tr>
  <tr>
    <td class="tg-rsz4">dialogflow-webhook-boilerplate</td>
    <td class="tg-rsz4">episode8</td>
    <td class="tg-7zrl">ai_ml_repo</td>
  </tr>
  <tr>
    <td class="tg-rsz4">fulfillment-multi-locale</td>
    <td class="tg-rsz4">GM-training</td>
    <td class="tg-7zrl">AI-NLP</td>
  </tr>
  <tr>
    <td class="tg-rsz4">hackathon-group-3</td>
    <td class="tg-rsz4">HealthCare_Bot</td>
    <td class="tg-7zrl">aniketbangar</td>
  </tr>
  <tr>
    <td class="tg-rsz4">hackathon-group-10</td>
    <td class="tg-rsz4">HospitalLocator</td>
    <td class="tg-7zrl">Building-Chatbot</td>
  </tr>
  <tr>
    <td class="tg-rsz4">Baisc_Demo</td>
    <td class="tg-rsz4">rasa-for-beginners</td>
    <td class="tg-7zrl">dong5854</td>
  </tr>
  <tr>
    <td class="tg-rsz4">diagrams2ai</td>
    <td class="tg-rsz4">rasaopen</td>
    <td class="tg-7zrl">echo2rasa</td>
  </tr>
  <tr>
    <td class="tg-rsz4">Email-WhatsApp-Integration-Chatbot</td>
    <td class="tg-rsz4">tradunion</td>
    <td class="tg-7zrl">elekdra01</td>
  </tr>
  <tr>
    <td class="tg-rsz4">heroku_demo</td>
    <td class="tg-wa1i" rowspan="8">16</td>
    <td class="tg-nrix" rowspan="8">HOTEL</td>
    <td class="tg-7zrl">06_hotel_bot</td>
    <td class="tg-7zrl">episode8</td>
  </tr>
  <tr>
    <td class="tg-rsz4">juwolfrum</td>
    <td class="tg-7zrl">amanjain1397</td>
    <td class="tg-7zrl">Foodie-Rasa-Chatbot</td>
  </tr>
  <tr>
    <td class="tg-rsz4">jwheat</td>
    <td class="tg-7zrl">LimeBot</td>
    <td class="tg-7zrl">FoodOrder_Chatbot</td>
  </tr>
  <tr>
    <td class="tg-rsz4">knock-knock</td>
    <td class="tg-7zrl">project_chatbot</td>
    <td class="tg-7zrl">formbot</td>
  </tr>
  <tr>
    <td class="tg-rsz4">moodbot</td>
    <td class="tg-7zrl">rasa-hotel-chatbot</td>
    <td class="tg-7zrl">gauravsbisht</td>
  </tr>
  <tr>
    <td class="tg-rsz4">MyPython-master</td>
    <td class="tg-7zrl">Hotel-Booking</td>
    <td class="tg-7zrl">GM-training</td>
  </tr>
  <tr>
    <td class="tg-rsz4">pydata18</td>
    <td class="tg-7zrl">hotel-booking-jawwadturabi</td>
    <td class="tg-7zrl">HospitalLocator</td>
  </tr>
  <tr>
    <td class="tg-rsz4">Rasa_Docker_Test</td>
    <td class="tg-7zrl">HOTEL-BOOKING-AGENT2</td>
    <td class="tg-7zrl">kshamajha</td>
  </tr>
  <tr>
    <td class="tg-rsz4">rasa-playground</td>
    <td class="tg-7dy1" rowspan="9">17</td>
    <td class="tg-m0vc" rowspan="9">INFO</td>
    <td class="tg-rsz4">256644</td>
    <td class="tg-7zrl">ManishaGDas</td>
  </tr>
  <tr>
    <td class="tg-rsz4">sathsaraRasantha</td>
    <td class="tg-rsz4">Data-Mining-Chatbot</td>
    <td class="tg-7zrl">NLP-workshop-newsbot</td>
  </tr>
  <tr>
    <td class="tg-rsz4">starter-pack-rasa-stack</td>
    <td class="tg-rsz4">nep-chatbot</td>
    <td class="tg-7zrl">place_finder</td>
  </tr>
  <tr>
    <td class="tg-rsz4">test_bot</td>
    <td class="tg-rsz4">rasa-faq-bot</td>
    <td class="tg-7zrl">rasaChatbot</td>
  </tr>
  <tr>
    <td class="tg-rsz4">TestFirstRasaBot</td>
    <td class="tg-rsz4">rasaopen</td>
    <td class="tg-7zrl">Restaurant_Chatbot</td>
  </tr>
  <tr>
    <td class="tg-rsz4">twb_asessement</td>
    <td class="tg-rsz4">TheWitchat</td>
    <td class="tg-7zrl">restaurantbot</td>
  </tr>
  <tr>
    <td class="tg-rsz4">HHandoffDAgent</td>
    <td class="tg-rsz4">trackncov19</td>
    <td class="tg-7zrl">Resto-bot</td>
  </tr>
  <tr>
    <td class="tg-rsz4">malikasinger1</td>
    <td class="tg-rsz4">vardhaman-freshers</td>
    <td class="tg-7zrl">Restuarant-Chatbot-Using-Rasa</td>
  </tr>
  <tr>
    <td class="tg-rsz4">stock-bot</td>
    <td class="tg-rsz4">FAQ-RASA-NLU</td>
    <td class="tg-7zrl">Upgrad-Assignment</td>
  </tr>
  <tr>
    <td class="tg-rsz4">concertbot</td>
    <td class="tg-wa1i" rowspan="12">18</td>
    <td class="tg-nrix" rowspan="12">INTERFACE AND COMMANDS</td>
    <td class="tg-7zrl">Developer-Buddy</td>
    <td class="tg-7zrl">Dining-Out</td>
  </tr>
  <tr>
    <td class="tg-rsz4">Jovo-sample</td>
    <td class="tg-7zrl">dialogflow-interactive-canvas</td>
    <td class="tg-7dy1" rowspan="9">28</td>
    <td class="tg-m0vc" rowspan="9">SHOPPING</td>
    <td class="tg-rsz4">beta</td>
  </tr>
  <tr>
    <td class="tg-wa1i">4</td>
    <td class="tg-nrix">CALENDAR</td>
    <td class="tg-7zrl">Date</td>
    <td class="tg-7zrl">ekgsBot</td>
    <td class="tg-rsz4">ChronoGG</td>
  </tr>
  <tr>
    <td class="tg-7dy1" rowspan="4">5</td>
    <td class="tg-m0vc" rowspan="4">CONFIGURATION</td>
    <td class="tg-rsz4">drum-tunner</td>
    <td class="tg-7zrl">fullfilment-firestore</td>
    <td class="tg-rsz4">dialogflow-transaction</td>
  </tr>
  <tr>
    <td class="tg-rsz4">Agent-Name</td>
    <td class="tg-7zrl">iotairblower</td>
    <td class="tg-rsz4">mobile-app-shopping-assistant</td>
  </tr>
  <tr>
    <td class="tg-rsz4">App-Management</td>
    <td class="tg-7zrl">iot-medan</td>
    <td class="tg-rsz4">voicecommerce</td>
  </tr>
  <tr>
    <td class="tg-rsz4">Device</td>
    <td class="tg-7zrl">jovo-skillrf</td>
    <td class="tg-rsz4">Ecommerce_Bot</td>
  </tr>
  <tr>
    <td class="tg-wa1i" rowspan="13">6</td>
    <td class="tg-nrix" rowspan="13">CONVERSATIONAL</td>
    <td class="tg-7zrl">Buddy-G7</td>
    <td class="tg-7zrl">voiceapplication-sonnar</td>
    <td class="tg-rsz4">chatbot_rasa_v2</td>
  </tr>
  <tr>
    <td class="tg-7zrl">iLearn</td>
    <td class="tg-7zrl">abishekv7</td>
    <td class="tg-rsz4">cse591chatbot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">knowledge-graph</td>
    <td class="tg-7zrl">MADE-dialog</td>
    <td class="tg-rsz4">Rasa_NLU_ChatBot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">smalltalk-chatfuel</td>
    <td class="tg-7zrl">App-Management</td>
    <td class="tg-wa1i" rowspan="13">29</td>
    <td class="tg-nrix" rowspan="13">TECHNOLOGY</td>
    <td class="tg-7zrl">ekgsBot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">smalltalk-manychat</td>
    <td class="tg-7zrl">Iot_light</td>
    <td class="tg-7zrl">iLearn_Dialogflow2ServiceNow</td>
  </tr>
  <tr>
    <td class="tg-7zrl">01_smalltalk_bot</td>
    <td class="tg-7dy1" rowspan="14">19</td>
    <td class="tg-m0vc" rowspan="14">JOB AND BUSINESS</td>
    <td class="tg-rsz4">fulfillment-multi-locale</td>
    <td class="tg-7zrl">ISU-Jovo-v2</td>
  </tr>
  <tr>
    <td class="tg-7zrl">Baymax</td>
    <td class="tg-rsz4">HR-Bot</td>
    <td class="tg-7zrl">kommunicate-support-bot-sample</td>
  </tr>
  <tr>
    <td class="tg-7zrl">Chatbot_for_Slack</td>
    <td class="tg-rsz4">Lead_Collection_Bot</td>
    <td class="tg-7zrl">Lead_Collection_Bot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">finbot-master</td>
    <td class="tg-rsz4">Camillads</td>
    <td class="tg-7zrl">02_lead_bot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">identity-cloning-toolkit</td>
    <td class="tg-rsz4">chatbot1demo</td>
    <td class="tg-7zrl">chatbot_rasa</td>
  </tr>
  <tr>
    <td class="tg-7zrl">rasa-workshop-pydata-berlin</td>
    <td class="tg-rsz4">chatform</td>
    <td class="tg-7zrl">chatbot_rasa_v2</td>
  </tr>
  <tr>
    <td class="tg-7zrl">santoshkumar30</td>
    <td class="tg-rsz4">FAQ_Bot</td>
    <td class="tg-7zrl">Customer-Service-Bot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">small-talk-rasa-stack</td>
    <td class="tg-rsz4">RasaDocker</td>
    <td class="tg-7zrl">devbot</td>
  </tr>
  <tr>
    <td class="tg-7dy1" rowspan="8">7</td>
    <td class="tg-m0vc" rowspan="8">CONVERTER</td>
    <td class="tg-rsz4">fulfillment-temperature-converter</td>
    <td class="tg-rsz4">RasaProject_Docker</td>
    <td class="tg-7zrl">ibot</td>
  </tr>
  <tr>
    <td class="tg-rsz4">libsample-advanced</td>
    <td class="tg-rsz4">recruitment-bot-rasa</td>
    <td class="tg-7zrl">Rasa_NLU_ChatBot</td>
  </tr>
  <tr>
    <td class="tg-rsz4">timezonebot-1</td>
    <td class="tg-rsz4">Job-Interview</td>
    <td class="tg-7zrl">Device</td>
  </tr>
  <tr>
    <td class="tg-rsz4">timezonebot2</td>
    <td class="tg-rsz4">fulfillment-regex</td>
    <td class="tg-7dy1" rowspan="7">30</td>
    <td class="tg-m0vc" rowspan="7">TRAVEL</td>
    <td class="tg-rsz4">city-to-city</td>
  </tr>
  <tr>
    <td class="tg-rsz4">Time-Zone-Chatbot</td>
    <td class="tg-rsz4">256644</td>
    <td class="tg-rsz4">ha-austin</td>
  </tr>
  <tr>
    <td class="tg-rsz4">Timezone-Rasa</td>
    <td class="tg-rsz4">ldaPub</td>
    <td class="tg-rsz4">sir2019-group-1</td>
  </tr>
  <tr>
    <td class="tg-rsz4">Currency-Converter</td>
    <td class="tg-wa1i" rowspan="7">20</td>
    <td class="tg-nrix" rowspan="7">META CHATBOTS</td>
    <td class="tg-7zrl">dialogflow-updates</td>
    <td class="tg-rsz4">08_travel_agency_bot</td>
  </tr>
  <tr>
    <td class="tg-rsz4">Formats</td>
    <td class="tg-7zrl">HumanHandoffDemonstrationAgent</td>
    <td class="tg-rsz4">Chatbot_Cab</td>
  </tr>
  <tr>
    <td class="tg-wa1i" rowspan="14">8</td>
    <td class="tg-nrix" rowspan="14">CUSTOMER SERVICE</td>
    <td class="tg-7zrl">fulfillment-multi-locale</td>
    <td class="tg-7zrl">kommunicate-support-bot-sample</td>
    <td class="tg-rsz4">flight-booking</td>
  </tr>
  <tr>
    <td class="tg-7zrl">iLearn_Dialogflow2ServiceNow</td>
    <td class="tg-7zrl">Camillads</td>
    <td class="tg-rsz4">insurance-en</td>
  </tr>
  <tr>
    <td class="tg-7zrl">ISU-Jovo-v2</td>
    <td class="tg-7zrl">chatbot1demo</td>
    <td class="tg-wa1i" rowspan="3">31</td>
    <td class="tg-nrix" rowspan="3">VEHICLE</td>
    <td class="tg-7zrl">TPCarBot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">Insurance_Bot</td>
    <td class="tg-7zrl">yassinelamarti</td>
    <td class="tg-7zrl">Car</td>
  </tr>
  <tr>
    <td class="tg-7zrl">03_real_estate_bot</td>
    <td class="tg-7zrl">FAQ</td>
    <td class="tg-7zrl">woman</td>
  </tr>
  <tr>
    <td class="tg-7zrl">04_feedback_bot</td>
    <td class="tg-7dy1" rowspan="4">21</td>
    <td class="tg-m0vc" rowspan="4">MUSIC AND SOUND</td>
    <td class="tg-rsz4">drum-tunner</td>
    <td class="tg-7dy1" rowspan="4">32</td>
    <td class="tg-m0vc" rowspan="4">WEATHER</td>
    <td class="tg-rsz4">rasa_react</td>
  </tr>
  <tr>
    <td class="tg-7zrl">07_survey_bot</td>
    <td class="tg-rsz4">name-that-tune</td>
    <td class="tg-rsz4">Weather_Bot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">10_freshdesk_customer_support_bot</td>
    <td class="tg-rsz4">your_song</td>
    <td class="tg-rsz4">WeatherBot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">Customer-Service-Bot</td>
    <td class="tg-rsz4">rasa-song-chatbot</td>
    <td class="tg-rsz4">Weather-Chatbot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">ibot</td>
    <td class="tg-wa1i" rowspan="5">22</td>
    <td class="tg-nrix" rowspan="5">NEWS</td>
    <td class="tg-7zrl">09_news_api</td>
    <td class="tg-wa1i" rowspan="5">33</td>
    <td class="tg-nrix" rowspan="5">DELIVERY</td>
    <td class="tg-7zrl">SDP-2018-Group-10</td>
  </tr>
  <tr>
    <td class="tg-7zrl">real-estate-rasa</td>
    <td class="tg-7zrl">NLP-workshop-newsbot</td>
    <td class="tg-7zrl">Talk-to-Spam-Robot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">sharadinfo</td>
    <td class="tg-7zrl">robot-rasa-nlp</td>
    <td class="tg-7zrl">nlp_bot_restaurant</td>
  </tr>
  <tr>
    <td class="tg-7zrl">RasaCustomerService</td>
    <td class="tg-7zrl">wall-e</td>
    <td class="tg-7zrl">RasaAPI</td>
  </tr>
  <tr>
    <td class="tg-7zrl">savelee-demo</td>
    <td class="tg-7zrl">News_Agent</td>
    <td class="tg-7zrl">Food-Delivery</td>
  </tr>
  <tr>
    <td class="tg-7dy1" rowspan="4">9</td>
    <td class="tg-m0vc" rowspan="4">DOMOTIC</td>
    <td class="tg-rsz4">Homie</td>
    <td class="tg-7dy1">23</td>
    <td class="tg-m0vc">NO TEXT</td>
    <td class="tg-rsz4">fulfillent-importer</td>
    <td class="tg-7dy1" rowspan="2">34</td>
    <td class="tg-m0vc" rowspan="2">ANIMALS</td>
    <td class="tg-rsz4">sleepy</td>
  </tr>
  <tr>
    <td class="tg-rsz4">iotairblower</td>
    <td class="tg-wa1i" rowspan="26">24</td>
    <td class="tg-nrix" rowspan="26">RESTAURANTS</td>
    <td class="tg-7zrl">foodfinder</td>
    <td class="tg-rsz4">MysteryAnimal</td>
  </tr>
  <tr>
    <td class="tg-rsz4">iot-medan</td>
    <td class="tg-7zrl">Food_Ordering_Chatbot</td>
    <td class="tg-wa1i">35</td>
    <td class="tg-nrix">HISTORY</td>
    <td class="tg-7zrl">Today-In-History</td>
  </tr>
  <tr>
    <td class="tg-rsz4">Iot_light</td>
    <td class="tg-7zrl">ai_ml_repo</td>
    <td class="tg-7dy1" rowspan="3">36</td>
    <td class="tg-m0vc" rowspan="3">EXERCISING</td>
    <td class="tg-rsz4">wellness-tracker-jovo</td>
  </tr>
  <tr>
    <td class="tg-wa1i" rowspan="9">10</td>
    <td class="tg-nrix" rowspan="9">EDUCATION</td>
    <td class="tg-7zrl">Education_Chatbot</td>
    <td class="tg-7zrl">AI-NLP</td>
    <td class="tg-rsz4">MADE-dialog</td>
  </tr>
  <tr>
    <td class="tg-7zrl">256644</td>
    <td class="tg-7zrl">aniketbangar</td>
    <td class="tg-rsz4">rasa-for-beginners</td>
  </tr>
  <tr>
    <td class="tg-7zrl">courses</td>
    <td class="tg-7zrl">Building-Chatbot</td>
    <td class="tg-wa1i" rowspan="2">37</td>
    <td class="tg-nrix" rowspan="2">SPORTS</td>
    <td class="tg-7zrl">Chat_Bot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">mpchatbot</td>
    <td class="tg-7zrl">dong5854</td>
    <td class="tg-7zrl">iplChatbot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">Reasearch-Project-chatbot</td>
    <td class="tg-7zrl">echo2rasa</td>
    <td class="tg-7dy1" rowspan="9">38</td>
    <td class="tg-m0vc" rowspan="9">ILLNESS</td>
    <td class="tg-rsz4">corona-chatbot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">RP</td>
    <td class="tg-7zrl">Foodie-Rasa-Chatbot</td>
    <td class="tg-rsz4">Covid-19_bot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">RP-12978452-kai</td>
    <td class="tg-7zrl">FoodOrder_Chatbot</td>
    <td class="tg-rsz4">covid19chatbot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">vardhaman-freshers</td>
    <td class="tg-7zrl">formbot</td>
    <td class="tg-rsz4">covid-19-chatbot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">googleChallenge</td>
    <td class="tg-7zrl">gauravsbisht</td>
    <td class="tg-rsz4">HealthCare_Bot</td>
  </tr>
  <tr>
    <td class="tg-7dy1" rowspan="5">11</td>
    <td class="tg-m0vc" rowspan="5">EVENTS AND LEISURE</td>
    <td class="tg-rsz4">marysbikeshop</td>
    <td class="tg-7zrl">kshamajha</td>
    <td class="tg-rsz4">rohitkumar5058</td>
  </tr>
  <tr>
    <td class="tg-rsz4">05_event_bot</td>
    <td class="tg-7zrl">ManishaGDas</td>
    <td class="tg-rsz4">Tiara-A-Chatbot</td>
  </tr>
  <tr>
    <td class="tg-rsz4">Mint-Events-Lead-Gen-bot</td>
    <td class="tg-7zrl">nlp_bot_restaurant</td>
    <td class="tg-rsz4">trackncov19</td>
  </tr>
  <tr>
    <td class="tg-rsz4">movie_chatbot</td>
    <td class="tg-7zrl">place_finder</td>
    <td class="tg-rsz4">FAQ-RASA-NLU</td>
  </tr>
  <tr>
    <td class="tg-rsz4">sokkalingam</td>
    <td class="tg-7zrl">rasaChatbot</td>
    <td class="tg-wa1i" rowspan="6">39</td>
    <td class="tg-nrix" rowspan="6">TIME</td>
    <td class="tg-7zrl">Create-Your-First</td>
  </tr>
  <tr>
    <td class="tg-wa1i" rowspan="10">12</td>
    <td class="tg-nrix" rowspan="10">FOOD</td>
    <td class="tg-7zrl">cookie-sales-skill</td>
    <td class="tg-7zrl">Restaurant_Chatbot</td>
    <td class="tg-7zrl">timezonebot-1</td>
  </tr>
  <tr>
    <td class="tg-7zrl">foodfinder</td>
    <td class="tg-7zrl">restaurantbot</td>
    <td class="tg-7zrl">timezonebot2</td>
  </tr>
  <tr>
    <td class="tg-7zrl">gordobbot</td>
    <td class="tg-7zrl">Restaurant-Bot</td>
    <td class="tg-7zrl">Time-Zone-Chatbot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">multimodal-food-apps</td>
    <td class="tg-7zrl">Resto-bot</td>
    <td class="tg-7zrl">Timezone-Rasa</td>
  </tr>
  <tr>
    <td class="tg-7zrl">Food_Ordering_Chatbot</td>
    <td class="tg-7zrl">Restuarant-Chatbot-Using-Rasa</td>
    <td class="tg-7zrl">Date</td>
  </tr>
  <tr>
    <td class="tg-7zrl">dong5854</td>
    <td class="tg-7zrl">starbucks</td>
    <td class="tg-7dy1" rowspan="3">40</td>
    <td class="tg-m0vc" rowspan="3">SCIENCE</td>
    <td class="tg-rsz4">Data-Mining-Chatbot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">echo2rasa</td>
    <td class="tg-7zrl">Upgrad-Assignment</td>
    <td class="tg-rsz4">ml-data-bot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">restaurantbot</td>
    <td class="tg-7zrl">Coffee-Shop</td>
    <td class="tg-rsz4">mpchatbot</td>
  </tr>
  <tr>
    <td class="tg-7zrl">starbucks</td>
    <td class="tg-7zrl">Dining-Out</td>
    <td class="tg-wa1i">41</td>
    <td class="tg-nrix">HOROSCOPE</td>
    <td class="tg-7zrl">Shany2</td>
  </tr>
  <tr>
    <td class="tg-7zrl">Food-Delivery</td>
    <td class="tg-7dy1" rowspan="4">25</td>
    <td class="tg-m0vc" rowspan="4">MONEY</td>
    <td class="tg-rsz4">expense_tracker</td>
    <td class="tg-7dy1">42</td>
    <td class="tg-m0vc">SECURITY</td>
    <td class="tg-rsz4">woman</td>
  </tr>
  <tr>
    <td class="tg-7dy1" rowspan="3">13</td>
    <td class="tg-m0vc" rowspan="3">COURSES</td>
    <td class="tg-rsz4">santoshikalaskar</td>
    <td class="tg-rsz4">Coffee-Shop</td>
    <td class="tg-wa1i">43</td>
    <td class="tg-nrix">LINGUISTIC</td>
    <td class="tg-7zrl">dialogflow-ssml</td>
  </tr>
  <tr>
    <td class="tg-rsz4">googleChallenge</td>
    <td class="tg-rsz4">Currency-Converter</td>
    <td class="tg-wa1i"> </td>
    <td class="tg-7zrl"></td>
    <td class="tg-7zrl"></td>
  </tr>
  <tr>
    <td class="tg-rsz4">malaynayak</td>
    <td class="tg-rsz4">financial-demo</td>
    <td class="tg-wa1i"> </td>
    <td class="tg-7zrl"></td>
    <td class="tg-7zrl"></td>
  </tr>
</tbody>
</table>
