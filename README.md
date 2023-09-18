# Open AI MovieDB Chatbot
This solution architecture proposal demonstrates how to effectively utilize OpenAI's language model to create a chatbot to chat with a movie database, extracted using BeautifulSoup from themoviedb.org.


**Architecture**

![moviedbazurechatbotarchitecture](https://github.com/KrishJain8/OpenAiMovieDBChatbot/assets/144550457/282405c1-c688-49f0-a980-6eb4e251ce98)


**Dataflow**

**Extract**: Movie information, such as name, genre, cast, showtimes, reviews, etc. can be extracted from themoviedb.org

**Transform**: The extracted data from themoviedb.org is transformed into a CSV file or alternatively a SQL DB and saved into Azure Block Storage.

**Create**: Create an OpenAI instance and call the block file.

**Chat**: Chat with Movie DB storage file.




**Components**

These are the key technologies used for this technical content review and research:
- Python
- BeautifulSoup
- themoviedb.org
- Azure OpenAI
- CSV file
- Azure Block Storage



**Scenario details**

This solution helps users to explore a movie database to find current movie information of all kinds to plan for watching a movie or exploring new movies based on the metadata of movies.


**Potential Use Cases**

By leveraging this chatbot, users can ask questions based on their preferences, schedule, or other factors for movie-watching. The chatbot responds in a concise manner based on user preferences. This chatbot can help users make an informed decision based on movie parameters when struggling with lots of movie choices. This process improves the experiences of users interested in movies, whether to watch a movie or for generally accessing current movie information.

My solution can be integrated with movie ticketing or theater websites to enhance user experience to search for movies and to purchase movie tickets directly through a chatbot.

**Scenario 1**: John Doe wants to watch a movie with his 8-year-old son. He intends to watch the movie on the upcoming weekend. John asks the chatbot for a kid-friendly movie that has available showtimes on the upcoming weekend.
