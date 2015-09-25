---
ID_PAGE: 25151
PG_TITLE: Action
PG_VERSION: 2.1
TAGS:
    - Action
---
##Description

class [Action](/classes/2.2/Action)



##Constructor

##new [Action](/classes/2.2/Action)(triggerOptions, condition)

Actions are a simple way to add interactions in your scenes. An action is launched when its trigger is fired.
See more here

####Parameters
 | Name | Type | Description
---|---|---|---
 | triggerOptions | any | 
optional | condition | [Condition](/classes/2.2/Condition) | 

##Members

###triggerOptions : any

The trigger options

###trigger : number

Number of the trigger

##Methods

###getTriggerParameter() &rarr; any

Get the trigger parameter
###execute(evt) &rarr; void

Execute the trigger

####Parameters
 | Name | Type | Description
---|---|---|---
 | evt | [ActionEvent](/classes/2.2/ActionEvent) | 

###then(action) &rarr; [Action](/classes/2.2/Action)



####Parameters
 | Name | Type | Description
---|---|---|---
 | action | [Action](/classes/2.2/Action) | 
