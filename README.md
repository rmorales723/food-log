## Project Description

This project is a basic food log which tracks calories, proteins, carbohydrates, and fats.
#
We have a New Entry react component that posts the user typed data for the meal type being created from the frontend to the Rails backend API. It lets the user add the meal type information (e.g. meal type, calories, proteins, carbohydrates, and fats).

When the user hits the Create Entry button after typing the information, it makes a POST /foodlog API call to the backend Rails API with the meal type information in the request body and the food log record is created and saved in the backend database.

![Screen Shot 2022-12-27 at 4 10 12 PM](https://user-images.githubusercontent.com/72527380/209723400-7848991d-2181-4501-9fae-8b31a18bdabd.png)
#

The user is able to display all the entries, and the total sum of calories, proteins, carbohydrates, and fats logged for each day.

![Screen Shot 2022-12-27 at 4 09 04 PM](https://user-images.githubusercontent.com/72527380/209723405-0df61b03-fc80-4e9b-a9b3-383cbe42aceb.png)
#
We have a Display Entries react component that makes a fetch API call (GET /foodlog) to the Rails backend API to fetch all the foodlog data that are present in the database, and then displays each foodlog in the UI. We have a foodlog react component to render each meal type data in the UI.

We have EDIT and DELETE buttons that give the user the ability to edit a meal type information and delete the food log.

When the user clicks on the DELETE button, it makes a DELETE request to the Rails backend API and deletes the food log record from the database.

![Screen Shot 2022-12-27 at 4 10 57 PM](https://user-images.githubusercontent.com/72527380/209723412-c7e01b12-f955-4dac-aaf5-c78133f6661b.png)
#
Implemented error handling.

![Screen Shot 2022-12-27 at 4 13 40 PM](https://user-images.githubusercontent.com/72527380/209723414-a85634c1-a3ef-4829-9d49-29af31e92f2e.png)
![Screen Shot 2022-12-27 at 4 14 19 PM](https://user-images.githubusercontent.com/72527380/209723421-0202ba46-9118-4b93-8764-1cc13061f690.png)
