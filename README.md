# Utisto
Utisto is a digital assistant built on the RASA stack that enhances customer engagement for utilities. This project plans on exploiting various popular customer-support models and features across platforms to build a strong text and voice controlled, AI powered, multi-lingual, analytical assistant. 

Use of RASA enables configuration management, instead of code-intense applications  for behavioural and operational control.
The current version works by integrating Utisto with Oracle Utilities Application Framework (CC&B, C2M, MDM) via real-time web service calls for the utilities sector. The future versions can be extended to integrate with ORMB to enable Utisto to engage with traffic in the Banking sector.

## Project Goal
The goal is to make Utisto:
- **insightful**
- **omni-channel compatible**
- **supportive to purposeful automation**
- **one stop shop**

Training this bot requires a colloquial feed of user-CSR conversations to match the local lingo that personifies the chat experience of the user, unique to every implementation. Features of RASA empower this  alongwith easy DEV to PROD deployment and live training of the assistant by use of RASA X.

## Setup and installation
To experience the rich features of RASA without installing, kindly refer:

https://rasa.com/docs/rasa/playground/

To continue with installing RASA, please refer:

https://rasa.com/docs/rasa/installation/

### Files for Utisto's Rasa Core model
- **data/nlu.md** file contains intents the assistant is expected to recognize and set context to user's query. 
- **data/stories.md** file contains some training stories which represent the conversations between a user and the assistant. 
- **domain.yml** file describes the domain of the assistant which includes intents, entities, slots, responses and actions the assistant should be aware of.  

**Note**: RASA starter pack should suffice to understand the workings of a basic RASA bot, refer:

https://github.com/RasaHQ/rasa-for-beginners

## Utisto in action
Utisto responds to a user's ping in multiple lingos. The AI understands the user's **Intent** and responds with easy-to-use buttons and a textual **Response**.
At this point, the user may choose to click on the on-screen buttons or enter a query without necessarily following a uni-directional flow.
Utisto responds with the best possible reponse. 

For a generic flow demo, consider the below snap of Utisto enabling a Utility's Customer to know his current balance. (More test results can be found in **utisto/tests/**)

![image](https://user-images.githubusercontent.com/71168871/96767916-cf8fed80-13fa-11eb-974f-000602b89c47.png)

**Note**: Unlike most NLU/P solutions that require "handing-over" of transactional data, RASA eliminates this transfer and can facilitate a ready-to-use solution with minimalistic resources. To further maximize security, Utisto relies on real-time SOAP requests to a web service of the OUAF edge app in the network, instead of database calls. Utisto loads the contextual **operation** of the web service to reduce time lags when in a given flow.

The current project covers the development of the IWS in CC&B/C2M. The IWS and hence Utisto are customizable components to adhere to a Utility's data mapping.
