# Alexa Recipes #
Alexa Recipes is an Amazon Echo voice skill and accompanying web app. Users can browse recipes online and send them to their Amazon Echo device. Then they can interact with Alexa via voice to work their way through the recipe step by step.

## Problem Statement ##
Many people use laptops, phones, or other screened devices to reference recipes while cooking. However, it can be inconvenient to constantly unlock these devices and to interact with them with full or messy hands in the kitchen . My capstone will provide one solution to this problem by allowing users to interact with their chosen recipes via voice.

## Feature Set ##
**Link accounts**: Users will create an account on my website and link it to their existing Amazon (Echo) account via OAuth.  
**Browse recipes**: On my website, users will be able to search and browse a large database of recipes, which includes recipes from popular sites like [Allrecipes](http://allrecipes.com/). This will be facilitated by my site's integration of the [Yummly API](https://developer.yummly.com/).  
**Save recipes**: On the website, users will star/save recipes that they would like to have access to on their Echo device. These recipes will be saved in the user's account.  
**Interact with recipes**: Via voice, users will launch the Recipes skill on their Echo device and then open a specific recipe of their choice. An intuitive voice interface will let users ask what step of the recipe they're on and what's coming up. Users will also be able to ask basic questions about ingredients and preparation time.  

**Other potential features (non-MVP)**:  
**Input and share recipes**: Users can input their own recipes on my website and publish them to share with other Alexa Recipes users.  
**Browse by category via voice**: With recipes categorized by type, users can ask Alexa to name aloud which recipes of a certain type a user has saved.

## Technology Choices ##
**Amazon Echo/Alexa**: I'll be creating an Amazon Echo skill by using the [Alexa Skills Kit](https://developer.amazon.com/public/solutions/alexa/alexa-skills-kit/getting-started-guide).  
**OAuth**: Users will link their account on my website to their Amazon account used on their Echo device.  
**Background jobs (email)**: I'll send email to users to confirm their account on my website and the successful linking of their account with their current Amazon account.   
**MongoDB**: Recipes and user info will be saved as MongoDB documents.  
**SSL**: To be published as an Alexa Skill, my application must make requests over HTTPS.   
