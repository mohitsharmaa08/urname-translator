# urname-translator
 
# Urname Translator

## List of Contents
- Descritpion
- Input
- Output
- Processing
- Screenshots
- Link

> **Description:** Want cool nerdy name, if yes then get your name in two different langugaes one is `Binary speak: the way your computer pronounces it` another is `Leet speak: hacker's name`. Just enter your name and get it translated into different languages. `Leet speak` name can also be used as user name for accounts, if media platform allows hackers it do chit-chat. For this app we have use `funtransalations.com API` to translate user input. Urname Translator has two pages as stated formely, both takes user name or any text as input and converts into desired language. 

<br>

> **Input:** A user has to enter his or her name or any text on choice of page and wait for atmost 5 seconds to get input translated. A empty input get epmpty output but with silence. Inputs dont have any constraints as input can be user name or any text which to be transalted.

<br>

> **Output:** User will get to know translated input in five seconds of clicking `Translate` button in the `green` output sectionexcept `API RATE LIMIT REACHED` if rate limit reached then user is informed with alert and told to try after X duration. 

<br>

> **Processing:**
- User has to enter his or her name or any input text and click on translate button on each page.
- If user entered input is empty, then user will get empty output.
- After clicking on transalte button on any page an API request is made to url `api.funtranslations.com/translate/[type].json` requesting text to translated, then based upon response recieved user is updated either with output or alert. On each page same process is done requesting API then taking action based on response.
- (continued) First user input is checked if it contains some text then API call is made else not, after that (if contains) then with user input is concatenated with desired api url, then encoded and then using fetch API or function request is made and response is taken and check for whether it contains data for request or not if contains then user is updated else alert is send to user, meanwhile error handling is done using catch while API request is being made.

<br>



<br>

> **Link:** [Urname Translator](https://urname-translator.netlify.app/index.html)