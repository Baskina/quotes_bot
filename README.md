# MongoDB Query Bot

This Python bot is designed to retrieve information from a MongoDB database based on user requests. The MongoDB database is hosted on Atlas MongoDB. Data was populated into the database using JSON files via a Python script in the `seeds.py` file, utilizing the ODM Mongoengine.

## Bot Commands:

- **name**: `<Author name>`
  - Retrieves quotes by the specified author.

- **tag**: `<tag>`
  - Retrieves quotes associated with the specified tag.

- **tags**: `<tag1,tag2...>`
  - Retrieves quotes associated with multiple tags.

- **exit**
  - Ends console communication with the bot.

The bot also supports searching based on partially typed author names or tag.

## Example Usage:

```
Enter command: name: Steve Martin
Steve Martin
“A day without sunshine is like, you know, night.”

Enter command: tag:life
Albert Einstein
“There are only two ways to live your life. One is as though nothing is a miracle. The other is as though everything is a miracle.”

Enter command: tags:life,live
Albert Einstein
“There are only two ways to live your life. One is as though nothing is a miracle. The other is as though everything is a miracle.”

Enter command: tag:li
Albert Einstein
“There are only two ways to live your life. One is as though nothing is a miracle. The other is as though everything is a miracle.”

Enter command: exit