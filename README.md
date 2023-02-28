# Business On Bot - Backend Task

This is a backend REST service that provides bank details through three API endpoints, built using NodeJS, ExpressJS, and MongoDB Atlas.

  1.POST api/import-csv: Uploads CSV data into MongoDB.
  2.GET api/search: Searches for bank details by city name, with optional limit and offset parameters. Results are ordered by IFSC code in ascending order.
  3.GET api/branch: Searches for bank details by city name, with optional limit and offset parameters. Results are ordered by IFSC code in descending order based on    branch name.
With this service, users can easily retrieve bank details using various search parameters, making it a simple and efficient solution.


# Case 1
Search API to return possible matches across all columns and all rows, ordered by IFSC code (ascending order) with limit and offset.

Request URL - /api/search?q=Mumbai&limit=2&offset=1

![Screenshot 2023-02-28 191227](https://user-images.githubusercontent.com/73026163/221874075-bd8e9c57-b780-4024-8d17-b758cd53d26a.png)

image:

# Case 2
Branch API to return possible matches based on the branch name ordered by IFSC code (descending order) with limit and offset

Request URL - /api/branch?q=LONI&limit=1&offset=1

![Screenshot 2023-02-28 191135](https://user-images.githubusercontent.com/73026163/221874092-61a8314b-e7bb-4bb7-b415-f7277625209f.png)
