## payments and billings path
* greet
    - utter_greet
* payments_and_billings
    - utter_PnB_menu_options
* account_balance
    - utter_collect_acctId
    - slot{"acctId":"4195007555"}
* acctId_collector{"acctId":"4195007555"}
    - slot{"acctId":"4195007555"}
    - action_acct_info
* bot_challenge
    - utter_goodbye

## account balance path
* greet
  - utter_greet
* account_balance
  - utter_collect_acctId
* account_balance
    - utter_collect_acctId
    - slot{"acctId":"3333007555"}
* acctId_collector{"acctId":"3333007555"}
    - slot{"acctId":"3333007555"}
    - action_acct_info
* bot_challenge
    - utter_goodbye


## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot
