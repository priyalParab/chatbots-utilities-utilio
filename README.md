# Utilio
Utilio is a digital assistant built on the RASA stack that enhances customer engagement. This project plans on exploiting various popular customer support codes and features across platforms to build a strong text and voice controlled, AI powered, multi-lingual, analytical assistant. 

Use of RASA enables configuration management, instead of code intense applications  for behavioural and operational control
The current version works by integrating Utilio with Oracle Utilities Application Framework (CC&B, C2M, MDM) via real-time web service calls for the utilities sector. The future versions can be extended to integrate with ORMB to enable Utilio to engage with traffic in the Banking sector.

## Project Goal
The goal is to make Utilio:
- **insightful**
- **omni-channel compatible**
- **supportive to purposeful automation**
- **one stop shop**

Training this bot requires a colloquial feed of user-CSR conversations to match the local lingo that personifies the chat experience of the user unique to every implementation. Features of RASA empower this  alongwith easy DEV to PROD deployment and live training of the assistant by use of RASA X.

## Setup and installation
To experience the rich features of RASA without installing, kindly refer
https://rasa.com/docs/rasa/playground/

To continue with installing RASA, please refer 
https://rasa.com/docs/rasa/installation/

### Files for Utilio's Rasa Core model
- **data/nlu.md** file contains intents the assistant is expected to recognize and set context to user's query. 
- **data/stories.md** file contains some training stories which represent the conversations between a user and the assistant. 
- **domain.yml** file describes the domain of the assistant which includes intents, entities, slots, responses and actions the assistant should be aware of.  

**Note**: RASA starter pack should suffice to understand the workings of a basic RASA bot
https://github.com/RasaHQ/rasa-for-beginners
