
![]
(http://www.plantuml.com/plantuml/img/SoWkIImgAStDuIejJYrIqBLJA2ujI2tAJIpAJYrHi58eJyp9LiZCqz24owVbvwS09P8pylEBKnLAyXMIIYkHf7Fpyr8hWV85YI1HBeVKl1IWwG00)

@startuml
user -> supermarket : walk in()
user -> food : choose to buy()
user -> money : pay()

@enduml


![](http://www.plantuml.com/plantuml/img/TP9Dai8W48Ntdg8hArtC1LXCUOAv0pyzXXB35DreUVjfI4XIegiGtlSQtalEn3fnleL39apmzGq9BvvOrcfR5kruMf4GBtu2fPdnziV0STuvdk0mIy8CJhCs6WZ5TCSqAB0ZsckT1N8gPvAH7LQz3pImsbuCEwsmLLNBbIXRYqI_ENmcvr2QVPpW1z6XsoLhYVliwtlBhwfd2RuEC35UvH2JueCGQ9H7hzennaK5FJcG3b2eghRunJ90AqtVjG_Q-E3vsQBDn5PrcTWws_DTsHluMZQejoVr9IvKmFBnoxq5FUFav4Vw1m00)
@startuml
user -> register : register user()
user -> login :attempt to login() 
login -> "databa seserver": check user status()
"databa seserver" -> "web server": user status()
"web server" -> user : login successful()
"web server" -> user : registation Needed()
user -> register: register user()
register -> login:user login()
user -> book : browse shows()
user -> book : choose show and date()
book -> "web user" : check availability()
"web user" -> "database server": availability status()
"database server" -> "web server" : availability()
"web server" -> user : available to book()
@enduml

![](http://www.plantuml.com/plantuml/img/SoWkIImgAStDuSfFIyjCJYrIqBLJo2zA0JAi5D9JInJymMpFlBHy3Kqki0HGGN9fSKb-BboDCv2BeWHaI45HVaffSWbKIG2KXwuAPbLoOawoWdj9VabY3eeqr55M2YcPnGKvYPKAHQd5fJabG3KEgNafG7S30000)

@startuml
officer -> order : get Order Info()
order-> customer : get Cust Info()
order -> product : get Product Info()
order -> order : calc Gtotal()
order -> officer : display result()
@enduml

![](http://www.plantuml.com/plantuml/img/SoWkIImgAStDuIejJYrIqBLJICxFBIWj0RAj598pKfEpNNCJCtCqDBbWua0bG9LbO0N5gNaf2gLvGAf48HLDdGAomhpKShW2g22gLKMfnGNvG8Dm6H0DDo5M8IM_F2ydFp45lvKfgJcf9QaA-Ja8TGv0vmAz2W00)

@startuml
user -> computer : checkEmail()
computer-> server : send unsent email()
computer -> server : new email()
server -> computer : response()
computer -> server : [new email] download email()
computer -> server : delete old email()
@enduml

