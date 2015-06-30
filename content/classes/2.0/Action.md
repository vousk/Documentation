---
ID_PAGE: 5726
PG_TITLE: Action
PG_VERSION: 2.0
---
##new [Action](page.php?p=5726)(triggerOptions, condition)


Actions are a simple way to add interactions in your scenes. An action is launched when its trigger is fired.
See more [here](https://github.com/BabylonJS/Babylon.js/wiki/How-to-use-Actions)


####Parameters
 | Name | Type | Description
---|---|---|---
 | triggerOptions | any | Options of the trigger
optional | condition | [Condition](page.php?p=5742) | [Condition](page.php?p=5742) to trigger the action
---

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
 | evt | [ActionEvent](page.php?p=5740) | An event to trigger
---

###then(action) &rarr; [Action](page.php?p=5726)

####Parameters
 | Name | Type | Description
---|---|---|---
 | action | [Action](page.php?p=5726) | The action to do
---