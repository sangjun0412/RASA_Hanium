## story_1
* greet
  - utter_greet
* ask_shipfee{"fee": "shipfee"}
 - utter_shipfee


## story_2
* greet
  - utter_greet
* ask_freightfee{"fee": "freightfee"}
  - utter_freightfee
  - action_reset_all_slot

## story_5
* greet
  - utter_greet
* ask_latefee{"fee": "latefee"}
  - utter_latefee
  - action_reset_all_slot
## story_3
* greet
  - utter_greet
* ask_fee{"fee": "사용료"}
  - utter_ask_price
* ship_fee2
  - utter_freightfee
  - action_reset_all_slot
## story_4
* greet
  - utter_greet
* ask_fee{"fee": "사용료"}
  - utter_ask_price
* ship_fee1
  - utter_shipfee
  - action_reset_all_slot
## story_6
* greet
 - utter_greet
* ask_fee{"fee": "사용료"}
 - utter_ask_price
* ship_fee3
 - utter_latefee
 - action_reset_all_slot


## fac form
* greet
  - utter_greet
* request_facility_info
  - fac_form
  - form{"name": "fac_form"}
  - form{"name": null}
  - action_reset_all_slot

## ship form
* greet
  - utter_greet
* request_ship_info
  - ship_form
  - form{"name": "ship_form"}
  - form{"name": null}
  - ship_form2
  - form{"name": "ship_form2"}
  - form{"name": null} 
  - action_reset_all_slot

