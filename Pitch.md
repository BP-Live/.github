# Budapest Live - Pitch

## Structure

- problem statement
    - creating 15 minute cities
    - empty business premises
- solution
    - what is it?
        - service for entrepreneurs to find their optimal business premises
    - why does it help?
        - recommends vacant business premises, helps the city to fill them up
        - shows the amount of competitors in the area, incentivizing the user to choose an area where that kind of service does not exist yet
- feasability
    - demo
        - user specifies their business needs
        - user gets a map showing competitors, vacant businesses, a heatmap of the availability of the kind of service
        - user can see pros/cons of the area, a business name suggestion, list of competitors
        - tech stack
            - next.js frontend
                - mobile-optimized - encourage the audience to try it!
            - fastapi backend
                - auto-scaling deployment on azure - high capacity
            - google maps api
        - how is AI utilized? (this is worth like 35%)
            - openai gpt 4 api
                - communicating needs, insights with user using natural language
    - data sourcing
        - google maps api
        - bkk api
        - property occupancy data
            - currently static
            - limited to 8th district
            - only option to source: local government
        - google pois
            - currently static
            - limited to budapest
            - we could source it from google in the future
    - business model (future)
        - target group: entrepreneurs
        - mainly public benefit
            - solves problems of the city
            - should have a free tier to reach goals and convince users initially
        - monetization, capital?
            - charging premium for more insights
                - location for corporations is a critical decision, information is probably worth more to them then our price

## Draft

Good afternoon! We are team Budapest Live. In Budapest a stunning 3000 retail spaces lay vacant, mirroring a global urban challenge. This number is increasing by 15% to 20% every year. These unutilized spaces represent not only a loss for the city's economy, but also a missed opportunity for local entrepreneurs. Our innovative app targets this issue, helping business owners find and revitalize these spaces, pushing Budapest closer to being an efficient 15 minute city where every need is within reach. 

Our solution enables users to input their business ideas and receive a comprehensive map highlighting vacant premises, local competitors and even a heatmap of services in the area. To achieve this we leverege cutting-edge AI technology, including OpenAI's GPT-4, to provide the user with a detailed description of the possibilities at that location. It even offers the users a fun name idea they could possibly use.

The technical backbone of our solution is robust and future-proof. We've developed a user-friendly, mobile optimized Next.js frontend, supported by a scalable FastAPI backend hosted on Microsoft Azure using Docker containerization.

Our monetization strategy is straightforward. We'll offer a free tier to attract users and showcase the potential of our solution to future customers. We plan to develop a premium tier with advanced features like automatic financial analysis using data acquired from other sources. We plan to add personalized business recommendations in favor of larger corporations.

Our priority is to enhance the versatility of our data sources. We plan to regularly update our property datbase and our points of interest dataset - currently provided by the Budapest Foundation for Enterprise Promotion. We plan to introduce integration with public transport links, providing users with up-to-date information to make their business reachable in a 15 minute city.

## Final

> **Value proposition:** Helping business owners to occupy vacant premises, pushing Budapest to become a 15-minute city.

### Problem definition

Good afternoon! We are team Budapest Live. The unutilized business premises represent a loss for the Budapest's economy, a missed opportunity for local entrepreneurs and makes people travel more than they should to get their needs met which results in more pollution and traffic. We've developed an app which tackles this issue by revitalizing these spaces, bringing Budapest closer to being an efficient 15-minute city.

### Solution, demo

Our solution is a service is targeted towards business owners. It helps to find the optimal business premises for them. On the landing page the user logs in using Google, gives location access and specifies the needs of their business including a location heuristic, which can be just "nearby" as well. After filling out the form, the user is presented with a map showing competitors in the area, recommended vacant business premises and a heatmap of the availability of the kind of service. The user gets a list of pros and cons of the area as well, which incentivizes them to choose an area where that kind of service does not exist yet.

### Technology, AI

The technological backbone of our solution is built with FastAPI and is hosted by Microsoft Azure, withstanding high traffic through auto-scaling. The frontend is built using Next.js. 

We use OpenAI's GPT-4 Turbo model to communicate the business needs and insights with the user through natural language. We used prompt engineering to supply it with data regarding the current location of the user and nearby businesses with similar profiles. We categorize businesses using location and type based clustering using the point of interests dataset.

### Feasability - business model

We created this service mainly for public benefit. Therefore, we plan to have a free tier to reach our social and environmental goals and convince users initially. In order to make our business sustainable, we plan to monetize it by charging premium for providing more detailed insights and automatic financial analysis, as we suspect that this information would be more valuable for large corporations than the price they would have to pay for our service. 

### Feasability - data sourcing

We use the Google Maps API to display the map to the user which is dynamically updated in time, however about the property occupancy and the points of interest we only have static data, and only for the 8th district and Budapest respectively. To make our service applicable in any city, we will have to work together with the local governments to get access to these datasets.

Our web app is optimized for mobile, therefore we encourage you to try it out on the link above. Thanks for your attention!
